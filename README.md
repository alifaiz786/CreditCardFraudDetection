# Credit Card Fraud Detection Using Unsupervised Learning

# Overview

This project utilizes unsupervised machine learning algorithms to detect fraudulent credit card transactions. It explores two major techniques: Isolation Forest and Local Outlier Factor, applying them to an anonymized credit card dataset to identify outliers that are likely fraudulent transactions

# Project Goals

- Understand and explore the dataset with visualization techniques.
- Implement and compare the performance of two unsupervised anomaly detection algorithms.
- Evaluate model accuracy, precision, recall, and F1-score for both approaches.

# Tools & Libraries

- Python 2.7.13 (from Anaconda distribution)
- Libraries: NumPy, Pandas, Matplotlib, Seaborn, SciPy, scikit-learn

# Dataset

- Source: [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- Features: 30 PCA-transformed variables + `Time`, `Amount`, and `Class` (fraud indicator)
- Extremely imbalanced dataset (fraud cases are ~0.17%)

# Workflow

1. Importing Libraries & Checking Versions
2. Loading and Sampling the Dataset (10% of original)
3. Exploratory Data Analysis (EDA):
   - Statistical summary using `describe()`
   - Histograms of all features
   - Correlation heatmap
4. Data Preparation: Feature matrix `X` and target `Y` (Class)
5. Applying Unsupervised Models:
   - Isolation Forest
   - Local Outlier Factor
6. Evaluation using Accuracy, Precision, Recall, and F1-score

# Evaluation Metrics

- Accuracy Score
- Precision
- Recall
- F1-Score

Each model's performance is reported and compared based on its ability to identify rare fraud cases.

# Results

| Model                | Fraud Detection Accuracy | Precision | Recall | F1-score |
|---------------------|--------------------------|-----------|--------|----------|
| Local Outlier Factor| Moderate                 | Low       | Low    | Low      |
| Isolation Forest    | Better                   | Higher    | Higher | Higher   |

Isolation Forest performed significantly better in terms of balancing precision and recall.
