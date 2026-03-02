# 🍽️ Task 3 – Cuisine Classification

## 📌 Objective
The goal of this task is to build a Machine Learning classification model that predicts the primary cuisine of a restaurant based on available features.

---

## 📊 Dataset Overview
The dataset contains information about restaurants including:

- Restaurant details
- Location information
- Price range
- Votes
- Aggregate ratings
- Cuisine types

Since many restaurants have multiple cuisines listed, only the **first cuisine** was considered for simplification.

---

## 🔍 Exploratory Data Analysis (EDA)

- Analyzed distribution of cuisine categories
- Identified class imbalance in dataset
- Selected top 10 most frequent cuisines to reduce noise
- Visualized cuisine frequency using bar plots

---

## 🧹 Data Preprocessing

- Removed missing values
- Simplified multi-label cuisine column (selected first cuisine)
- Filtered top 10 cuisines
- Dropped irrelevant columns:
  - Restaurant ID
  - Restaurant Name
  - Address
  - Locality
  - Currency
- Applied One-Hot Encoding to categorical features
- Encoded target variable using LabelEncoder
- Performed Train-Test Split (80-20)

---

## 🤖 Model Selection

The following models were tested:

- Random Forest Classifier
- Gradient Boosting Classifier

Final selected model:
> **Gradient Boosting Classifier**

---

## 📈 Model Performance

- Accuracy: ~44%
- Evaluation Metrics:
  - Precision
  - Recall
  - F1-score

Due to class imbalance and overlapping features between cuisines, extremely high accuracy is not expected for this multi-class classification task.

---

## ⚠️ Challenges

- Class imbalance (some cuisines dominate dataset)
- Overlapping feature patterns between cuisines
- Limited strong predictive features for cuisine differentiation

---

## 💾 Model Saving

The following components were saved using `joblib`:

- Trained Gradient Boosting model (`cuisine_gb_model.pkl`)
- Label Encoder (`cuisine_label_encoder.pkl`)
- Feature columns (`cuisine_columns.pkl`)

This ensures reproducibility and future predictions without retraining.

---

## 🧠 Key Learnings

- Handling multi-class classification problems
- Managing class imbalance
- Importance of feature engineering
- Using ensemble models for improved performance
- Model persistence using joblib

---

## 🚀 Conclusion

Cuisine classification is a complex multi-class problem. Despite dataset limitations, a robust machine learning pipeline was developed, achieving reasonable accuracy and demonstrating proper ML workflow including preprocessing, model training, evaluation, and deployment readiness.
