# 📊 Customer Lifetime Value Prediction System using Machine Learning

> An end-to-end Machine Learning and Business Intelligence project that predicts **Customer Lifetime Value (CLV)**, segments customers based on predicted future value, and visualizes actionable business insights through an interactive **Power BI Dashboard**.
> # 📊 Customer Lifetime Value Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.11-blue)
![XGBoost](https://img.shields.io/badge/XGBoost-ML-success)
![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-yellow)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Overview

Customer Lifetime Value (CLV) is a key business metric used to estimate the total revenue a customer is expected to generate over their relationship with a business.

This project builds a complete **Customer Lifetime Value Prediction System** using historical retail transactions. The solution combines **feature engineering, machine learning, customer segmentation, and business intelligence** to help organizations identify valuable customers and support data-driven marketing strategies.

---

## 🚀 Key Features

* ✅ End-to-end Machine Learning pipeline
* ✅ Data cleaning and preprocessing
* ✅ Feature engineering using RFM, AOV, and Tenure
* ✅ Time-based train-test split to avoid data leakage
* ✅ Customer Lifetime Value prediction using XGBoost
* ✅ Feature importance analysis
* ✅ Customer segmentation into High, Medium, and Low Value groups
* ✅ Interactive Power BI dashboard
* ✅ Business recommendations based on predicted customer value

---

# 📷 Dashboard Preview


![Customer Lifetime Value Dashboard](Dashboard/Dashboard%20screenshot.png)

---

# 🛠️ Tech Stack

### Programming

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* XGBoost
* Joblib

### Business Intelligence

* Microsoft Power BI

### Development Environment

* Jupyter Notebook
* Anaconda

---

# 📂 Project Structure

```text
Customer_LTV_Project/
│
├── Dashboard/
│   ├── Customer_LTV_dashboard.pbix
│   └── Dashboard screenshot.png
│
├── data/
│   ├── Online Retail.xlsx
│   ├── cleaned_online_retail.csv
│   ├── customer_features.csv
│   ├── dashboard_dataset.csv
│   └── final_ml_dataset.csv
│
├── models/
│   ├── xgboost_ltv_model.pkl
│   └── feature_columns.pkl
│
├── notebooks/
│   └── Customer_LTV.ipynb
│
├── Outputs/
│   ├── plots/
│   └── predictions/
│
├── Project_report/
│   └── CLV_Project_Report.docx
│
├── README.md
├── requirements.txt
└── LICENSE
```

---

# 📁 Folder Description

### 📂 Dashboard

Contains the Power BI dashboard and dashboard screenshots used for business reporting.

---

### 📂 data

Contains the datasets used throughout the project.

* Raw Online Retail dataset
* Cleaned dataset
* Feature engineered dataset
* Dashboard-ready dataset

---

### 📂 models

Contains the trained XGBoost model and saved feature columns used for prediction.

---

### 📂 notebooks

Contains the complete Jupyter Notebook implementing the entire machine learning pipeline.

---

### 📂 Outputs

Contains generated prediction files and visualization images.

---

### 📂 Project_report

Contains the final project report documenting the methodology and implementation.

---

# 🔄 Project Workflow

## 1. Data Collection

* Imported the Online Retail transactional dataset.
* Explored data types, missing values, and overall structure.

---

## 2. Data Cleaning

* Removed missing Customer IDs.
* Removed cancelled transactions.
* Removed duplicate records.
* Created a Revenue feature.
* Saved the cleaned dataset for reproducibility.

---

## 3. Exploratory Data Analysis

Analyzed customer purchasing behaviour and transaction statistics to understand data quality and business patterns.

---

## 4. Feature Engineering

Created customer-level features including:

* Recency
* Frequency
* Monetary Value
* Average Order Value (AOV)
* Tenure

These features summarize customer purchasing behaviour and serve as model inputs.

---

## 5. Time-Based Train-Test Split

Instead of using a random split, historical transactions from the first **9 months** were used for training while the following **3 months** were used for prediction.

This approach simulates real-world forecasting and prevents data leakage.

---

## 6. Target Variable Creation

Future customer revenue was calculated from the prediction period to create the **Future Customer Lifetime Value** target variable.

A logarithmic transformation was applied to reduce skewness before model training.

---

## 7. Machine Learning

Two regression models were developed and evaluated:

* Random Forest Regressor
* XGBoost Regressor

Evaluation metrics:

* R² Score
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

XGBoost achieved the best performance and was selected as the final model.

---

## 8. Feature Importance

Model interpretation identified the strongest drivers of customer lifetime value:

1. Frequency
2. Monetary
3. Tenure
4. Recency
5. Average Order Value

These insights help businesses understand the characteristics of valuable customers.

---

## 9. Customer Segmentation

Customers were segmented into:

* 🟢 High Value
* 🟡 Medium Value
* 🔴 Low Value

based on predicted future lifetime value to support targeted marketing and retention strategies.

---

## 10. Power BI Dashboard

An executive dashboard was developed to visualize:

* Customer KPIs
* Customer Segmentation
* Revenue Contribution by Segment
* Customer Profile Matrix
* Feature Importance
* Model Performance
* Machine Learning Workflow
* Business Recommendations

---

# 📈 Key Results

| Metric                 | Result                       |
| ---------------------- | ---------------------------- |
| Customers Analysed     | **3,365**                    |
| Transactions Processed | **392K+**                    |
| Final Model            | **XGBoost Regressor**        |
| Customer Segments      | **High, Medium & Low Value** |
| Dashboard              | **Microsoft Power BI**       |

---

# 💼 Business Value

This solution enables businesses to:

* Predict future customer revenue.
* Identify high-value customers.
* Improve customer retention strategies.
* Optimize marketing campaigns.
* Allocate marketing budgets more effectively.
* Support data-driven decision-making through interactive dashboards.

---

# 🔮 Future Improvements

Potential enhancements include:

* Streamlit web application for real-time predictions
* Hyperparameter tuning using Optuna/GridSearchCV
* SHAP-based model explainability
* Cloud deployment using Azure or AWS
* REST API deployment using FastAPI

---

# 📚 Learning Outcomes

This project strengthened practical skills in:

* Data Cleaning
* Feature Engineering
* Predictive Machine Learning
* Model Evaluation
* Customer Analytics
* Power BI Dashboard Development
* Business Intelligence
* Git & GitHub

---

# 👤 Author

**Dhruva Vermani**

Aspiring Data Scientist | Machine Learning | Data Analytics

If you found this project interesting, feel free to connect or explore the repository.
