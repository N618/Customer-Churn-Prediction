# Customer-Churn-Prediction
End-to-end machine learning project for predicting telecom customer churn using Python, Scikit-learn
Customer Churn Prediction using Machine Learning

Python | Scikit-Learn | Pandas | NumPy | Matplotlib | XGBoost | Power BI

Overview

Customer churn is one of the biggest challenges faced by subscription-based businesses. Predicting customers who are likely to leave enables organizations to implement targeted retention strategies, reducing revenue loss and improving customer satisfaction.

This project develops an end-to-end Machine Learning pipeline to predict customer churn using the IBM Telco Customer Churn dataset. The project includes data preprocessing, exploratory data analysis, feature engineering, class imbalance handling, model development, hyperparameter tuning, model evaluation, and business insights visualization using Power BI.

Dashboard Preview

(Add your dashboard screenshot here)

Project Workflow
Data Collection
        │
        ▼
Data Cleaning
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Feature Engineering
        │
        ▼
SMOTE (Class Balancing)
        │
        ▼
Model Training
        │
        ▼
Hyperparameter Tuning
        │
        ▼
Model Evaluation
        │
        ▼
Business Insights Dashboard
Project Structure
├── data
│   ├── raw
│   └── processed
│
├── notebooks
│
├── src
│
├── models
│
├── dashboard
│
├── reports
│
├── images
│
├── presentation
│
├── requirements.txt
├── LICENSE
└── README.md
Dataset

The IBM Telco Customer Churn dataset contains customer demographics, service subscriptions, billing information, and churn status.

Features include
Customer Demographics
Internet Services
Phone Services
Contract Type
Payment Method
Monthly Charges
Total Charges
Tenure
Churn Status
Data Preprocessing

The following preprocessing techniques were applied:

Missing Value Treatment
Duplicate Removal
Label Encoding
One-Hot Encoding
Feature Scaling
Outlier Analysis
SMOTE for Class Imbalance
Exploratory Data Analysis

Key analyses performed:

Churn Distribution
Contract Type Analysis
Payment Method Analysis
Internet Service Analysis
Monthly Charges Distribution
Tenure Analysis
Correlation Heatmap
Machine Learning Models

Models evaluated:

Logistic Regression
Decision Tree
Random Forest
Gradient Boosting
XGBoost

Hyperparameter tuning performed using GridSearchCV.

Model Performance
Model	Accuracy	Precision	Recall	F1 Score
Logistic Regression	xx%	xx	xx	xx
Decision Tree	xx%	xx	xx	xx
Random Forest	82.03%	xx	0.85	xx
XGBoost	xx%	xx	xx	xx
Key Results
Achieved 82.03% Test Accuracy
Improved churn recall from 45% → 85% using SMOTE
Reduced false negatives significantly
Performed 20-Fold Cross Validation
Identified major churn drivers using Feature Importance
Business Insights

The analysis identified several key factors influencing customer churn:

Month-to-month contracts exhibit significantly higher churn rates.
Customers with Fiber Optic Internet services are more likely to churn.
Electronic Check payment method has the highest churn probability.
Higher monthly charges increase churn risk.
Longer-tenure customers are substantially less likely to churn.
Technologies Used
Python
Pandas
NumPy
Scikit-Learn
XGBoost
Imbalanced-Learn (SMOTE)
Matplotlib
Seaborn
Power BI
Jupyter Notebook
Future Improvements
Deploy model using Streamlit
Real-time churn prediction API
Explainability using SHAP
Automated retraining pipeline
Cloud deployment (Azure/AWS)
Author

Nitish Ranjan Jha

Senior Data Analyst

Python
SQL
Power BI
Machine Learning
Statistics
