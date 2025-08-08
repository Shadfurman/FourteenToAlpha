# FourteenToAlpha
# FourteenToAlpha

**FourteenToAlpha** is a 14-day sprint to build a complete, end-to-end trading bot — from raw market data to backtested equity curves — with zero scope creep.

## Project Goals
- Train a simple but effective model (Conv-Transformer, CNN+GRU fallback) on daily OHLCV data.
- Produce reproducible backtests with walk-forward validation.
- Export a minimal inference function: **buy / flat / sell** for any ticker.
- Keep scope small enough to finish in 14 days.

## Data
- **Source:** NYSE + NASDAQ historical daily OHLCV (adjusted closes for splits/dividends).
- **Format:** CSV → Parquet conversion for speed & compression.
- **Features:** pct-change, rolling mean/volatility, RSI(14).

## Tech Stack
- Python, Pandas, NumPy
- PyTorch (model training)
- scikit-learn (baseline models)
- Matplotlib (plots)
- Colab / Google Drive for execution & storage

## Roadmap
**Phase 1 – Skeleton & Data Lock**  
**Phase 2 – Backtest & Baseline**  
**Phase 3 – Model Integration**  
**Phase 4 – Multi-Fold Training & Eval**  
**Phase 5 – Wrap & Deliverable**  

Full roadmap in [`Trading Bot 14-Day Roadmap`](docs/Trading_Bot_14_Day_Roadmap.md)

## License
MIT (or your choice)

---

*This project follows a strict “no side quests” policy: finish the minimal viable pipeline first, then iterate.*
