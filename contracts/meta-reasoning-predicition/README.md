# GiverLiquidity Prediction Protocol

A binary prediction market on Sui where users bet on:
> "Will more people donate or not?"

## Features

- Binary betting market: Yes vs No
- Sui Move smart contract
- On-chain resolution using GiverRegistry
- Simple reward claiming system

## How to Build

```bash
sui move build
```

## How to Deploy (Testnet)

```bash
sui client switch-env testnet
sui client publish --gas-budget 500000000
```

## Author

ARM3rd / GiverLiquidity Hackathon Team
