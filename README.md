# Trader Behavior & Market Sentiment Analysis

This repo contains an analysis of trader performance vs the Bitcoin Fear & Greed index.

## Files
- `py.ipynb` - Jupyter notebook with EDA, per-account analysis, Granger tests, event study, visualizations.
- `data/` - place raw `historical_data.csv` and `fear_greed_index.csv` here if you want to run locally.
- `requirements.txt` - Python packages needed.
- `outputs/` - notebook saves outputs to `/mnt/data/trader_sentiment_outputs` when run in this environment.

## How to run
1. Upload `historical_data.csv` and `fear_greed_index.csv` to `/mnt/data` (or edit the notebook paths).
2. Open `py.ipynb` and run cells top-to-bottom in Google Colab or a local Jupyter environment.
3. Results and CSVs will be saved to `/mnt/data/trader_sentiment_outputs`.

## Key findings (brief)
- Initial Kruskal-Wallis test on daily avg PnL by sentiment returned p ≈ 0.10 — not significant at α=0.05 (first pass).
- Recommend per-account segmentation, lag/event studies, and feature engineering for more actionable signals.
