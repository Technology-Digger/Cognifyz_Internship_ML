# ⭐ Task 1 – Predict Restaurant Ratings

## 📌 Objective
The goal of this task is to build a Machine Learning regression model to predict the aggregate rating of a restaurant based on various features such as votes, price range, and other attributes.

---

## 📊 Dataset Overview
The dataset contains detailed information about restaurants, including:

- Restaurant details
- Location (City, Country)
- Price range
- Votes
- Online delivery availability
- Aggregate rating (Target variable)

---

## 🔍 Exploratory Data Analysis (EDA)

- Analyzed distribution of restaurant ratings
- Observed large number of **0 ratings (unrated restaurants)**
- Identified that most ratings lie between **2.5 – 4.5**
- Explored relationships between features using:
  - Histograms
  - Boxplots
  - Correlation heatmap

---

## 📈 Key Insights

- **Votes** and **Price Range** show the strongest correlation with ratings (~0.4)
- Higher customer engagement (votes) → higher ratings
- Premium restaurants tend to have slightly better ratings
- Location features (latitude, longitude) have minimal impact
- Some features like Restaurant ID and Country Code are not useful for prediction

---

## 🧹 Data Preprocessing

- Removed restaurants with **0 ratings** (treated as noise)
- Handled missing values
- Dropped irrelevant columns:
  - Restaurant ID
  - Country Code
  - Latitude & Longitude
- Converted categorical variables using One-Hot Encoding
- Split data into training and testing sets (80-20)

---

## 🤖 Model Selection

Models used:

- Linear Regression ✅
- Decision Tree Regressor

Final selected model:
> **Linear Regression** (best performance)

---

## 📊 Model Performance

- **R² Score:** ~0.83  
- **Mean Squared Error (MSE):** Low  

👉 Interpretation:
- The model explains approximately **83% of the variance** in restaurant ratings
- Indicates strong predictive performance

---

## 🔥 Feature Importance

Top influencing features:

- Votes
- Price Range

These features significantly impact restaurant ratings.

---

## 💾 Model Saving

The trained model was saved using `joblib`:

- Model file: `restaurant_rating_model.pkl`
- Feature columns: `model_columns.pkl`

This allows reuse of the model without retraining.

---

## 🧠 Key Learnings

- Understanding regression problems
- Importance of EDA before modeling
- Feature selection improves model performance
- Avoiding data leakage during preprocessing
- Evaluating models using R² and MSE

---

## 🚀 Conclusion

A robust regression model was built to predict restaurant ratings with high accuracy. The project demonstrates a complete machine learning workflow including data cleaning, feature engineering, model training, evaluation, and deployment readiness.
