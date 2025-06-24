# Intraday Electricity Price Analysis – GB Market

## Overview
- Analyzes intraday electricity prices in Great Britain using historical data, renewable generation patterns, and advanced modeling.
- Aims to identify market regimes and build an automated trading strategy.

## Key Insights
- Price Trends: Two daily peaks (8–9 AM, 4–6 PM); Sundays are cheapest.
- Wind Generation: High wind lowers prices (negative correlation).
- Price Volatility: Spikes linked to demand-supply imbalances.
- Market Regimes: Hidden Markov Model (HMM) effectively classifies volatility regimes.

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

## Model Used: LSTM
- Predicts intraday prices using historical data along with wind and solar generation inputs.

## Results
- Return: 98.5%
- Final Capital: £19,849.75
- Sharpe Ratio: 0.13
- Max Drawdown: –14.87%
