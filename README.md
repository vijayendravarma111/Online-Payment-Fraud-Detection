# Online Payment Fraud Detection using Machine Learning

## Project Overview
This project focuses on detecting fraudulent online payment transactions using Machine Learning techniques. 
The system analyzes transaction details such as transaction type, amount, and account balance changes to 
classify transactions as **Fraudulent** or **Legitimate**.

The project follows an end-to-end Machine Learning pipeline including data analysis, preprocessing, 
model training, evaluation, and final model selection.

---

## Problem Statement
Online payment systems are vulnerable to fraudulent activities. Detecting fraud accurately while minimizing 
false alarms is a critical challenge due to highly imbalanced transaction data.

---

## Dataset
- Source: Kaggle – Online Payment Fraud Detection Dataset
- File: `onlinefraud.csv`
- Description: Simulated transaction data with fraud labels
- Note: Dataset is not uploaded due to size constraints.

---

## Exploratory Data Analysis (EDA)
- Analyzed fraud vs non-fraud distribution
- Studied fraud patterns across transaction types
- Identified high-risk transaction categories (TRANSFER, CASH_OUT)
- Visualized amount and balance inconsistencies

---

## Data Preprocessing
- Removed non-informative identifier columns
- Encoded categorical transaction types
- Handled missing values
- Applied stratified train-test split
- Addressed class imbalance

---

## Models Trained
| Model | Purpose |
|-----|--------|
| Logistic Regression | Baseline model |
| Random Forest | Non-linear fraud detection |
| XGBoost | Final optimized model |

---

## Final Model
**XGBoost Classifier**
- Best performance on imbalanced data
- Improved fraud recall and F1-score
- Achieved ~99.9% validation accuracy

---

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Fraud detection performance was evaluated with emphasis on **recall**, as missing frauds is costlier than false alarms.

---

## Model Saving
The final trained model is saved as: model/fraud_detection_xgboost.pkl

---

## Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Google Colab

---



---

## Conclusion
The project demonstrates how Machine Learning can effectively identify fraudulent online transactions 
by learning transaction behavior patterns. XGBoost proved to be the most effective model for this task.

---

## Future Enhancements
- Deploy model using Flask or Streamlit
- Real-time fraud detection API
- Threshold tuning for recall optimization

