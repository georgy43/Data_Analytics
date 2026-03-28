# Customer Segmentation (Level 1 - Project 2)

## Objective
- Segment customers into distinct groups using K-Means Clustering on marketing analytics data.

## Dataset
- Marketing campaign dataset from Kaggle (marketing_data.csv).
- Contains customer demographics, spending habits, and campaign response data.

## What This Notebook Does

### Data Loading
- Uploads CSV via Google Colab file upload.
- Handles both tab-separated and comma-separated formats.

### Data Cleaning and Feature Engineering
- Fills missing numerical values with median.
- Drops remaining null rows.
- Creates derived features:
  - Age (from Year_Birth).
  - Total_Spending (sum of all Mnt columns).
  - Total_Campaigns (sum of accepted campaigns).
  - Total_Purchases (sum of purchase channels).
  - Total_Children (kids + teens).

### Exploratory Data Analysis
- Correlation heatmap across all numerical features.
- Distribution of total spending.
- Average spending by product category.

### Clustering
- Selects numerical features and removes ID columns.
- Clips outliers at the 5th and 95th percentiles.
- Scales features using StandardScaler.
- Applies PCA to reduce dimensions to 2 components.
- Runs K-Means for K = 2 through 10.
- Uses the Elbow Method and Silhouette Score to find the optimal number of clusters.

### Results
- Assigns cluster labels to each customer.
- Visualizes clusters in 2D PCA space with centroids.
- Generates cluster profiles showing mean feature values per segment.
- Prints a summary with cluster sizes and silhouette score.

## Libraries Used
- numpy, pandas, matplotlib, seaborn, scikit-learn, scipy
