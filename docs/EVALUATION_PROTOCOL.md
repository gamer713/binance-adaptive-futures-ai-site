# Forecast Evaluation Protocol

## 1. Purpose

This document describes the evaluation principles for Binance Adaptive Futures AI.

The purpose is to measure forecasting performance systematically rather than relying on isolated successful predictions or unverified performance claims.

## 2. Evaluation Unit

Each forecast should be treated as an individual prediction record containing, where available:

- Market or trading pair.
- Forecast creation timestamp.
- Forecast horizon.
- Predicted direction.
- Predicted return.
- Reference market price.
- Model or forecasting-system identifier.
- Subsequent observed market price.
- Verification timestamp.
- Evaluation result.

## 3. Forecast Horizons

Predictions are evaluated against their corresponding subsequent market observations:

- 1 hour.
- 3 hours.
- 6 hours.
- 12 hours.
- 24 hours.

Each horizon should be evaluated independently.

## 4. Verification Principles

The evaluation process should:

1. Preserve the original forecast.
2. Avoid modifying a prediction after its creation.
3. Match the forecast to the correct market and horizon.
4. Compare predictions with subsequent observed market data.
5. Record missing or incomplete observations rather than silently excluding them.
6. Maintain a traceable record of evaluation results.

## 5. Performance Measures

Potential evaluation measures include:

| Measure | Purpose |
|---|---|
| Directional accuracy | Measures correct direction predictions |
| MAE | Measures average absolute prediction error |
| RMSE | Penalizes larger prediction errors |
| Return error | Measures differences between predicted and realized returns |
| Coverage | Measures the proportion of forecasts successfully evaluated |
| Horizon analysis | Compares results across forecast horizons |
| Market analysis | Compares results across individual markets |

Metrics should be selected according to the type of prediction and the availability of reliable observations.

## 6. Avoiding Evaluation Bias

Evaluation should consider:

- Chronological train/test separation.
- Prevention of future-data leakage.
- Appropriate temporal separation between training and evaluation periods.
- Out-of-sample testing.
- Consistent evaluation rules.
- Transparent reporting of unsuccessful predictions.

Historical data used for development should not be presented as independent evidence of future performance.

## 7. Trading-Cost Considerations

Forecast accuracy alone does not demonstrate trading profitability.

Any future strategy evaluation should account for:

- Exchange trading fees.
- Bid-ask spread.
- Slippage.
- Funding payments.
- Execution assumptions.
- Risk and drawdown.

Net performance should only be reported when supported by a clearly documented evaluation methodology.

## 8. Current Development Status

Prediction recording and outcome verification are part of the project's research workflow.

Comprehensive independent validation, robustness analysis and realistic net-performance assessment remain ongoing.

No profitability claim is made.

## 9. Operational Safety

The platform currently operates in observation-only mode.

- Automated trading is disabled.
- Exchange orders are not submitted.
- Research signals are for manual review.

## 10. Future Improvements

Potential improvements include:

- Immutable prediction records.
- Cryptographic integrity checks.
- Reproducible evaluation reports.
- Model-version tracking.
- Independently verifiable timestamps.
- Investigation of BNB Chain-based research attestations.

These proposed improvements are not yet deployed.
