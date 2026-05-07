# Statistical Arbitrage: QQQ vs SPY Pairs Trading Strategy
**By Aung Myo Win | UCSD | 2026**

## Overview
This project implements a statistical arbitrage pairs trading strategy 
using QQQ (Nasdaq-100 ETF) and SPY (S&P 500 ETF). The strategy exploits 
the mean-reverting relationship between two highly correlated ETFs using 
z-score based signals.

## Key Results
| Metric | Value |
|--------|-------|
| Correlation | 0.9464 |
| Cointegration P-value | 0.0132 ✅ |
| Optimal Z-score Threshold | 2.0 |
| Total Return | +4.51% |
| Sharpe Ratio | 0.2546 |
| Max Drawdown | -7.64% |

## Methodology
1. **Pair Selection** — Identified QQQ and SPY as highly correlated ETFs
2. **Statistical Validation** — Proved cointegration with p-value of 0.0132
3. **Signal Generation** — Z-score based trading signals
4. **Backtesting** — Tested on 2016-2020 historical data
5. **Optimization** — Tested multiple threshold values (1.5, 2.0, 2.5)

## Technologies
- Python, Pandas, NumPy
- yfinance, statsmodels
- Matplotlib

## How to Run
```bash
pip install yfinance pandas matplotlib statsmodels
jupyter notebook Quant_Pairs_Trading.ipynb
```
