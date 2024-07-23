# Credit Risk Analysis Report

## Overview
The purpose of this analysis is to predict the risk level of loans using financial data. Specifically, we aim to classify loans as either healthy (0) or high-risk (1) using a logistic regression model.

## Summary of Results
- The logistic regression model achieved a **balanced accuracy score** of approximately **95.2%**. 

The confusion matrix shows that the model has low rates of misclassification, ensuring reliable predictions.
**Confusion Matrix:**
[[18663   102]
 [   56   563]]


- The classification report indicated high precision, recall, and F1-scores for both classes, with particularly strong performance for the healthy loan class.
 Classification Report:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

As is clear above, the model is very strong in predicting healthy loans (Class 0) with a precision 100% and recall of 0.99. For high-risk loans (Class 1), the model also performs well with a precision of 0.85 and a recall of 0.91.

A recall of 0.91 means the model correctly identifies 91% of high-risk loans, which is significant for risk management.
The logistic regression model demonstrates excellent performance in predicting loan risk, with high accuracy and strong classification metrics. Therefore, the model is well-suited for the task and should be used by the company to assess loan risk.
