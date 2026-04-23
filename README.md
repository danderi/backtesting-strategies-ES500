# Backtesting Strategies on S&P 500 Futures (ES)

## Overview
Quantitative research project analyzing the statistical edge of popular 
day trading strategies applied to E-mini S&P 500 futures (ES).

## Objective
Compare multiple intraday trading strategies through algorithmic backtesting 
to determine which ones have a measurable statistical edge under different 
market conditions.

## Strategies Analyzed
- [ ] 01 — Opening Range Breakout (ORB)
- [ ] 02 — VWAP Bounce
- [ ] 03 — ICT Optimal Trade Entry (OTE)
- [ ] 04 — Mean Reversion RSI(2)
- [ ] 05 — Comparative Analysis

## Data
- Instrument: E-mini S&P 500 Futures (ESM26)
- Timeframe: 1 minute bars resampled to 5 minutes
- Source: NinjaTrader 8 historical data export
- Period: March 2026 — April 2026 (expanding as more contracts are added)

## Tools
- Python 3.12
- Pandas, NumPy, Plotly

## Project Status
**Current phase:** Data acquisition and environment setup

### Completed
- [x] Environment setup (Python, Jupyter, libraries)
- [x] Data export from NinjaTrader 8 (ESM26)
- [x] Data cleaning and resampling to 5 min bars
- [x] ORB SHORT backtest (Mar–Apr 2026) — 13 trades

### In Progress
- [ ] Acquiring historical contracts (ESU25, ESZ25) for larger sample
- [ ] ORB LONG backtest (May 2025 — Mar 2026)

### Pending
- [ ] VWAP Bounce strategy
- [ ] ICT OTE strategy
- [ ] Mean Reversion RSI(2) strategy
- [ ] Comparative analysis and final conclusions

## Current Results
| Strategy | Period | Direction | Trades | Win Rate | Profit Factor |
|----------|--------|-----------|--------|----------|---------------|
| ORB | Mar–Apr 2026 | SHORT | 13 | 38.5% | 0.85 |

## Conclusions
Work in progress. Results will be updated as each strategy is tested.

## Author
danderi
