# System Architecture

## 1. Purpose

Binance Adaptive Futures AI is an independent experimental platform for multi-market cryptocurrency forecasting, prediction recording and systematic outcome verification.

This document describes the high-level research architecture and its current development scope.

## 2. Architecture Overview

The research workflow consists of the following logical stages:

```text
Cryptocurrency Market Data
          |
          v
Data Processing and Validation
          |
          v
Feature Engineering
(36 engineered features)
          |
          v
Forecasting Engine
          |
          v
Multi-Horizon Predictions
(1h / 3h / 6h / 12h / 24h)
          |
          v
BUY / SELL / HOLD Research Signals
          |
          v
Manual Review
          |
          v
Prediction Recording
          |
          v
Outcome Verification and Evaluation
```

## 3. Market Coverage

The current research universe includes:

- BTC
- ETH
- BNB
- SOL
- XRP
- DOGE
- LINK
- ADA
- AVAX
- LTC

The platform is designed to generate five forecast horizons for each market, resulting in 50 forecasts per complete cycle.

## 4. Core Components

### Market Data Layer

Responsible for obtaining and preparing cryptocurrency market information for research.

### Data Processing and Feature Engineering

Processes input data, applies validation and constructs 36 engineered features for forecasting.

### Forecasting Engine

Generates market forecasts across five time horizons.

### Signal Generation

Produces BUY, SELL and HOLD research signals. These are intended for manual review rather than automatic execution.

### Prediction Verification

Records forecasts and compares them with subsequent market outcomes at their respective horizons.

### Evaluation and Risk Analysis

Supports assessment of forecast consistency, prediction errors and relevant trading-cost and risk considerations.

## 5. Operational Safety

The current prototype operates in observation-only mode.

- Automated real-money trading is disabled.
- Exchange order submission is disabled.
- Research signals require manual review.
- No profitability guarantee is made.
- Forecast performance remains subject to further validation.

## 6. Proposed BNB Chain Architecture

BNB Chain integration is a future research direction.

A potential architecture to investigate is:

```text
Off-chain AI Research Platform
          |
          v
Prediction Record Generation
          |
          v
Timestamp and Record Hash
          |
          v
Potential BNB Chain Attestation
          |
          v
Potential Decentralized Storage
```

Potential areas for investigation:

- BNB Chain smart-contract attestations.
- Cryptographic integrity of prediction records.
- BNB Greenfield storage feasibility.
- Data availability and verification.
- Security and cost assessment.

None of these on-chain components is currently implemented or deployed.

## 7. Current Limitations

The platform is an experimental research prototype. Its forecasting outputs have not established reliable net trading profitability.

Further work is required on out-of-sample evaluation, transaction costs, slippage, funding rates, robustness and security.

## 8. Independence

This is an independent project and is not affiliated with or endorsed by Binance or BNB Chain.
