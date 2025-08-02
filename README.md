# 🏥 Healthcare Premium Prediction

This project predicts individual **health insurance premiums** using demographic and health-related data. By applying machine learning regression techniques with hyperparameter tuning and model interpretability, it delivers accurate and explainable predictions to support pricing strategies for insurers.

---

## 📌 Problem Statement

Healthcare premiums depend on multiple factors like age, smoking status, BMI, and more. The goal is to build a predictive regression model that estimates a person’s health insurance cost based on their profile.

---

## 🔧 Tools & Technologies

- **Python**
- **Pandas, NumPy** – Data manipulation
- **Matplotlib, Seaborn** – Data visualization
- **Scikit-learn** – ML modeling, encoding, evaluation
- **XGBoost / Random Forest** – Advanced regressors
- **SHAP** – Model interpretability
- **Streamlit** *(optional)* – Dashboard for user interaction

---

## 📊 Exploratory Data Analysis (EDA)

- Distribution of `charges`, `age`, and `BMI`
- Smoking status impact on premium
- Interaction between `smoker`, `age`, and `charges`
- Detection of outliers and skewness
- Pairplots and correlation heatmaps

---

## 🧼 Data Preprocessing

### 🔠 Feature Encoding
- Applied **Label Encoding** for binary features like `sex`, `smoker`
- Used **One-Hot Encoding** for multi-category feature `region`
  
### 🔍 Feature Scaling
- Standardized continuous variables like `age` and `BMI` where needed

---

## ⚙️ Modeling Approach

- Data split into train and test sets (80-20)
- Models Trained:
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - XGBoost Regressor

---

## 🔧 Hyperparameter Tuning

Used **GridSearchCV** and **RandomizedSearchCV** to optimize models:

- **Random Forest:** Tuned `n_estimators`, `max_depth`, `min_samples_split`
- **XGBoost:** Tuned `learning_rate`, `n_estimators`, `max_depth`, `subsample`

Resulted in significant performance gains with minimal overfitting.

---

## 📈 Model Performance

| Model                   | R² Score | RMSE   |
|------------------------|----------|--------|
| Linear Regression       | 0.76     | ~6000  |
| Random Forest (Tuned)   | 0.89     | ~4200  |
| XGBoost (Tuned)         | 0.91     | ~3900  |

---


