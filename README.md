# Customer Churn Prediction using k-Nearest Neighbours

## Overview
This project develops a machine learning model to predict telecom customer churn. A k-nearest neighbours (kNN) classifier is used to estimate the probability that a customer will leave. Because churn datasets are typically imbalanced, model performance is evaluated using ROC curves and Area Under the Curve (AUC) rather than accuracy alone. The analysis also explores how different classification thresholds affect the ability to identify high-risk customers.

---

## Business Problem
Customer churn is costly because acquiring new customers is often more expensive than retaining existing ones. By identifying customers who are likely to churn before they leave, companies can target retention strategies such as promotions, service upgrades, or personalized offers.

---

## Dataset
Telco Customer Churn dataset  
File: `WA_Fn-UseC_-Telco-Customer-Churn.csv`

Each observation represents a telecom customer. The dataset includes information on service usage, account characteristics (e.g., tenure, contract type, billing method), and demographic attributes. These variables are used to predict whether a customer will churn.

---

## Methods
- k-Nearest Neighbours (kNN) classification model  
- Standardization of numeric predictors  
- Bootstrap validation for tuning model parameters  
- Model evaluation using ROC curves and Area Under the Curve (AUC)  
- Threshold optimization using the Youden index  

---

## Key Results
- Model AUC: **0.818**
- The kNN model performed better than a naïve classifier that predicts the majority class.
- Accuracy alone was misleading due to class imbalance.
- Adjusting the classification threshold improved the model’s ability to identify likely churners.

---

## Tools Used
- R  
- caret  
- ROCR  
- Quarto  

---

## Key Takeaway
This analysis demonstrates that model evaluation choices matter in churn prediction. Accuracy alone can be misleading when datasets are imbalanced, while ROC/AUC and threshold analysis provide more useful insight for decision-making in customer retention strategies.

---
data not included due to licensing
