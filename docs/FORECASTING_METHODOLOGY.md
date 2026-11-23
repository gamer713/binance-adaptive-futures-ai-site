# Forecasting Methodology

## 1. Objective

Binance Adaptive Futures AI investigates multi-market, multi-horizon forecasting for cryptocurrency markets.

The objective is to generate measurable research forecasts, record their outputs and evaluate their accuracy against subsequent market observations.

This document describes the current research scope. It does not claim that the forecasting approach is profitable or consistently accurate.

## 2. Market Universe

The current research universe contains 10 cryptocurrency markets:

BTC, ETH, BNB, SOL, XRP, DOGE, LINK, ADA, AVAX and LTC.

## 3. Feature Engineering

The current pipeline uses 36 engineered features.

These features are intended to represent relevant market information for forecasting. Their individual definitions, transformations and predictive contributions remain subject to ongoing evaluation.

## 4. Forecast Horizons

The platform generates forecasts across five horizons:

| Horizon | Evaluation target |
|---|---|
| 1 hour | Subsequent 1h market outcome |
| 3 hours | Subsequent 3h market outcome |
| 6 hours | Subsequent 6h market outcome |
| 12 hours | Subsequent 12h market outcome |
| 24 hours | Subsequent 24h market outcome |

Across 10 markets and five horizons, a complete cycle covers 50 forecasts.

## 5. Research Signal Categories

The system produces three research signal categories:

- BUY: Positive directional research indication.
- SELL: Negative directional research indication.
- HOLD: No actionable directional indication under the current signal logic.

These signals are research outputs and require human review.

## 6. Prediction Verification

The project records forecasts for subsequent evaluation.

The verification process is intended to:

1. Preserve the original prediction and its timestamp.
2. Identify the relevant forecast horizon.
3. Obtain the corresponding subsequent market observation.
4. Compare the predicted direction or return with the realized outcome.
5. Record the evaluation result.
6. Analyse performance across markets and horizons.

## 7. Evaluation Considerations

Forecasting research should be evaluated using appropriate measures, potentially including:

- Directional accuracy.
- Prediction error.
- Return-prediction error.
- Performance by market and forecast horizon.
- Stability across different market conditions.
- Out-of-sample robustness.

Realistic trading evaluation must also account for transaction fees, spread, slippage and funding costs where applicable.

No metric should be interpreted as proof of future performance.

## 8. Research Limitations

The platform remains experimental.

Historical performance does not guarantee future results. Further independent validation is required before any claim of reliable trading performance can be made.

## 9. Operational Controls

- Observation-only operation.
- Automated real-money execution disabled.
- Exchange order submission disabled.
- Manual review of research signals.

## 10. Future Research

Potential improvements include more robust out-of-sample testing, calibration analysis, regime-specific evaluation, uncertainty estimation and stronger prediction-record integrity.

BNB Chain integration remains a proposed future research direction.
