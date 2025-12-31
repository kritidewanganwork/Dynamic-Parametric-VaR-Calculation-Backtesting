# Dynamic-Parametric-VaR-Calculation-Backtesting

## Overview
This project implements a rolling-window parametric VaR model for an equity
portfolio using historical returns and a normal distribution assumption.
The model is evaluated through backtesting and exception analysis.

## Assets
- Apple (AAPL)
- Microsoft (MSFT)
- Google (GOOGL)

## Methodology
- Daily log returns are computed from adjusted prices
- Portfolio returns are calculated using fixed weights
- Mean and volatility are estimated using a rolling window
- VaR is computed at a specified confidence level
- Backtesting is performed by counting VaR exceptions

## Diagnostics
- Rolling VaR vs realized returns
- Return distribution with VaR and Expected Shortfall
- QQ plot to assess normality assumptions

## How to Run
1. Install dependencies:
   pip install -r requirements.txt
2. Open the notebook:
   dynamic_parametric_var.ipynb
3. Run all cells sequentially

## Results Summary
- Rolling VaR closely tracks changes in portfolio volatility
- Backtesting shows a small number of VaR breaches
- Exception rate is slightly above the theoretical level, reflecting fat-tailed equity returns
- QQ plot indicates deviations from normality in the tails

## Limitations
- Assumes normally distributed returns
- Does not model volatility clustering
- Not intended for regulatory capital calculations

## Future Enhancements
- GARCH-based volatility
- Historical and Monte Carlo VaR
