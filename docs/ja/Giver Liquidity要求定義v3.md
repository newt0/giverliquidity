# GiverLiquidity - Requirements Definition

## 🎯 Project Overview

**Tagline**: "The Liquidity of Goodwill"

**Brand Message**:

- Donate Swag.
- Mint Reputation.
- Prove You're a GIVER - onchain.

**Mission**: Web3 イベントの Swag 配布文化を社会貢献に転換し、善意の行動をオンチェーンで可視化・流通させる分散型レピュテーションプロトコル

---

## 🌟 Vision & Philosophy

### Why We Exist

Web3 業界は理想的なビジョンで始まったにも関わらず、現在は投機的な側面が強調され、社会的信頼が低下している。私たちは**Web3 を世界の Giver にする**という使命のもと、善意の行動をオンチェーンで証明し、業界のレピュテーション向上を目指す。

### Core Philosophy

- **意思の価値化**: トランザクションに依存しない誠意の記録
- **透明性の確保**: SNS アイデンティティ連携による虚偽抑止
- **社会的信用の構築**: オンチェーン Karma システムの実現

---

## 🎯 Market Analysis & Problem Statement

### Current Market Issues

1. **Swag 供給過多**: Web3 イベントで大量配布される Swag の多くが未使用で余っている
2. **レピュテーション危機**: Web3 業界への世界的な信頼低下
3. **機会損失**: 善意のリソースが有効活用されていない
4. **証明困難**: 個人の社会貢献活動が適切に評価・可視化されていない

### Target Market Size

- グローバル Web3 イベント: 年間 1,000+件
- 想定 Swag 流通量: 年間数百万アイテム
- 潜在寄付価値: 年間数億円相当

---

## 💡 Solution Architecture

### Core Solution

GiverLiquidity は、**Swag 寄付行動をオンチェーン証明書（SBT）に変換**し、個人・企業の社会的レピュテーションを可視化する分散型プロトコルです。

### Key Innovation Points

1. **ゼロコスト実装**: 既存のイベントリソース内で完結
2. **迅速な意思決定**: 追加予算不要のため企業導入が容易
3. **ゲーミフィケーション**: 予測市場との統合でエンゲージメント向上
4. **バイラル設計**: SNS 連携による自然な拡散メカニズム

---

## 🛠 Technical Architecture

### Sui Blockchain Integration

- **SBT (Soulbound Token)**: 非譲渡型レピュテーション NFT
- **Gasless Transaction**: $SUI 非保有者も参加可能
- **高速処理**: Sui の並列実行による快適 UX

### Walrus Storage Integration

- **寄付記録の永続化**: 改ざん不可能な分散ストレージ
- **メタデータ管理**: 画像・証明書類の分散保存
- **コスト効率**: 従来の IPFS より高性能・低コスト

### Cross-Chain Compatibility

- **マルチチェーン対応**: 他チェーンからの参加も可能
- **フィアット決済**: クレジットカードによる寄付対応
- **ソーシャルログイン**: Twitter 連携でウォレット不要参加

---

## 👥 Target Users & Use Cases

### Primary Users (B2C)

- **Crypto Natives**: 既存の Web3 コミュニティメンバー
- **KOL/Influencers**: 影響力のあるオピニオンリーダー
- **Founders**: プロジェクト創設者・経営者層

### Enterprise Users (B2B)

- **L1/L2 Protocols**: レイヤー 1・2 ブロックチェーンプロジェクト
- **CEX/DEX**: 暗号資産取引所
- **Web3 Startups**: 新興 Web3 企業

### Use Case Examples

#### Case 1: ETHGlobal Tokyo

- 参加者がブースで Swag 受領時に QR コード読み込み
- 寄付意思表明 → Reputation SBT mint
- 予測市場で「今回の Giver 率」にベット参加

#### Case 2: 自治体連携イベント（仙台市）

- 地域産品クーポンを Swag 代替として配布
- 寄付先は東北復興支援プロジェクト
- Giver レピュテーションが DAO 参加権に連動

---

## 🔮 Prediction Market Integration

### Meta-Reasoning Market Design

- **Binary Prediction**: 「このイベントでの Giver 率予測」
- **4 分類分析**: 寄付行動(Yes/No) × 予測(High/Low)によるペルソナ分析
- **GameFi 要素**: 予測成功によるリワード配布

### Revenue Streams

1. **Prediction Market Fee**: ベット手数料（2-5%）
2. **Enterprise Licensing**: 企業向けダッシュボード利用料
3. **Data Analytics**: 匿名化された行動データ販売
4. **Premium Features**: Giver NFT 保有者向け限定機能

---

## 📊 Key Performance Indicators

### Primary KPIs

- **Giver Rate**: Swag 受領者中の寄付意思表明割合
- **SBT Mint Volume**: 発行された証明書数
- **Total Donation Value**: 累積寄付額・回数

### Secondary KPIs

- **Prediction Market TVL**: 予測市場での賭け金総額
- **Social Engagement**: SNS 上での UGC 数・リーチ数
- **Enterprise Adoption**: 導入企業・自治体数

### Success Metrics for Sui Hackathon

- **MVP 完成度**: 核となる寄付 →SBT mint 機能の実装
- **Sui/Walrus 活用度**: ブロックチェーン機能の効果的活用
- **社会的インパクト**: 実際の寄付実行・受益者への価値提供

---

## 🚀 MVP Development Plan

### Phase 1: Core Infrastructure (Hackathon Scope)

- Sui 上での SBT smart contract 開発
- Walrus による寄付記録保存システム
- 基本的な Web UI (Next.js)
- Twitter 連携機能

### Phase 2: Prediction Market Integration

- Binary prediction market 契約
- ベット機能 UI/UX
- リワード配布メカニズム

### Phase 3: Enterprise Dashboard

- 企業向け寄付管理画面
- 分析ダッシュボード
- API 提供

---

## 🏗 Technical Stack

### Blockchain Layer

- **Sui Blockchain**: メインチェーン（SBT 発行・管理）
- **Walrus Storage**: 分散ストレージ（証明書・メタデータ）
- **Cross-chain Bridge**: 他チェーンとの相互運用性

### Application Layer

- **Frontend**: Next.js + TypeScript
- **Backend**: Node.js + Express
- **Database**: PostgreSQL (オフチェーンデータ)
- **Authentication**: Social Login (Twitter OAuth)

### Integration Services

- **Payment**: Stripe (フィアット決済)
- **Social**: Twitter API
- **Analytics**: Custom dashboard + Google Analytics

---

## 🌍 Social Impact & Sustainability

### Direct Impact

- **寄付促進**: 未使用 Swag の有効活用
- **災害支援**: 被災地・困窮地域への物資提供
- **透明性向上**: 寄付行動の可視化・検証可能性

### Indirect Impact

- **業界レピュテーション**: Web3 の社会的信頼回復
- **行動変容**: 善意の行動が評価される文化形成
- **コミュニティ形成**: Giver 同士のネットワーク構築

### Sustainability Model

- **自己資金循環**: 予測市場収益による運営資金確保
- **コミュニティ駆動**: DAO 化による分散ガバナンス移行
- **パートナーシップ**: 企業・自治体との持続的協力関係

---

## 🎯 Hackathon Presentation Strategy

### Demo Scenario

1. **Live Demonstration**: 実際の Swag 寄付 →SBT mint process
2. **Technical Deep Dive**: Sui/Walrus 技術活用の説明
3. **Social Impact Showcase**: 実際の寄付先・受益者の紹介
4. **Future Vision**: 予測市場統合後のエコシステム全体像

### Key Differentiators

- **Real-world Problem**: 具体的な社会課題への取り組み
- **Technical Innovation**: Sui/Walrus の特性を活かした設計
- **Scalability**: グローバル展開可能なビジネスモデル
- **Community Impact**: Web3 業界全体への貢献

---

## 📈 Post-Hackathon Roadmap

### Q1 2025: MVP Launch

- 主要 Web3 イベントでのパイロット実施
- 初期パートナー企業の獲得
- コミュニティフィードバック収集

### Q2 2025: Prediction Market Integration

- ゲーミフィケーション要素の本格導入
- 収益モデルの確立
- マーケティング戦略の実行

### Q3 2025: Enterprise Expansion

- 大手企業・自治体との提携
- API 提供開始
- 国際展開の準備

### Q4 2025: DAO Transition

- コミュニティガバナンスの導入
- トークンエコノミクスの設計
- 持続可能な運営体制の確立

---

## 🔚 Conclusion

GiverLiquidity は、Web3 の技術的優位性と社会的責任を両立させる革新的なプロジェクトです。Sui Hackathon を通じて、単なる技術デモンストレーションを超えた、**実際の社会課題解決**と**業界全体への貢献**を実現したいと考えています。

**"Web3 を世界の Giver にする"** - この理念のもと、善意の流通を促進し、より良い未来を築いていきます。
