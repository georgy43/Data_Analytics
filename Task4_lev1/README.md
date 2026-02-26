# 💬 Sentiment Analysis on Twitter Data
**Oasis Infobyte — Data Analytics Internship | Level 1 | Project 3**

---

## 📌 Objective
Build a sentiment analysis model to classify tweets as **Positive**, **Neutral**, or **Negative** using NLP and machine learning techniques.

---

## 📂 Dataset
- **Source:** Twitter Data (CSV)
- **Records:** ~162,980 tweets
- **Columns:** `clean_text`, `category`
- **Labels:** -1 (Negative), 0 (Neutral), 1 (Positive)

---

## 🛠️ Tools & Libraries
| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Pandas & NumPy | Data manipulation |
| NLTK | NLP preprocessing |
| Scikit-learn | ML models & evaluation |
| TF-IDF Vectorizer | Feature extraction |
| WordCloud | Text visualization |
| Matplotlib & Seaborn | Plotting |
| Google Colab | Development environment |

---

## 🔍 Key Steps
1. **Data Loading & Cleaning** — Handled nulls, mapped labels to readable names
2. **EDA** — Sentiment distribution, tweet length analysis
3. **Word Clouds** — Visual representation of top words per sentiment
4. **Text Preprocessing** — Lowercasing, URL/mention removal, lemmatization, stopword removal
5. **Feature Engineering** — TF-IDF vectorization with bigrams (10,000 features)
6. **Model Training** — Trained 3 models: Logistic Regression, Naive Bayes, Linear SVC
7. **Evaluation** — Accuracy, Classification Report, Confusion Matrix
8. **Live Demo** — Real-time tweet sentiment prediction

---

## 📊 Models Compared
| Model | Type |
|-------|------|
| Logistic Regression | Linear classifier |
| Naive Bayes | Probabilistic classifier |
| Linear SVC | Support Vector Machine |

---

## 📈 Visualizations
- Sentiment Distribution (Bar + Pie Chart)
- Tweet Length Distribution by Sentiment
- Word Clouds for each Sentiment class
- Model Accuracy Comparison Bar Chart
- Confusion Matrices for all 3 models

---

## 🚀 How to Run
1. Open `Project3_Sentiment_Analysis.ipynb` in Google Colab
2. Upload `Twitter_Data.csv` when prompted
3. Run all cells (`Runtime > Run all`)
4. ⚠️ Note: Preprocessing ~163K tweets takes ~1-2 minutes

---

## 📜 License
This project is part of the Oasis Infobyte Internship Program.

---

*#oasisinfobyte #oasisinfobytefamily #internship #python*
