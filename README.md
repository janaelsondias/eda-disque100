# Disque 100 exploratory analysis

## Unsupervised machine learning

[ML pipeline notebook](notebooks/ml-unsupervised-pipeline.ipynb) covers local data
collection, preparation, feature engineering, model training, and evaluation
without requiring a target variable.

Install dependencies with `uv sync` from the repository root, then select
`.venv` as the notebook kernel and run all cells in order. The notebook reads
`data/trafico-pessoas-2021-2025.csv` and runs from the root or `notebooks/`.
It compares K-Means and Ward clustering using internal metrics and K-Means
seed agreement. A reproducible 5,000-record cap bounds the workload.

Results are exploratory record-level patterns, not individual risk predictions.
Repeated report identifiers are retained unless their entire records are
duplicates. Review reporting bias, feature sensitivity, and report-grouped
stability before interpreting clusters. No record-level results are exported;
clear notebook outputs before sharing.