# Credit Risk Analysis Report

## Overview
The purpose of this analysis is to predict the risk level of loans using financial data. Specifically, we aim to classify loans as either healthy (0) or high-risk (1) using a logistic regression model.

## Results
- Summary of Results
- The logistic regression model achieved a **balanced accuracy score** of approximately **95.2%**. 

- The confusion matrix showed that the model correctly predicted the majority of healthy loans and high-risk loans.
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


The logistic regression model demonstrates excellent performance in predicting loan risk, with high accuracy and strong classification metrics. Thus, I highly recommend using this model to help in financial decision-making processes.
