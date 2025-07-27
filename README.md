# Sentimental analysis
# 📰 Financial Market News - Sentiment Analysis

## 📌 Objective
To build a machine learning model that predicts whether the daily financial market news sentiment is **positive (1)** or **negative (0)** based on 25 headlines per day.

---

## 📁 Dataset
- Source: [YBI Foundation Dataset](https://github.com/YBI-Foundation/Dataset/blob/main/Financial%20Market%20News.csv)
- 4101 rows × 27 columns:
  - 1 Date column
  - 1 Label column (target)
  - 25 headline columns (features)

---

## 🔧 Tools & Libraries
- Python
- Pandas, NumPy
- Scikit-learn (CountVectorizer, RandomForestClassifier)
- Google Colab / Jupyter Notebook
- Matplotlib (optional for visualization)

---

## 🔄 Workflow

### 🧹 1. Preprocessing
- Combined all 25 news headlines into a single string per row.
- Converted text to numerical features using `CountVectorizer` (Bag-of-Words).

### 🧠 2. Model Building
- Split data into train/test (70/30 split).
- Trained `RandomForestClassifier(n_estimators=200)`.

### 📊 3. Evaluation
- Confusion Matrix
- Classification Report
- Accuracy: ~51%
  - Precision (Class 1): ~0.53
  - Recall (Class 1): ~0.73
  - F1 Score (Weighted): ~0.48

---

## ⚠️ Limitations
- Headlines include non-financial news, causing noise.
- Accuracy is low; better models or cleaning techniques (TF-IDF, BERT, stopword removal) could improve performance.

---

## ✅ Learning Outcomes
- Real-world experience in Natural Language Processing (NLP).
- Text preprocessing, vectorization, model building & evaluation.
- Gained insight into how data quality affects ML accuracy.
