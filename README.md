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

## Key Findings
- VaR captures central risk but underestimates tail losses
- Exception rate slightly exceeds the theoretical level
- QQ plot shows fat-tailed behaviour typical of equity returns

## Limitations
- Assumes normally distributed returns
- Does not model volatility clustering
- Not intended for regulatory capital calculations

## Future Enhancements
- GARCH-based volatility
- Historical and Monte Carlo VaR
