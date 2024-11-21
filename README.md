# credit-risk-classification

Loan Risk Analysis Report

Overview of the Analysis

The purpose of this analysis was to develop and evaluate a machine learning model capable of predicting the risk level of loans based on financial data. This analysis aimed to assist financial institutions in identifying high-risk loans, enabling better decision-making and risk management.

The dataset included information on loan statuses and financial features. The target variable, loan_status, was binary, with 0 indicating healthy loans and 1 indicating high-risk loans. 

The machine learning process involved the following steps:

Data preprocessing and splitting into training and testing sets.
Building a logistic regression model to classify loans.
Evaluating the model's performance using metrics such as accuracy, precision, recall, and confusion matrices.
Results

Logistic Regression Model Performance:
Accuracy Score: 96.8%
Precision:
Class 0 (Healthy Loan): 96.8%
Class 1 (High-Risk Loan): 0%
Recall:
Class 0 (Healthy Loan): 100%
Class 1 (High-Risk Loan): 0%

Confusion Matrix:
18765,     0 
619,     0

Summary

The logistic regression model achieves high overall accuracy (96.8%) by correctly classifying healthy loans (class 0). However, it completely fails to identify high-risk loans (class 1). This is evident from:

A recall of 0 for high-risk loans, meaning no high-risk loans were correctly identified.
A precision of 0 for high-risk loans, meaning the model never predicted any loans as high-risk.
The primary issue stems from the class imbalance in the dataset, where healthy loans heavily outweigh high-risk loans. The model prioritizes the majority class, leading to poor performance in detecting high-risk loans.

Recommendation:
This model is not recommended for identifying high-risk loans, as it fails to predict the minority class (1).
To improve performance:
Address the class imbalance using techniques such as oversampling or undersampling.
Use a model that handles class imbalance better, such as Random Forest or Gradient Boosting with class weights.
By addressing the class imbalance and fine-tuning the model, the institution can develop a more effective tool for identifying high-risk loans.
