# 📉 Customer Churn Prediction – Telco Dataset

This project uses the **Telco Customer Churn dataset** to predict whether a customer will discontinue a telecom service using machine learning techniques.

---

## 🧠 Problem Statement

**Churn** refers to customers who stop using a company's service. Reducing churn is crucial for subscription-based businesses. In this project, we analyze the customer data and build ML models to predict churn.

---

## 📂 Dataset

- **Source:** [Telco Customer Churn Dataset – Kaggle](https://www.kaggle.com/datasets)
- **File:** `Telco_customer_churn.xlsx`
- **Sheet Used:** `Telco_Churn`
- **Features Include:**
  - Customer demographics
  - Service usage patterns
  - Contract and billing information
  - Churn label (`Churn Value`)

---

## 🛠️ Project Workflow

### 1. 📊 Exploratory Data Analysis (EDA)
- Summary statistics
- Null values & data types
- Churn distribution
- Correlation heatmaps

### 2. 🧹 Data Preprocessing
- Convert `Total Charges` to numeric
- Drop irrelevant columns (e.g., `CustomerID`, `Lat Long`)
- Encode categorical variables using Label Encoding
- Feature scaling using `StandardScaler`

### 3. 🤖 Model Building
- Train-test split (with `stratify` to avoid class imbalance)
- Trained models:
  - Logistic Regression
  - Random Forest Classifier

### 4. 📈 Model Evaluation
- Classification report
- Confusion matrix
- ROC-AUC curve

---

## 📌 Results

| Model               | Accuracy | AUC Score |
|--------------------|----------|-----------|
| Logistic Regression| ~0.80    | ~0.83     |
| Random Forest       | ~0.82    | ~0.87     |

Random Forest performed better in both classification and AUC metrics.

---

## 🔍 Key Insights

- Customers with **Month-to-Month** contracts churn the most.
- Customers who pay via **Electronic Check** are more likely to churn.
- **Tenure** and **Total Charges** negatively correlate with churn.
- Longer-tenured customers are less likely to leave.

---

## 🧠 Future Work

- Use advanced models like XGBoost or LightGBM
- Apply SMOTE to handle class imbalance
- Feature importance visualization using SHAP
- Web app deployment (e.g., Streamlit or Flask)

---

## 📒 Files Included

- `Customer_Churn_Prediction.ipynb` – Full Jupyter notebook
- `Telco_customer_churn.xlsx` – Dataset
- `README.md` – This project summary

---

## 🙌 Acknowledgements

Thanks to **IBM** and **Kaggle** for providing the dataset.

---

## 🔗 Connect with Me

If you like this project, feel free to ⭐ it and check out my other work on [GitHub](https://github.com/vaishnav-DA).

