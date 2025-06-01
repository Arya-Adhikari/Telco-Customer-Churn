# 📊 Customer Churn Prediction

This project aims to predict customer churn using the **Telco Customer Churn** dataset. It covers the full data science pipeline—from data exploration and cleaning to model training, evaluation, and interpretation.

---

## 🧠 Problem Statement

Telecommunication companies are often affected by customer churn. This project uses machine learning models to analyze customer behavior and predict which customers are likely to leave, allowing businesses to take proactive retention measures.

---

## 📁 Dataset

**Source:** IBM Sample Dataset  
**File:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`  
**Rows:** 7,043  
**Columns:** 21

Each row represents a customer with attributes such as:
- Demographics (Gender, Age group, etc.)
- Service usage (Phone, Internet, Streaming)
- Account info (Contract type, Monthly Charges, Tenure)
- Target variable: `Churn` (Yes/No)

---

## 📌 Key Features Created
- `TotalSpend` – MonthlyCharges × Tenure
- `CustomerTenureGroup` – Categorized tenure into `New`, `Early`, `Secure`, `Loyal`

---

## 📈 Exploratory Data Analysis

- Churn rates are highest among **month-to-month** contract customers.
- **Electronic check** payment method has the highest churn.
- **Senior citizens** and customers without dependents are more likely to churn.
- **Tenure** is one of the most important predictors.

Visualizations include:
- Bar plots
- Histograms
- Box plots
- Correlation heatmaps
- Pie charts

---

## 🤖 Models Used

| Model               | Accuracy | AUC-ROC Score |
|--------------------|----------|---------------|
| Logistic Regression| ✅       | ✅            |
| Decision Tree      | ✅       | ✅            |
| Random Forest      | ✅ Best  | ✅ Best       |

- **Random Forest** with GridSearchCV performed the best.
- Evaluation via **accuracy**, **confusion matrix**, **ROC curve**, and **classification report**.

---

## 🧪 Model Evaluation Metrics

- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix
- ROC Curve & AUC Score
- Feature Importance

---

## 🛠 Technologies Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib, Plotly
- Scikit-learn
- Joblib (for model serialization)

---

## 🧾 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/churn-prediction.git
   cd churn-prediction
