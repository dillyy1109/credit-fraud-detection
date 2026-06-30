# 💳 Credit Card Fraud Detection

Machine learning project that detects fraudulent credit card transactions using **Logistic Regression** and **Random Forest** models built with **R** and the **tidymodels** framework.

🌐 **Live Demo:** https://dillyy1109.github.io/credit-fraud-detection/

---

# Project Overview

Credit card fraud is a challenging classification problem because fraudulent transactions make up only a tiny fraction of all transactions. In highly imbalanced datasets like this, traditional accuracy can be misleading.

This project develops and compares multiple machine learning models to identify fraudulent transactions while focusing on metrics that better reflect real-world fraud detection performance.

---

# Project Highlights

- Built end-to-end fraud detection pipeline in **R**
- Compared **Logistic Regression** and **Random Forest**
- Handled severe class imbalance using **downsampling**
- Tuned classification threshold to maximize **F1 Score**
- Evaluated models using **Precision-Recall AUC**, ROC AUC, Precision, Recall, and F1 Score
- Visualized model performance and feature importance

---

# Dataset

**Credit Card Fraud Detection Dataset**

- European credit card transactions
- Binary classification problem

Target variable:

- **0** → Legitimate transaction
- **1** → Fraudulent transaction

The dataset is highly imbalanced, making fraud detection significantly more difficult than standard classification problems.

> The dataset is not included in this repository due to licensing and size restrictions.

---

# Tech Stack

**Language**

- R

**Libraries**

- tidymodels
- ranger
- glmnet
- dplyr
- ggplot2

**Machine Learning**

- Logistic Regression
- Random Forest

---

# Methodology

## 1. Data Preparation

- Stratified 80/20 train-test split
- Normalized numerical features
- Applied downsampling to the majority class during training

---

## 2. Model Development

Two supervised learning models were trained:

### Logistic Regression

- Baseline linear classifier
- Regularized using glmnet

### Random Forest

- Ensemble tree-based classifier
- Implemented using ranger

---

## 3. Model Evaluation

Because fraud detection involves extremely imbalanced data, model performance was evaluated using:

- Precision-Recall AUC (Primary Metric)
- ROC AUC
- Precision
- Recall
- F1 Score

The decision threshold was optimized using the validation set to maximize the F1 Score.

---

# Results

The Random Forest model outperformed Logistic Regression across the primary evaluation metrics.

Key observations:

- Higher Precision-Recall AUC
- Improved recall for fraudulent transactions
- Better balance between precision and recall after threshold tuning
- Feature importance analysis identified the most influential transaction characteristics

*(Replace this section with your actual evaluation metrics if available.)*

---

# Repository Structure

```
credit-fraud-detection/
│
├── images/
│   ├── pr_curve.png
│   ├── roc_curve.png
│   └── feature_importance.png
│
├── creditfrauddetection.Rmd
├── creditfrauddetection.html
├── README.md
```

---

# Future Improvements

Potential enhancements include:

- SMOTE oversampling
- Cost-sensitive learning
- XGBoost implementation
- Hyperparameter tuning
- Time-based train/test split
- Probability calibration
- Model deployment using Shiny

---

# Key Skills Demonstrated

- Machine Learning
- Predictive Modeling
- Fraud Detection
- Classification
- Feature Engineering
- Threshold Optimization
- Model Evaluation
- Data Visualization
- R Programming

---

# About Me

**Dilly Nguyen**

Data Science student at DePaul University with interests in machine learning, predictive analytics, and risk modeling.

- LinkedIn: https://linkedin.com/in/dilly1109
- GitHub: https://github.com/dillyy1109

---

If you found this project interesting, feel free to connect with me on LinkedIn or explore my other machine learning projects.

