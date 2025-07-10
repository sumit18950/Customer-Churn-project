# 📊 Customer Churn Prediction

This project aims to predict customer churn for a subscription-based telecommunications service using machine learning. By identifying customers likely to leave, the company can take targeted actions such as offering discounts or improving services to retain them.

---

## 🔍 Problem Statement

**Customer churn** is the phenomenon where a customer stops using a service. Reducing churn is vital for subscription-based businesses. Using historical data about customer behavior, service subscriptions, and account details, we aim to **build a predictive model** that flags customers at risk of leaving.

---

## 📁 Dataset

- **Source:** [Telco Customer Churn Dataset (Kaggle)](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Size:** 7,043 customer records
- **Target:** `Churn` (Yes/No)
- **Features:** Customer demographics, tenure, monthly charges, contract type, internet services, etc.

---

## 🧹 Workflow Summary

1. **Data Cleaning**
   - Removed customer ID
   - Converted `TotalCharges` to numeric
   - Handled missing values

2. **Feature Engineering**
   - Label encoded binary categorical variables
   - One-hot encoded multi-class categorical variables

3. **Modeling**
   - Split data into train/test sets
   - Scaled features using `StandardScaler`
   - Trained `RandomForestClassifier` model
   - Evaluated with Accuracy, ROC AUC, Confusion Matrix

4. **Evaluation**
   - Accuracy: **78.7%**
   - ROC AUC Score: **82%**
   - Churn Recall: **49%**

5. **Insights**
   - Customers with month-to-month contracts, high monthly charges, and no tech support/security are more likely to churn.

---

## 📈 Visuals

- ROC Curve
- Confusion Matrix
- Feature Importance Bar Chart
![image](https://github.com/user-attachments/assets/bb2eac96-2e18-4b7d-8c92-2ba766325af7)
![image](https://github.com/user-attachments/assets/ebf31a48-6472-423f-b8da-6337e72838fb)

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## ✅ Future Work

- Improve recall using SMOTE or resampling techniques
- Try other models: XGBoost, LightGBM
- Deploy using Streamlit or Flask
- Use SHAP for explainability

---

## 📂 Project Structure

