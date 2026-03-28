# Housing Price Prediction (Level 2 - Project 1)

## Objective
- Predict housing prices using Linear Regression.

## Dataset
- Housing price dataset from Kaggle.
- Contains features like area, number of rooms, location details, and the target price column.

## What This Notebook Does

### Data Loading
- Uploads CSV via Google Colab file upload.
- Displays shape and first few rows.

### Exploratory Data Analysis
- Checks for missing values and duplicates.
- Automatically detects the price/target column.
- Generates a correlation heatmap with annotated values.
- Shows top features correlated with the price.
- Plots the price distribution and a Q-Q plot for normality check.

### Preprocessing
- Fills missing numerical values with median.
- Fills missing categorical values with mode.
- Encodes categorical columns using LabelEncoder.
- Drops ID-like columns.
- Splits data into 80/20 train/test.
- Scales features using StandardScaler.

### Model Training
- Trains a Linear Regression model on the scaled training data.
- Predicts on the test set.

### Evaluation
- Reports MAE, RMSE, and R-squared score.
- Plots Actual vs Predicted scatter with the ideal diagonal line.
- Shows feature coefficients as a horizontal bar chart.
- Performs residual analysis with a histogram and residuals-vs-predicted plot.

## Libraries Used
- numpy, pandas, matplotlib, seaborn, scikit-learn, scipy
