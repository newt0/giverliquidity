# Giver Liquidity 要求定義

## 構成要素

- Tagline
- Vision (Why)
- MARKET & ISSUES (Where)
- Problem (Why)
- Solution (How)
- How to Work (What)
- Features (What)
- Target User (Whom)
- Usecases
- User Flow
- KPIs
- Revenue Model
- Team (Who)
- Resources
- Roadmap
- Tech Stack
- Ending

## Project Phrases

### Tagline

The Liquidity of Goodwill.

### Brand Copy

Donate Swag.
Mint Reputation.
Prove You’re a GIVER – onchain.

### Short Description

A protocol that turns swag donations into on-chain credentials.

## プロジェクト概要

Giver Liquidity は、Web3 イベントで配布される Swag（ノベルティ）を起点に、参加者が寄付または寄付意思を表明することで、その行為を Reputation NFT として Mint できる dApp である。

- **参加者**：Swag を受け取るか、不要であれば寄付。行動をオンチェーンに記録し、NFT として称号を受け取る。
- **出展企業**：余剰 Swag を一括寄付し、その記録を企業の Reputation として活用できる。
- **社会貢献**と**信頼の可視化**を Web3 の文脈で融合し、レピュテーション・プロトコルとして機能する。

さらに、メタ推理型予測市場と統合することで、行動だけでなく「社会の善意をどう見るか」という推論を記録する。SNS シェア設計も重視し、アテンションエコノミーにおいて自然に拡散される構造を持つ。

## VISION (Why)

- 理想主義で始まった Web3 は、今や強欲と欺瞞に満ちた世界になっている。
- 業界の印象は世界的に悪化しつつあり、信頼の再構築が急務である。
- しかし、Web3 だからこそ実現できる「善意の証明」がある。
- GiverLiquidity は、Web3 発の善意を社会に届けることで、信頼を再構築する挑戦である。
- Web3 を「世界の Giver」へ。

## MARKET & ISSUES (Where)

- Web3 業界ではイベントごとに大量の Swag が配布されており、その多くが使われることなく処分されている。
- カンファレンス自体も供給過多で、Swag も過剰供給気味になっている。
- イベント満足度に直接寄与しない Swag の一部を、社会的に必要とされている人々へ届けることで、大きな価値転換が可能である。
- 追加コスト不要で実現でき、既存リソースの再分配により、企業・ユーザー・第三者すべてがハッピーになるスキーム。
- 特に、被災地・孤児院・貧困地域など、イベント開催国周辺への寄付が高い意義を持つ。
- 被災者としての個人的経験を踏まえても、このスキームには確かな価値があると信じている。

## Problem (Why)

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

## Features (What)

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

## Target User (Whom)

### 2C（個人）

- Crypto Native
- KOL や Web3 イベント常連

### 2B（法人）

- L1/L2 プロジェクト
- CEX・Wallet 事業者

## Usecases

### CASE 1: ETHGlobal Tokyo

- T シャツ受領 → 寄付意思表明 → NFT Mint
- プロフィール表示可能な非譲渡型 NFT

### CASE 2: 自治体 × Web3 イベント（仙台市）

- Swag の代わりに地域産品
- 被災地支援プロジェクトと連携
- Reputation NFT による市民参加の可視化

## User Flow

1. Swag を受け取る or 寄付意思を選択
2. UI でフォーム記入 & Wallet 連携（Twitter Login）
3. Mint 実行（SBT）
4. SNS 拡散 or Prediction Market 参加

## KPIs

### 寄付

- Giver 率（Swag 受領者中の寄付割合）
- Mint 数・保持率
- 合計寄付額 & 回数

### Prediction

- ベット総額
- 参加者数

### アテンション

- SNS UGC 数（ツイート等）

### 2B

- 導入企業数・自治体数
- 1 イベントあたりの企業寄付件数
- 対象支援地域・施設数

## Revenue Model

- Prediction Market 参加手数料
- Reputation NFT 連動の広告モデル
- 公的補助金・助成金
- Web3 Grant
- Reputation スコア活用（DAO 選挙参加、特典付与）
- 企業・出展者への導線販売

## Tech Stack

- Sui
- Walrus
- Next.js

## Ending

GiverLiquidity は、Web3 の善意と reputational layer を再定義するプロトコルである。Swag の再分配という物理行動をきっかけに、社会的信頼と経済的価値をつなぐ UX を設計する。このプロジェクトによって、Web3 に希望と信頼を取り戻したい。
