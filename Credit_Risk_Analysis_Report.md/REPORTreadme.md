# Credit Risk Analysis Report

## Overview

## Purpose of the Analysis
The purpose of this analysis is to predict the risk level of loans using financial data. Specifically, the goal is to classify loans as either 0 (healthy loan) or 1 (high-risk loan) using a logistic regression model.

## Financial Information in the Data
The dataset lending_data.csv contains the following financial information:

1. loan_size: The size of the loan.
2. interest_rate: The interest rate of the loan.
3. borrower_income: The income of the borrower.
4. debt_to_income: The debt-to-income ratio of the borrower.
5. num_of_accounts: The number of accounts the borrower has.
6. derogatory_marks: The number of derogatory marks on the borrower’s credit    report.
7. total_debt: The total debt of the borrower.
8. loan_status: The status of the loan (0 for healthy loan and 1 for high-risk loan).

## Variables to Predict
The target variable to predict is loan_status. Here are the basic counts of the loan_status variable:

0 (healthy loan): A large majority.
1 (high-risk loan): A small minority.

## Stages of the Machine Learning Process

### Data Loading and Preparation:
The data is read from a CSV file into a Pandas DataFrame.
Initial exploration and inspection of the data to understand its structure and contents.

### Data Splitting:
The data is split into training and testing sets to evaluate the model's performance on unseen data.

### Model Training:
A logistic regression model (LogisticRegression) is chosen for the classification task.
The model is trained using the training data.

### Model Prediction:
The trained model is used to make predictions on the testing data.

### Model Evaluation:
1. The balanced accuracy score of the model is calculated to assess its performance.
2. A confusion matrix is generated to understand the distribution of predictions.
3. A classification report is printed to provide precision, recall, and F1-score metrics for both classes (0 and 1).

### Methods Used
The primary method used in this analysis is Logistic Regression. This algorithm is suitable for binary classification tasks and provides probabilities for the classes, allowing for a straightforward interpretation of the results.

## Summary of Results
The logistic regression model achieved a balanced accuracy score of approximately 95.2%.

The confusion matrix showed that the model correctly predicted the majority of healthy loans and high-risk loans.
**Confusion Matrix:**
[[18663   102]
 [   56   563]]

The classification report indicated high precision, recall, and F1-scores for both classes, with particularly strong performance for the healthy loan class.
Classification Report:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

### Conclusion

A recall of 0.91 means the model correctly identifies 91% of high-risk loans, which is significant for risk management.
The logistic regression model demonstrates excellent performance in predicting loan risk, with high accuracy and strong classification metrics. Therefore, the model is well-suited for the task and should be used by the company to assess loan risk.


