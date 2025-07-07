# 🛒 Amazon Product Sentiment Analysis

This project focuses on analyzing customer reviews from Amazon to determine the **sentiment polarity** (Positive, Negative, Neutral) using Natural Language Processing (NLP) techniques.

---

## 📌 Project Overview

Customer feedback on e-commerce platforms like Amazon provides valuable insights into user satisfaction and product performance. This project performs sentiment classification on product reviews using **NLP preprocessing** and a **Multinomial Naive Bayes classifier**.

---

## 📂 Project Structure

Amazon-Product-Sentiment-Analysis/
│
├── data/
│ └── AmazonProductReviewsData.tsv
├── notebooks/
│ └── Amazon Product Sentiment Analysis.ipynb
├── requirements.txt
├── .gitignore
├── README.md


---

## 📊 Dataset

- **Source:** Amazon customer reviews (TSV format)
- **Features:**
  - `review_body`: The actual review content
  - `star_rating`: Rating provided by user (used to infer sentiment)

---

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Libraries Used:**
  - `pandas`, `numpy`
  - `sklearn`
  - `re`, `string`
  - `nltk` (for stopword removal and text processing)

---

## 🔍 Key Steps

1. **Data Cleaning & Preprocessing**
   - Dropping null values
   - Mapping star ratings to sentiment labels:
     - Ratings 1–2 → Negative
     - Rating 3 → Neutral
     - Ratings 4–5 → Positive
   - Text normalization (lowercasing, punctuation & stopword removal)

2. **Feature Extraction**
   - TF-IDF vectorization of cleaned text reviews

3. **Model Building**
   - Using Multinomial Naive Bayes Classifier
   - Train-test split and model evaluation

4. **Evaluation Metrics**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report

---

## 📈 Model Performance

- **Model Used**: Random Forest Classifier
- **Accuracy**: ~83%
- **Observations**: Balanced performance across all three sentiment classes.

---

## 🧪 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Amazon-Product-Sentiment-Analysis.git
   cd Amazon-Product-Sentiment-Analysis


