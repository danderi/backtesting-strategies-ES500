# Backtesting Strategies on S&P 500 Futures (ES)

## Overview
Quantitative research project analyzing the statistical edge of popular 
day trading strategies applied to E-mini S&P 500 futures (ES).

## Objective
Compare multiple intraday trading strategies through algorithmic backtesting 
to determine which ones have a measurable statistical edge under different 
market conditions.

## Strategies Analyzed
- [x] 01 — Opening Range Breakout (ORB)
- [ ] 02 — VWAP Bounce (in progress)
- [ ] 03 — ICT Optimal Trade Entry (OTE)
- [ ] 04 — Mean Reversion RSI(2)
- [ ] 05 — Comparative Analysis

## Data
- Instrument: E-mini S&P 500 Futures
- Contracts: ESM25, ESU25, ESZ25, ESH26, ESM26
- Timeframe: 1 minute bars resampled to 5 minutes
- Source: NinjaTrader 8 historical data export
- Period: May 2025 — April 2026

## Tools
- Python 3.12
- Pandas, NumPy, Plotly
- Jupyter Notebooks

## Current Results
| Strategy | Period | Direction | Trades | Win Rate | Profit Factor | PnL |
|----------|--------|-----------|--------|----------|---------------|-----|
| ORB | Mar–Apr 2026 | SHORT | 13 | 38.5% | 0.85 | -$838 |
| ORB | May 2025–Mar 2026 | LONG | 178 | 44.4% | 0.96 | -$1,319 |
| ORB + prev close filter | May 2025–Mar 2026 | LONG | 110 | 46.4% | 1.16 | +$2,525 |
| VWAP Bounce v1 | May 2025–Mar 2026 | LONG+SHORT | 1209 | 34.4% | 0.91 | -$14,300 |
| VWAP Bounce v2 (3 velas) | May 2025–Mar 2026 | LONG+SHORT | 425 | 35.1% | 1.05 | +$2,438 |
| VWAP Bounce v3 (ATR stop) | May 2025–Mar 2026 | LONG+SHORT | 70 | — | — | pending |

## Conclusions
Work in progress. Preliminary findings:
- ORB without filters shows no edge in isolation
- Adding a previous close filter improves ORB significantly
- VWAP Bounce requires more sophisticated entry filters to be viable
- Discrecional context (market phase, balance zones, delta) likely adds significant edge on top of mechanical rules

## Project Status
### Completed
- [x] Environment setup (Python, Jupyter, libraries)
- [x] Data export from NinjaTrader 8 (5 contracts)
- [x] Data cleaning, merging and resampling to 5 min bars
- [x] ORB SHORT backtest (Mar–Apr 2026)
- [x] ORB LONG backtest (May 2025–Mar 2026)
- [x] ORB LONG with previous close filter
- [x] VWAP Bounce v1, v2, v3 (in progress)

### Pending
- [ ] VWAP Bounce — refine entry filters
- [ ] ICT OTE strategy
- [ ] Mean Reversion RSI(2) strategy
- [ ] Comparative analysis and final conclusions

## Author
danderi
