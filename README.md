## Overview
This project combines deep learning and financial optimization by integrating **Long Short-Term Memory (LSTM)** networks with **Mean-Variance Optimization (MVO)**. The goal was to predict asset returns using LSTM and construct an optimized portfolio maximizing the Sharpe Ratio.

## Key Features
- **LSTM Predictions**: Used to forecast future returns of 10 assets based on 5 years of historical price data (2020–2025).
- **Portfolio Optimization**: Selected the top 5 performing assets based on a 6-month moving average of predicted returns and optimized the portfolio using MVO.

## Results
### LSTM Model Performance:
| Stock | RMSE       | MAE        | MAPE      |
|-------|------------|------------|-----------|
| AAPL  | 7.33       | 5.889      | 2.763%    |
| MSFT  | 10.267     | 8.628      | 2.057%    |
| TSLA  | 19.502     | 13.314     | 5.436%    |
| AMZN  | 5.800      | 4.551      | 2.439%    |
| NVDA  | 7.829      | 6.323      | 5.661%    |
| GOOG  | 10.315     | 9.036      | 5.352%    |
| SPY   | 25.698     | 24.070     | 4.412%    |
| XLK   | 7.616      | 6.502      | 2.981%    |
| QQQ   | 9.806      | 7.477      | 1.612%    |
| GLD   | 8.824      | 7.886      | 3.498%    |


### Optimized Portfolio:
- **Weights**:
  - TSLA: 16.51%
  - GLD: 39.24%
  - NVDA: 44.25%
  - AAPL: 0%
  - AMZN: 0%
- **Performance**:
  - Expected Annual Return: 51.57%
  - Annual Volatility: 32.02%
  - Sharpe Ratio: 1.49

## Conclusion
This project demonstrated the effectiveness of combining LSTM predictions with MVO for portfolio optimization. The resulting portfolio achieved a high Sharpe Ratio, reflecting strong risk-adjusted performance.

### Future Work
- Experiment with advanced LSTM architectures (e.g., bidirectional LSTMs or attention mechanisms).
- Incorporate larger and more diverse datasets.
- Explore ensemble methods to improve prediction accuracy.
- Investigate reinforcement learning for dynamic portfolio rebalancing.

---
