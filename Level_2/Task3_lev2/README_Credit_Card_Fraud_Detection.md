# Credit Card Fraud Detection (Level 2 - Project 3)

## Objective
- Detect fraudulent credit card transactions in a highly imbalanced dataset using SMOTE and supervised ML models.

## Dataset
- Credit card fraud dataset from Kaggle (creditcard.csv).
- Contains 284,807 transactions with only about 0.17% labeled as fraud.
- Features are PCA-transformed (V1-V28) plus Amount and Time.

## What This Notebook Does

### Data Loading
- Uploads CSV via Google Colab file upload.
- Prints the number of fraud vs legitimate transactions and the imbalance ratio.

### Exploratory Data Analysis
- Bar chart of class distribution (normal and log scale).
- Overlaid histograms comparing transaction amounts for fraud vs legitimate.

### Preprocessing
- Scales Amount and Time using RobustScaler.
- Drops the original Amount and Time columns.
- Splits data 80/20 with stratification.
- Applies SMOTE (Synthetic Minority Oversampling) to balance the training set.
- Prints class counts before and after SMOTE.

### Model Training
- Trains three classifiers on the SMOTE-balanced data:
  - Logistic Regression
  - Random Forest
  - XGBoost
- Reports Precision, Recall, F1, and AUC for each.

### Evaluation
- Confusion matrix heatmaps for all three models.
- ROC curves with AUC values.
- Precision-Recall curves.
- Comparison table with the best model based on F1 score.

## Libraries Used
- numpy, pandas, matplotlib, seaborn, scikit-learn, imbalanced-learn, xgboost
