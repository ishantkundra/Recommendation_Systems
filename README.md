# 🤖 Recommendation Systems Project – Popularity & Collaborative Filtering Models

## 📌 Project Overview

This project explores two widely used recommendation system techniques — **popularity-based** and **collaborative filtering** — to suggest mobile phones to users based on behavior and ratings data. The analysis is grounded in real-world smartphone reviews collected from multiple sources.

---

## 📱 Domain: Smartphones & Electronics

India’s smartphone market, driven by high user engagement and rising demand, presents a massive opportunity for personalized recommendation systems. This project simulates such a system using historical product ratings.

---

## 🎯 Project Objective

To build a recommendation system using:
- **Popularity-Based Model**: Recommends top-rated phones to all users
- **Collaborative Filtering** (SVD, kNNWithMeans): Suggests personalized recommendations based on user-item interactions

---

## 📊 Dataset Description

The dataset (from multiple CSVs) includes:
- `author`: reviewer
- `product`: mobile phone model
- `score`: average rating
- `domain`: source website
- `language`, `country`, `extract`, etc.

Final dataset used: **1 million rows**, filtered and cleaned.

---

## 🛠️ Key Steps

### ✅ Data Preprocessing
- Merged multiple CSV files
- Removed duplicates and irrelevant features
- Imputed missing values and cleaned noisy fields
- Retained only top features: `author`, `product`, and `score`
- Filtered to 1M random samples using `random_state=612`

### 📈 EDA & Insights
- Identified most-reviewed products and authors
- Filtered data to users/products with >50 reviews

### ⭐ Popularity-Based Recommender
- Recommended top 5 globally best-rated phones

### 👥 Collaborative Filtering (Personalized Recommender)
- **SVD-based model** using Surprise library
- **kNNWithMeans model** (both item-based and user-based)
- Trained, validated, and compared models
- RMSE used for model evaluation
- Top 5 product recommendations for selected test users

### 🔍 Business Use-Cases
- Popularity model for new users (cold start)
- CF model for returning users (personalized feed)

---

## ⚙️ Tools, Libraries & Skills Used

- **Languages:** Python
- **Libraries:** Pandas, NumPy, Surprise, Matplotlib, Seaborn
- **Skills:**
  - Recommender Systems
  - Collaborative Filtering
  - Popularity-Based Recommendation
  - kNNWithMeans (user/item-based)
  - SVD (Matrix Factorization)
  - Evaluation using RMSE
  - Python Data Analysis

---

## 📁 Repository Structure

<pre>

.
├── code/
│   └── RS/
│       ├── Recommendation Systems_01IK.ipynb      # Main project notebook
│       └── Recommendation Systems_01IK.html       # HTML export of notebook
│
├── dataset/
│   └── Data Set.zip                               # Source data (multiple CSVs)
│
├── Problem Statement/
│   └── RS - Problem_Statement.pdf                 # Detailed project brief
│
├── .gitignore
└── README.md                                      # This file

</pre>

---

## 💡 Key Learnings

- Built and compared personalized vs. non-personalized recommendation models  
- Understood limitations of collaborative filtering (cold start, sparsity)  
- Applied industry techniques to build scalable and testable recommender systems  
- Used Surprise library for modeling and evaluation (SVD, kNNWithMeans)

---

## ✍️ Author

**Ishant Kundra**  
📧 [ishantkundra9@gmail.com](mailto:ishantkundra9@gmail.com)  
🎓 Master’s in Computer Science | AIML Track
