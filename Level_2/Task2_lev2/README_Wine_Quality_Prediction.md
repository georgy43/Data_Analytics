# Wine Quality Prediction (Level 2 - Project 2)

## Objective
- Classify wine as Good or Not Good using multiple machine learning models.

## Dataset
- Wine quality dataset from Kaggle.
- Contains physicochemical properties like acidity, sugar, pH, alcohol, etc.
- Target: quality score (converted to binary -- 7 or above is Good).

## What This Notebook Does

### Data Loading
- Uploads CSV via Google Colab file upload.
- Displays shape and first few rows.

### Exploratory Data Analysis
- Checks for missing values.
- Shows the distribution of quality scores.
- Plots a bar chart of quality distribution.
- Generates a correlation heatmap.

### Preprocessing
- Creates a binary label: quality >= 7 mapped to Good (1), rest to Not Good (0).
- Drops the original quality column and any ID column.
- Splits data 80/20 with stratification.
- Scales features using StandardScaler.

### Model Training
- Trains four classifiers:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
  - SVM (with probability estimates)
- Evaluates each on Accuracy, Precision, Recall, F1, and AUC.

### Evaluation
- Confusion matrix heatmaps for all four models side by side.
- ROC curves overlaid on one plot with AUC values in the legend.
- Feature importance chart from the Random Forest model.
- Comparison table with the best model highlighted.

## Libraries Used
- numpy, pandas, matplotlib, seaborn, scikit-learn
