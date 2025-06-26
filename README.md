# Telco Customer Churn - EDA Project

This repository contains an exploratory data analysis (EDA) of the Telco Customer Churn dataset. The objective is to understand customer behavior, identify patterns in churn, and explore features that influence customer retention.

---

## 📁 Dataset Overview
- **Source**: Telco Customer Churn dataset (Kaggle / IBM Sample Dataset)
- **Rows**: 7,043 customers
- **Columns**: 21 features
- **Target Column**: `Churn` (Yes/No)

Features include:
- Demographics: `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- Services signed up: `PhoneService`, `InternetService`, `StreamingTV`, etc.
- Account details: `tenure`, `Contract`, `PaperlessBilling`, `PaymentMethod`
- Charges: `MonthlyCharges`, `TotalCharges`

---

## 🧹 Data Cleaning
- Converted `TotalCharges` from object to numeric, handled invalid blanks using `errors='coerce'`
- Removed 11 rows with `NaN` in `TotalCharges`
- Reset dataframe index after dropping rows
- Encoded `Yes/No` columns (`Partner`, `Churn`, etc.) into `1/0`



### 1. Churn Distribution
- Visualized base churn rate
- About 26.5% of customers have churned

### 2. Gender-wise Churn
- Similar churn rates across male and female customers

### 3. Contract Type vs Churn
- Month-to-month contract users churn the most
- One/Two year contracts have much lower churn

### 4. Monthly Charges vs Churn
- Churned users tend to have higher monthly charges on average

### 5. Tenure vs Churn
- Newer customers (low tenure) are more likely to churn

### 6. Internet Service vs Churn
- Fiber optic users churn the most
- DSL users churn less, and 'No internet' users churn the least

### 7. Payment Method vs Churn
- Customers using electronic check methods have the highest churn rate

### 8. Correlation Heatmap
- `tenure` negatively correlated with `Churn`
- `MonthlyCharges` positively correlated
- `TotalCharges` shows weak negative correlation

---

## 📌 Key Insights
- Long-term contracts (1–2 years) significantly reduce churn
- Higher bills and shorter tenure increase churn likelihood
- Electronic checks and fiber optic users more prone to churn

---

## 🛠 Tools Used
- Python, Pandas, NumPy
- Seaborn, Matplotlib for visualization
- Jupyter Notebook for interactive EDA

---

## 📂 Folder Structure (if needed)
