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
