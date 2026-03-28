# Credit Card Fraud Detection - Advanced (Level 2 - Project 5)

## Objective
- Perform advanced fraud detection using a combination of supervised models, anomaly detection algorithms, and an autoencoder neural network.

## Dataset
- Same credit card fraud dataset from Kaggle (creditcard.csv).
- 284,807 transactions, approximately 0.17% fraud.
- PCA-transformed features (V1-V28) plus Amount and Time.

## What This Notebook Does

### Data Loading
- Uploads CSV via Google Colab file upload.
- Prints fraud count, percentage, and the imbalance ratio.

### Advanced EDA
- Runs Mann-Whitney U tests on each feature to find statistically significant differences between fraud and legitimate transactions.
- Ranks features by effect size.
- Plots overlaid histograms of the top 6 most discriminating features for fraud vs legitimate.

### Preprocessing
- Scales Amount and Time with RobustScaler.
- Splits data 80/20 with stratification.

### Sampling Strategy Comparison
- Compares four strategies using Logistic Regression as a baseline:
  - No sampling
  - Random undersampling
  - SMOTE
  - ADASYN
- Reports F1 and Recall for each to show the effect of resampling.

### Supervised Models
- Trains three models:
  - Logistic Regression with class_weight='balanced'
  - Random Forest on SMOTE-resampled data
  - XGBoost with scale_pos_weight
- Reports Recall, F1, and AUC for each.

### Anomaly Detection
- Isolation Forest: fits on test data, flags anomalies based on contamination rate.
- Local Outlier Factor (LOF): detects outliers using local density estimation.
- Reports Precision, Recall, and F1 for both.

### Autoencoder
- Trains a neural network autoencoder on only the legitimate (non-fraud) training transactions.
- Architecture: input -> 14 -> 7 -> 14 -> output (reconstruction).
- Computes reconstruction error on the test set.
- Finds the optimal threshold by sweeping over error percentiles to maximize F1.
- Reports Precision, Recall, and F1.

### Model Comparison
- ROC curves for all supervised models.
- Full comparison table covering all 7 approaches (3 supervised + 2 anomaly detection + 1 autoencoder).
- Summary of which methods work best and a recommendation to use an ensemble for production.

## Libraries Used
- numpy, pandas, matplotlib, seaborn, scikit-learn, imbalanced-learn, xgboost, tensorflow/keras, scipy
