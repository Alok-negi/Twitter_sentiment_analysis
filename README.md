# 🐦 Twitter Sentiment Analysis using NLP & Machine Learning

This project classifies tweets as **positive** or **negative** using Natural Language Processing (NLP) and machine learning models.
It covers **data preprocessing**, **exploratory data analysis (EDA)**, **feature engineering**, and **model training** with TF-IDF vectorization.

---

## 📂 Dataset

**Source:** [Sentiment140 Dataset](https://www.kaggle.com/datasets/kazanova/sentiment140)
**Size:** 1.6 million tweets (balanced: 800k positive, 800k negative)

**Columns:**

* `target` — Sentiment label (0 = Negative, 1 = Positive)
* `id` — Tweet ID (removed in preprocessing)
* `date` — Tweet date (not used in modeling)
* `flag` — Query flag (not used in modeling)
* `user` — Username (removed in preprocessing)
* `text` — Tweet content

---

## 🧹 Data Preprocessing

Steps applied to clean the tweets:

1. Removed unnecessary columns (`id`, `flag`, `user`)
2. Converted sentiment labels from `(4 → 1)` for binary classification
3. Lowercased text
4. Removed punctuation, special characters, and numbers
5. Tokenized text
6. Removed stopwords (NLTK)
7. Lemmatized words

---

## 📊 Model Training & Evaluation

* **Vectorization:** TF-IDF (Term Frequency–Inverse Document Frequency)
* **Model Used:** Logistic Regression (with hyperparameter tuning)
* **Metrics:** Accuracy Score


---

## 📈 Results

* Logistic Regression achieved **high accuracy** on the test dataset.
* Demonstrated the effectiveness of preprocessing + TF-IDF on large text datasets.


