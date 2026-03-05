# Coursework 1 — Group 1: Hybrid NLP Preprocessing

## Overview

Three preprocessing pipelines (rule-based, statistical, deep learning) applied to:

- **English:** Sentiment140 Twitter Dataset (1.6M tweets)
- **Swahili:** Swahili News Classification Dataset

Each pipeline is evaluated for topic discovery quality, vocabulary metrics, and meaning preservation.

## Files

- `notebooks/group1_hybrid_preprocessing.ipynb` — main notebook
- `requirements.txt` — Python dependencies
- `data/processed/` — 6 cleaned CSVs (`{language}_{pipeline}.csv`)
- `reports/pipeline_comparison_metrics.csv` — final metrics table
- `reports/figures/` — generated plots

## Quick Start

### On Google Colab (recommended)

1. Open the notebook via the **Open in Colab** badge.
2. Run all cells top-to-bottom — dependencies install automatically.
3. Upload your `kaggle.json` when prompted (download from **kaggle.com → Account → API → Create New Token**).

### Locally

```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

Then open `notebooks/group1_hybrid_preprocessing.ipynb` in Jupyter.

## Notes

- Datasets are downloaded automatically via `kagglehub` — no manual placement needed.
- The Swahili dataset contains **news articles** (not tweets). Cross-language comparisons reflect both language and domain differences.
- Outputs persist to Google Drive on Colab when available; fall back to local filesystem otherwise.
