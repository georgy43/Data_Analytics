# 🧹 Data Cleaning — Airbnb NYC 2019
**Oasis Infobyte — Data Analytics Internship | Level 1 | Project 4**

---

## 📌 Objective
Clean the Airbnb NYC 2019 dataset by handling missing values, removing duplicates, fixing data types, detecting outliers, and standardizing text — making it ready for reliable analysis.

---

## 📂 Dataset
- **Source:** Airbnb Open Data — New York City 2019
- **Records:** 48,895 listings
- **Columns:** id, name, host_id, host_name, neighbourhood_group, neighbourhood, latitude, longitude, room_type, price, minimum_nights, number_of_reviews, last_review, reviews_per_month, calculated_host_listings_count, availability_365

---

## 🛠️ Tools & Libraries
| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Pandas | Data manipulation & cleaning |
| Matplotlib | Visualizations |
| Seaborn | Heatmap for missing values |
| Google Colab | Development environment |

---

## 🔍 Cleaning Steps Performed

| Issue | Column(s) | Fix Applied |
|-------|-----------|-------------|
| Missing values | name, host_name | Filled with 'Unknown' |
| Missing values | last_review | Filled with 'No Review' |
| Missing values | reviews_per_month | Filled with 0 |
| Wrong data type | last_review | Converted to datetime |
| Duplicate rows | All | Removed duplicates |
| Invalid price | price | Removed rows where price = 0 |
| Price outliers | price | Removed listings above $1000/night |
| Night outliers | minimum_nights | Removed listings above 365 nights |
| Inconsistent text | neighbourhood_group, room_type | Applied strip + title case |

---

## 📈 Visualizations
- Missing Values Heatmap (before cleaning)
- Price Distribution — Before vs After Cleaning
- Number of Listings by Neighbourhood Group
- Average Price by Neighbourhood Group
- Room Type Distribution (Pie Chart)
- Price by Room Type (Boxplot)

---

## 🚀 How to Run
1. Open `Project4_Data_Cleaning.ipynb` in Google Colab
2. Upload `AB_NYC_2019.csv` when prompted
3. Run all cells (`Runtime > Run all`)
4. The cleaned CSV will be automatically downloaded at the end

---

## 📜 License
This project is part of the Oasis Infobyte Internship Program.

---

*#oasisinfobyte #oasisinfobytefamily #internship #python*
