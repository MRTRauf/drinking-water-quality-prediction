# Drinking Water Feasibility Prediction (GAMMAFEST)

Competition project to predict **household drinking-water feasibility** using machine learning (classification), with an emphasis on **F1-score** due to class imbalance.

## Repository contents
- `notebooks/water_quality_prediction.ipynb` — cleaned, publishable notebook version of the competition pipeline
- `notebooks/original_competition_notebook.ipynb` — original notebook (as-is) for provenance
- `data/` — `train.csv`, `test.csv`, and `sample_submission.csv` (competition files)

## Method summary
Based on the accompanying report, the workflow follows CRISP-DM and includes:
- EDA (missing values, imbalance, distribution checks)
- Preprocessing: mode imputation, SMOTE oversampling, outlier removal (Isolation Forest)
- Feature selection (low variance, multicollinearity, adversarial validation)
- Model screening and tuning (tree-based boosting performs best)

The report states the best-performing tuned model is **XGBoost** with **F1 ≈ 95.78%** (std ≈ 0.0014).

## Quickstart (local)
```bash
pip install -r requirements.txt
```

Then open and run:
- `notebooks/water_quality_prediction.ipynb`

## Notes
- This repo is intended as a portfolio artifact showcasing an end-to-end ML workflow.
- If you prefer not to publish full datasets, replace `data/train.csv` and `data/test.csv` with small samples and update the notebook paths accordingly.
