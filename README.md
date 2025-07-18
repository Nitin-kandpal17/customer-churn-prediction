# 📉 Customer Churn Prediction 

This project focuses on predicting customer churn in the telecom industry using machine learning. The goal is to identify customers who are likely to leave the service and suggest data-driven retention strategies.

---

## 🧠 Problem Statement

Customer churn is a significant issue for service-based businesses. By analyzing historical customer behavior and service data, we aim to build a predictive model that flags potential churners.

---

## 📊 Dataset

- **Source**: IBM Telco Customer Churn Dataset (Kaggle)
- **Records**: 7043
- **Target**: `Churn` (Yes/No)
- **Features**: Customer demographics, services used, contract type, payment method, tenure, etc.

---

## 🔍 Project Phases

### 📅 Day 1: Exploratory Data Analysis
- Analyzed churn trends by contract type, tenure, and payment method.
- Extracted key patterns influencing churn.

### ⚖️ Day 2: Preprocessing + SMOTE
- Handled missing values and categorical variables.
- Applied **Stratified Train-Test Split**.
- Used **SMOTE** to balance the classes.

### 🧪 Day 3: Model Building
- Trained and evaluated models using:
  - ✅ Random Forest
  - ✅ XGBoost
- Focused on improving **F1-score** using class balancing.

### 🧠 Day 4: Hyperparameter Tuning + Strategy
- Tuned Random Forest & XGBoost with `GridSearchCV`.
- Evaluated both models using:
  - Confusion Matrix
  - Classification Report
- Identified top churn indicators.
- Suggested data-backed retention strategies.

---

## 🧰 Techniques Used

- SMOTE (Synthetic Minority Over-sampling)
- GridSearchCV
- XGBoost & Random Forest
- Confusion Matrix & Classification Report
- Feature Importance Analysis

---

## 📌 Retention Strategy Insights

Based on feature importance from Random Forest and XGBoost:
- Customers with **month-to-month contracts** are highly likely to churn.
- Users opting for **electronic check payments** have higher churn rates.
- Customers with **lower tenure** or **fiber optic internet** are more prone to leave.
- Strategic recommendations:
  - Incentivize long-term contracts.
  - Offer discounts or personalized plans to at-risk groups.

---

## 💾 Artifacts

| File/Folder         | Description                              |
|---------------------|------------------------------------------|
| `data/`             | Processed datasets (train/test/SMOTE)    |
| `models/`           | Saved models (`.pkl` files)              |
| `outputs/`          | Classification reports, plots, etc.      |
| `notebooks/`        | Jupyter notebooks (Day-wise)             |

---

## 🚀 Future Scope (Optional)

- Deploy model with Streamlit for real-time predictions.
- Add LIME/SHAP for model interpretability.

---

## 📁 Directory Structure
## Project Directory Structure

```
├── data/
│   ├── WA_Fn-UseC_-Telco-Customer-Churn.csv
│   ├── X_test.csv
│   ├── X_train_sm.csv
│   ├── y_test.csv
│   └── y_train_sm.csv
├── models/
│   ├── random_forest_best.pkl
│   ├── xgb_churn_model.pkl
│   └── xgboost_best.pkl
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_model_training.ipynb
│   └── 04_model_tuning.ipynb
├── outputs/
│   ├── classification_report_rf.txt
│   ├── classification_report_xgb.txt
│   └── classification_report.txt
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```


---

## 👤 Author

- **Nitin Kandpal**
- Aspiring Data Scientist
- GitHub: [Nitin-Kandpal](https://github.com/Nitin-kandpal17)

---


