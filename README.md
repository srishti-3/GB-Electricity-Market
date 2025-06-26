# Intraday Electricity Price Analysis – GB Market

## Overview
- Analyzes intraday electricity prices in Great Britain using historical data and technical indicators.
- Aims to identify market regimes and build an automated trading strategy.

## Model Used: LSTM

-LSTM is used to forecast next-hour electricity prices based solely on historical price data.
-It captures time-based trends and volatility through its memory-based architecture.
-The model learns patterns from past price sequences to predict future movements.
-LSTM predictions are combined with technical indicators (like RSI, MACD, and SMA) to generate trading signals.


## Trading Strategy
- Initial Capital: £10,000
- Indicators:
  - RSI (6)
  - MACD
  - SMA (24)
  - ATR (24)
  - LSTM-based predicted prices
- Risk Controls:
  - Position size = 2% of capital
  - Stop-loss = 1.5 × ATR
  - Take-profit = 2 × ATR



## Results
- Return: 98.5%
- Final Capital: £19,849.75
- Sharpe Ratio: 0.13
- Max Drawdown: –14.87%
