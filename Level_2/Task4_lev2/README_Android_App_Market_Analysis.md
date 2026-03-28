# Android App Market Analysis (Level 2 - Project 4)

## Objective
- Perform exploratory data analysis on Google Play Store data to uncover market trends and insights.

## Dataset
- Google Play Store apps dataset from Kaggle.
- Contains app metadata such as name, category, rating, reviews, installs, price, type (free/paid), and size.

## What This Notebook Does

### Data Loading
- Uploads CSV via Google Colab file upload.
- Automatically selects the apps file (excludes review files).
- Displays shape and first few rows.

### Data Exploration
- Checks data types, missing values, and duplicate counts.

### Data Cleaning
- Removes duplicate apps (keeps first occurrence).
- Cleans the Installs column by stripping "+" and "," characters, converts to numeric.
- Cleans the Price column by removing "$", converts to numeric.
- Converts the Size column from strings (e.g., "19M", "500k") to numeric MB values.
- Drops rows with missing Rating values.
- Converts Reviews to numeric.

### Analysis and Visualizations
- Top 15 app categories by count (horizontal bar chart).
- Rating distribution histogram with the mean marked.
- Box plot comparing ratings of free vs paid apps.
- Pie chart showing the proportion of free vs paid apps.
- Top 10 categories by total installs.
- Correlation heatmap of numerical features.

### Key Findings
- Family and Games categories dominate the store.
- Over 92% of apps are free.
- Ratings cluster between 4.0 and 4.5.

## Libraries Used
- numpy, pandas, matplotlib, seaborn, plotly
