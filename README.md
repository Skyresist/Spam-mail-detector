# 📧 Spam Email Detection (Up to 98% Accuracy)

A machine learning project to detect spam emails using various models like Multinomial Naive Bayes and Logistic Regression.  
Achieved up to **98% accuracy** with CountVectorizer + MultinomialNB.

---

## 📊 Dataset Overview

- 5,572 labeled SMS/email messages
- Two classes: `spam` (1) and `ham` (0)
- Common spam themes: prizes, urgent actions, offers

---

## 🧹 Data Preprocessing

- Lowercased all text
- Removed punctuation and numbers
- Removed stopwords
- Applied optional stemming
- Created additional feature: `email_length`
- Handled outliers by trimming top/bottom 1% message lengths

---

## 🤖 Models and Methods

- **Multinomial Naive Bayes** + **CountVectorizer**
- **Multinomial Naive Bayes** + **TfidfVectorizer**
- **Logistic Regression** + **TfidfVectorizer**
- Feature combination: text + email length using ColumnTransformer

---

## 📈 Results

| Model | Accuracy |
|-------|----------|
| MultinomialNB + CountVectorizer | **98%** |
| MultinomialNB + TfidfVectorizer | 96.4% |
| Logistic Regression + TfidfVectorizer | 96.5% |

- Best model: **MultinomialNB + CountVectorizer (98%)**
- Balanced recall and precision for spam detection.
