# 🛒 Amazon Product Sentiment Analysis

This project focuses on analyzing customer reviews from Amazon to determine the **sentiment polarity** (Positive, Negative, Neutral) using Natural Language Processing (NLP) techniques.

---

## 📌 Project Overview

Customer feedback on e-commerce platforms like Amazon provides valuable insights into user satisfaction and product performance. This project performs sentiment classification on product reviews using **NLP preprocessing** and a **Random Forest Classifier**.

---

## 📂 Project Structure

```
Amazon-Product-Sentiment-Analysis/
│
├── data/
│   └── AmazonProductReviewsData.tsv
├── notebooks/
│   └── Amazon Product Sentiment Analysis.ipynb
├── requirements.txt
├── .gitignore
├── README.md
```

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
  - `scikit-learn`
  - `re`, `string`
  - `nltk`

---

## 🔍 Key Steps

1. **Data Cleaning & Preprocessing**
   - Dropping null values
   - Mapping star ratings to sentiment labels:
     - Ratings Compound Score < -0.05 → Negative
     - Rating Compound Score -0.05 and 0.05 → Neutral
     - Ratings Compound Score > 0.05 → Positive
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
- **Observations**: Balanced performance across all three sentiment classes

---

## 🧪 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/sourav-003/PM-Sentiment-Analysis-Project.git
   cd Amazon-Product-Sentiment-Analysis
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate   # For Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

---

## 🙏 Acknowledgements

Special thanks to **Kumar Sundram Sir** and **LearnBay** for their constant guidance and support throughout the project.

---

## 📬 Contact

- **Author**: [Sourav Kumar](https://github.com/sourav-003)
- **LinkedIn**: [Sourav Kumar](https://www.linkedin.com/in/sourav-kumar-5814341b8)

---

⭐ *If you found this project helpful, don't forget to leave a ⭐ on the repository!*


