以下に、**GiverLiquidity の UX 改善に関する議論を整理して体系化**しました。目的は、**Web3 初心者でも参加しやすい UX の実現と、SNS 連携によるソーシャル・インパクトの最大化**です。

---

## 🧩 **GiverLiquidity UX 設計の課題と改善提案まとめ**

---

### 🟥 【課題】SUI によるガス支払いが高すぎる参入障壁

#### ▸ 問題点：

- Web3 未経験ユーザーが**SUI を持っていない**ため参加できない
- ウォレット作成や CEX/Bridge 経由の SUI 入手が重すぎる手間
- フィジカルイベントやボランティア系文脈に不適

---

### ✅ 【解決策 1】Gasless 構成（Relayer による署名&送信代行）

#### ▸ 技術的アプローチ：

- zkLogin 認証＋ Relayer によるオンチェーン Tx 送信
- 寄付 Tx を**GiverLiquidity 運営側が代行**

#### ▸ メリット：

- **ユーザーは SUI 不要・Wallet 不要**
- イベント参加者や一般人も即参加可能
- Web2 的 UX の実現：ボタンひとつで「寄付を証明」

---

### ✅ 【解決策 2】zkLogin による SNS アカウントログイン

#### ▸ zkLogin とは？

- Google/Twitter などの OAuth ログインを ZK 証明に変換し、**Sui 上の署名者として使える認証方式**
- ウォレットを生成せず、OAuth ID ベースの「署名権限」を構築

#### ▸ 応用例：

- Twitter ログイン → GiverLiquidity 参加
- ユーザーの寄付 Tx に、**Twitter 名 or ハンドル**が結びつく
- ガス代は Relayer 負担

---

## 🌐 **拡張構想：ソーシャルインパクトの可視化**

---

### ✅ 【提案 1】Giver ランキング表示

| 項目     | 内容                                                           |
| -------- | -------------------------------------------------------------- |
| 表示対象 | 累積寄付数、寄付した Swag の数・種類、イベント別ランキング     |
| UI 構成  | Twitter アイコン＋表示名＋寄付数などを表形式やカード形式で表示 |
| 意義     | \*\*「見える善意」\*\*を可視化し、ゲーミフィケーションを導入   |

---

### ✅ 【提案 2】リアルタイム寄付フィード

| 項目     | 内容                                                         |
| -------- | ------------------------------------------------------------ |
| 表示内容 | 「@username が Devcon Swag を寄付しました」などのログ        |
| 技術構成 | オンチェーン Tx ログ＋オフチェーンの Walrus/Arweave への反映 |
| 応用     | イベント会場モニター、公式 Web ページ、SNS シェア誘導        |

---

### ✅ 【提案 3】SNS 連携による UGC 拡散

| 項目   | 内容                                                |
| ------ | --------------------------------------------------- |
| UX     | 寄付後「シェア」ボタンでテンプレ Tweet 生成         |
| 内容例 | 「#Devcon で Swag を寄付しました。#GiverLiquidity」 |
| 目的   | **UGC 創出による自走的なマーケティング効果**の誘発  |

---

## 🔒 安全性と倫理への配慮

- Twitter ハンドル名や表示名は**短縮化 or 匿名加工**を検討（例：`@alice****`）
- 位置情報などの**個人特定性は排除**
- 寄付の意思表明や履歴は**永続ストレージに明記され、改ざん不可**

---

## 📌 結論：推奨構成

| 項目       | 採用案                               |
| ---------- | ------------------------------------ |
| 認証       | zkLogin（Twitter OAuth）             |
| 実行       | Relayer による Gasless Tx            |
| 表示       | ランキング＋リアルタイムログ         |
| 拡散       | SNS シェア導線（Twitter）            |
| ストレージ | Sui Tx + Arweave/Walrus で不変性保証 |

---

この設計により、\*\*「寄付＝善意＝誇り」\*\*を可視化・ゲーム化しつつ、**完全ノンカストディアル・ガスレスな UX**を実現します。
