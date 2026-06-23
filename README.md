# IBM Customer Churn Prediction

<p align="left">

<img src="https://img.shields.io/badge/PYTHON-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/PANDAS-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/NUMPY-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
<img src="https://img.shields.io/badge/SCIKIT--LEARN-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/XGBOOST-EC6B23?style=for-the-badge"/>
<img src="https://img.shields.io/badge/SMOTE-4CAF50?style=for-the-badge"/>
<img src="https://img.shields.io/badge/MATPLOTLIB-11557C?style=for-the-badge"/>
<img src="https://img.shields.io/badge/SEABORN-4C72B0?style=for-the-badge"/>
<img src="https://img.shields.io/badge/JUPYTER-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>

</p>

## Overview

Customer churn is one of the biggest challenges for subscription-based businesses.  
This project analyzes the IBM Telco Customer Churn dataset to identify the major factors influencing churn and builds machine learning models to predict whether a customer is likely to leave.

The goal is to support proactive retention strategies by identifying high-risk customers early.

---

## Objective

- Analyze customer behavior and service usage patterns
- Identify the key drivers of churn
- Build predictive machine learning models for churn classification
- Handle class imbalance using SMOTE
- Compare multiple models using accuracy, precision, recall, F1-score, and ROC-AUC
- Select the best-performing model for churn prediction

---

## Dataset

This project uses the **IBM Telco Customer Churn** dataset.

It includes customer-level information such as:

- Gender
- Senior citizen flag
- Partner and dependents
- Tenure
- Phone service
- Internet service
- Contract type
- Payment method
- Monthly charges
- Total charges
- Churn status

---

## Project Structure

```text
IBM-Customer-Churn-Prediction
│
├── README.md
├── LICENSE
├── requirements.txt
├── .gitignore
│
├── data
│   ├── raw
│   │   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│   └── processed
│       └── cleaned_churn_data.csv
│
├── notebooks
│   └── IBM Customer Churn Analyssi(2).ipynb
│
├── src
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── model_training.py
│   ├── model_evaluation.py
│   └── utils.py
│
├── models
│   └── best_model.pkl
│
├── reports
│   ├── churn_analysis_report.pdf
│   └── model_performance_summary.pdf
│
└── images
    ├── churn_distribution.png
    ├── correlation_heatmap.png
    ├── roc_curve.png
    └── feature_importance.png






Data Preparation

The notebook includes the following preprocessing steps:

Checked data shape, column types, missing values, and duplicates
Converted TotalCharges from object to numeric
Handled blank values in TotalCharges as missing values
Removed rows with missing TotalCharges
Dropped customerID because it is only an identifier
Encoded categorical variables
Standardized numeric features using StandardScaler
Exploratory Data Analysis

The analysis explores:

Churn vs non-churn distribution
Tenure, MonthlyCharges, and TotalCharges patterns
Relationships between categorical variables and churn
Customer segment behavior
Class imbalance in the target variable
Feature Engineering

The modeling pipeline includes:

Train-test split
Label encoding
Feature scaling
Balancing the target classes using SMOTE
Preparing the data for classification models
Machine Learning Models Used

The following models were trained and compared:

Logistic Regression
Decision Tree
Random Forest
Gradient Boosting
XGBoost

Hyperparameter tuning was performed using GridSearchCV.

Model Evaluation

The models were evaluated using:

Accuracy
Confusion Matrix
Classification Report
Precision
Recall
F1 Score
ROC-AUC Curve

Since churn prediction is an imbalanced classification problem, recall and F1-score were treated as more important than accuracy alone.

Best Model

Based on the notebook results, Gradient Boosting performed best among the tested models.

Key Business Insights
Customers with month-to-month contracts show the highest churn rate
Customers with shorter tenure are more likely to churn
Higher monthly charges are associated with increased churn
Customers using electronic check tend to churn more often
Long-term contracts improve customer retention
Workflow
Data Collection
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Feature Encoding
      ↓
Feature Scaling
      ↓
Train-Test Split
      ↓
SMOTE Balancing
      ↓
Model Training
      ↓
Hyperparameter Tuning
      ↓
Model Evaluation
      ↓
Business Insight Extraction
Technologies Used
Python
Pandas
NumPy
Scikit-Learn
XGBoost
Imbalanced-Learn
Matplotlib
Seaborn
Jupyter Notebook
How to Run the Project
git clone https://github.com/your-username/IBM-Customer-Churn-Prediction.git
cd IBM-Customer-Churn-Prediction
pip install -r requirements.txt
jupyter notebook

Open the notebook and run all cells step by step.

Conclusion

This project demonstrates a complete churn prediction workflow, from raw data cleaning to model building and evaluation.
It highlights the most important churn drivers and supports data-driven customer retention strategies.

Author

Nitish Jha
Data Analyst | Python | SQL | Power BI | Machine Learning

