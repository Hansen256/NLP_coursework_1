# Coursework 1 - Group 1 Hybrid NLP Preprocessing

## Files

- `notebooks/group1_hybrid_preprocessing.ipynb`: main notebook implementation
- `requirements.txt`: Python dependencies
- `data/raw/`: place Kaggle CSV files here
- `data/processed/`: generated cleaned datasets (6 files)
- `reports/pipeline_comparison_metrics.csv`: final metrics table
- `reports/figures/`: generated plots

## Dataset placement

Download and place:

- Sentiment140 CSV as `data/raw/sentiment140.csv`
- Swahili tweets CSV as `data/raw/swahili_tweets.csv`

If your filenames differ, update the `DATA_PATHS` cell in the notebook.

## Setup

```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

## Run

Open and run:

- `notebooks/group1_hybrid_preprocessing.ipynb`

## Notes

- Swahili deep preprocessing uses multilingual transformer tokenization and optional multilingual NER masking fallback.
- The notebook exports 3 cleaned datasets per language: rule/stat/deep (6 total).
