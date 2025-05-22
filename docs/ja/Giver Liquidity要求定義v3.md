# GiverLiquidity - Requirements Definition

## 🎯 Project Overview

**Tagline**: "The Liquidity of Goodwill"

**Brand Message**:

- Donate Swag.
- Mint Reputation.
- Prove You're a GIVER - onchain.

**Short Description**:

A protocol that turns swag donations into on-chain credentials.

## プロジェクト概要

Giver Liquidity は、Web3 イベントで配布される Swag（ノベルティ）を起点に、参加者が寄付または寄付意思を表明することで、その行為を Reputation NFT として Mint できる dApp である。

- **参加者**：Swag を受け取るか、不要であれば寄付。行動をオンチェーンに記録し、NFT として称号を受け取る。
- **出展企業**：余剰 Swag を一括寄付し、その記録を企業の Reputation として活用できる。
- **社会貢献**と**信頼の可視化**を Web3 の文脈で融合し、レピュテーション・プロトコルとして機能する。

さらに、メタ推理型予測市場と統合することで、行動だけでなく「社会の善意をどう見るか」という推論を記録する。SNS シェア設計も重視し、アテンションエコノミーにおいて自然に拡散される構造を持つ。

## Vision

- 理想主義で始まった Web3 は、今や強欲と欺瞞に満ちた世界になっている。
- 業界の印象は世界的に悪化しつつあり、信頼の再構築が急務である。
- しかし、Web3 だからこそ実現できる「善意の証明」がある。
- GiverLiquidity は、Web3 発の善意を社会に届けることで、信頼を再構築する挑戦である。
- Web3 を「世界の Giver」へ。

## MARKET & ISSUES

- Web3 業界ではイベントごとに大量の Swag が配布されており、その多くが使われることなく処分されている。
- カンファレンス自体も供給過多で、Swag も過剰供給気味になっている。
- イベント満足度に直接寄与しない Swag の一部を、社会的に必要とされている人々へ届けることで、大きな価値転換が可能である。
- 追加コスト不要で実現でき、既存リソースの再分配により、企業・ユーザー・第三者すべてがハッピーになるスキーム。
- 特に、被災地・孤児院・貧困地域など、イベント開催国周辺への寄付が高い意義を持つ。
- 被災者としての個人的経験を踏まえても、このスキームには確かな価値があると信じている。

## Problem

- Web3 の世界的なレピュテーションの低下。
- イベントを中心とした Swag の供給過多、およびその UX 価値の低下。
- 善意ある行動が可視化されず、他者に伝播されない設計。

## Solution (How)

- Swag の寄付行動を Web3 的に抽象化し、行動ログとレピュテーションをリンクさせる dApp を開発。
- 参加者の意思・行動をオンチェーンに記録し、NFT（SBT）として称号化。
- SNS 拡散設計によって、行動が社会に伝播する構造を設計。
- さらに、メタ推理型予測市場を導入し、寄付行動に対する「社会的期待や予想」も記録・評価可能に。
- 二択行動 × 二択予測によって、4 パターンの思想ポジションが導出され、グロースにも活用可能。

## 哲学・設計思想

- オンチェーン Tx だけでなく、意志そのものを記録対象にする。
- SNS ID との紐づけにより、虚偽やスパムを抑制。
- Reputation を Web3 における信用の基礎インフラと位置づける。

## Target Market Size

- グローバル Web3 イベント: 年間 1,000+件
- 想定 Swag 流通量: 年間数百万アイテム
- 潜在寄付価値: 年間数億円相当

## How to Work (What)

### 2B 寄付（企業向け）

- Swag を一括寄付 → SBT 発行 + SNS シェア
- Walrus に記録、企業名・Twitter アカウントと紐づけ

### 2C 寄付（イベント参加者）

- Swag 受領時に「受け取る or 寄付する」を選択
- 寄付意思を記録 → SBT ミント用 QR を取得
- Swag ボックス投函後、UI から記録送信 → Reputation NFT を受領

※ センサー等による物理的検証は未導入（工数削減のため）。

### Prediction Market（予測市場）

- Giver or Taker の多数派を予想してベット
- Binary 構造（Yes/No）で UX シンプルに

- Sui チェーン採用
- Walrus によるオフチェーン記録
- zkLogin によるソーシャルログイン（Twitter）
- Gasless Tx 対応
- Prediction Market は無料ベット or トークン報酬型（法規制対策）

### コア機能

- 意思表明 + 記録
- Reputation NFT の Mint
- イベント別・Swag 別の記録可視化
- 企業モードで一括寄付 → 可視化対応

### 拡張機能

- Prediction Market
- Giver 率の可視化
- 報酬配分
- 信頼スコア形成・DAO 参加条件連携

## 👥 Target Users

### Primary Users (B2C)

- **Crypto Natives**: 既存の Web3 コミュニティメンバー
- **KOL/Influencers**: 影響力のあるオピニオンリーダー
- **Founders**: プロジェクト創設者・経営者層

### Enterprise Users (B2B)

- **L1/L2 Protocols**: レイヤー 1・2 ブロックチェーンプロジェクト
- **CEX/DEX**: 暗号資産取引所
- **Web3 Startups**: 新興 Web3 企業

## 🔮 Prediction Market Integration

### Meta-Reasoning Market Design

- **Binary Prediction**: 「このイベントでの Giver 率予測」
- **4 分類分析**: 寄付行動(Yes/No) × 予測(High/Low)によるペルソナ分析
- **GameFi 要素**: 予測成功によるリワード配布

## Revenue Model

- Prediction Market 参加手数料
- Reputation NFT 連動の広告モデル
- 公的補助金・助成金
- Web3 Grant
- Reputation スコア活用（DAO 選挙参加、特典付与）
- 企業・出展者への導線販売

## 📊 Key Performance Indicators

### Primary KPIs

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

## 🏗 Technical Stack

### Blockchain Layer

- **Sui Blockchain**: メインチェーン（SBT 発行・管理）
- **Walrus Storage**: 分散ストレージ（証明書・メタデータ）
- **Wormhole**: 他チェーンとの相互運用性

### Application Layer

- Next.js + TypeScript

### Integration Services

- **Payment**: Stripe (フィアット決済)
- **Social**: Twitter API
- **Analytics**: Custom dashboard + Google Analytics

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

## 🔚 Conclusion

GiverLiquidity は、Web3 の技術的優位性と社会的責任を両立させる革新的なプロジェクトです。Sui Hackathon を通じて、単なる技術デモンストレーションを超えた、**実際の社会課題解決**と**業界全体への貢献**を実現したいと考えています。

**"Web3 を世界の Giver にする"** - この理念のもと、善意の流通を促進し、より良い未来を築いていきます。
