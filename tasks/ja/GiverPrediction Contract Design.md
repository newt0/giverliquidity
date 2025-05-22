以下に、Sui Move をベースにした**GiverLiquidity 予測市場 v1（多数派二択モデル）**の**スマートコントラクト構造設計**を提示します。

---

# **GiverPrediction Contract Design（Sui Move）**

## **前提設計**

- イベントごとに 1 つの予測市場（binary market）
- 賭けは `Yes`（寄付する人が多い） or `No`（しない人が多い）
- 決済は\$SUI または USDC（SUI ベースで設計）
- 結果は `GiverRegistry` に記録された `寄付Tx数` から算出
- 報酬は勝利側に比例配分、プロトコル Fee あり

---

## **1. データ構造（主要構造体）**

```move
struct EventMarket has key {
    id: ID,
    event_id: String,
    total_yes_stake: u64,
    total_no_stake: u64,
    bets: Table<address, BetRecord>,
    resolved: bool,
    outcome: Option<bool>, // true = Yes, false = No
}

struct BetRecord {
    amount: u64,
    prediction: bool, // true = Yes, false = No
    claimed: bool,
}
```

---

## **2. コア関数**

### `create_event_market(event_id: String)`

- 管理者のみ実行可
- `EventMarket` を新規作成して Storage に保存

---

### `place_bet(market_id: ID, prediction: bool, amount: u64)`

- prediction: `true` = Yes, `false` = No
- Stake 金額分の\$SUI を支払い
- `BetRecord` を保存し、マーケットの該当 Pool に加算

---

### `resolve_market(market_id: ID)`

- 管理者または自動実行 Bot
- `GiverRegistry`から `寄付Tx数 / 総参加数` を取得
- 結果（Yes か No）を判断して `EventMarket.outcome` をセット
- `resolved = true` に

---

### `claim_reward(market_id: ID)`

- ベットしたユーザーのみ呼び出し可
- `outcome`が自分の予測と一致していれば報酬受取
- 報酬 = 賭け金 × `TotalLosingPool / TotalWinningPool`
- 3〜5%程度の Fee をプロトコルに送信
- `BetRecord.claimed = true` に更新

---

## **3. 外部参照（GiverRegistry）**

```move
public fun get_decision_count(event_id: String): (u64, u64) {
    // returns (yes_count, total_count)
}
```

→ `resolve_market`で使用
→ 課題としては Bot による自動解決 or DAO 化による結果確定

---

## **4. セキュリティ/UX 補足**

| 項目       | 内容                                                              |
| ---------- | ----------------------------------------------------------------- |
| フロント   | zkLogin で即参加（ウォレット不要）                                |
| ガス補助   | sponsor_tx でユーザー負担ゼロ可能                                 |
| スパム防止 | 最低ステーク額（例：0.1 SUI）設定                                 |
| フェア性   | `resolve_market` は誰でも実行可能だが一度きり。勝手に捏造できない |

---

## **5. ストレージ設計**

- `event_id` をキーに `EventMarket` を格納（storage-efficient）
- 個別ユーザーの BetRecord は `Table<address, BetRecord>` でオンチェーン保持

---

## **今後の拡張案**

| 機能                  | 説明                                 |
| --------------------- | ------------------------------------ |
| 可変オッズ式          | AMM ベースで常にレート変動する設計へ |
| NFT 連動報酬倍率      | 特定 NFT 保有者は 2 倍など           |
| グループ投票/DAO 連携 | 小規模 DAO 単位で賭けさせるなど      |

---
