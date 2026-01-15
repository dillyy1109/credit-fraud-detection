# Credit Card Fraud Detection

## Overview
This project builds a machine learning model to detect fraudulent credit card transactions.
Because fraud cases are extremely rare, the project focuses on **Precision-Recall AUC (PR AUC)**
instead of accuracy.

## Dataset
- Credit Card Transactions dataset (European cardholders)
- Target variable: `Class`
  - `0` = Non-fraud
  - `1` = Fraud
- Highly imbalanced dataset

*(Dataset not included due to size and licensing restrictions)*

## Methods
- Language: **R**
- Framework: **tidymodels**
- Train/Test split: 80/20 (stratified)
- Preprocessing:
  - Feature normalization
  - Downsampling of majority class (training only)
- Models:
  - Logistic Regression (glmnet)
  - Random Forest (ranger)
- Evaluation Metrics:
  - PR AUC
  - ROC AUC
  - Precision, Recall, F1
- Threshold tuning using validation set (maximize F1)

## Results
- Random Forest achieved higher PR AUC than Logistic Regression
- Threshold tuning significantly improved recall of fraud cases
- Feature importance analysis highlights key transaction components

## Files
- `creditfrauddetection.Rmd` – Full analysis and modeling workflow
- `creditfrauddetection.html` – Rendered report
- `images/` – Key plots (PR curves, feature importance)

## Future Improvements
- SMOTE instead of downsampling
- Cost-sensitive learning
- Time-based train/test split
- Model calibration

## Author
**Dilly Nguyen**  
Data Science Undergraduate

