# Drinking Water Feasibility Prediction

Machine learning project to predict household drinking-water feasibility
in Indonesia using structured household and environmental features.

## 🏆 Context
Developed for the **Water Feasibility Prediction – GAMMAFEST** Kaggle competition.
This is a binary classification task evaluated using **F1-score**.

## 🧪 Data
Structured tabular data provided by the competition.
(Full datasets are included here for reproducibility; can be replaced with samples if needed.)

## 🤖 Approach
- Data cleaning & preprocessing
- Handling class imbalance
- Feature inspection
- Model benchmarking (XGBoost, LightGBM, CatBoost)
- Final model selection based on F1-score

## 📊 Results
- **Final model:** XGBoost
- **Metric:** F1-score
- **Score:** **95.78%** (validation)

## 📁 Repository Guide
- `notebooks/water_quality_prediction.ipynb`  
  Clean, readable end-to-end pipeline (recommended for review)
- `data/`  
  Competition datasets (train/test/sample_submission)
- `requirements.txt`  
  Dependencies

## ⚠️ Notes
This repository is intended as a portfolio artifact showcasing an end-to-end ML workflow.
