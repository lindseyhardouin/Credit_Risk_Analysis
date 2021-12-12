# Credit Risk Analysis Report

## Overview of the Analysis

This application prepares two logistic regression models for classifying credit worthiness, one using original data with a large class imbalance, and the second with the data resampled with the oversampling method. It then attempts to identify the better of model using evaluation tools including balanced accuracy scores, confussion matrices and classification reports.

The data includes a variety of information relative to the borrower's credit history and stats as well as information regardling the loan they're applying. Included are loan size they are applying for, interest rate, borrower income, debt to income ratio, number of open accounts, derogatory marks and total debt. These features are used to predict a borrower's loan status as being either healthy (0) or unhealthy (1).

The information detailed above should then be analyzed for class imbalances. As loan health is inherently imbalanced, the user can determine the extent using the value_counts function. Next, the user should prepare two logistic regression models using both the original and resampled data. Once the model, fit and predict steps have been performed on both sets, the user should use evalutation tools to determine the better model to classify each credit case. 


## Results

* Machine Learning Model 1, Original Data :
  * Balanced Accuracy Score : 0.95205
  * Precision (0) : 1.00
  * Precision (1) : 0.85
  * Recall (0) : 0.99
  * Recall (1) : 0.91

* Machine Learning Model 2, Resampled Data:
  * Balanced Accuracy Score : 0.99368
  * Precision (0) : 1.00
  * Precision (1) : 0.84
  * Recall (0) : 0.99
  * Recall (1) : 0.99


## Summary

Evaluation of the above scores, the resampled logistic regresional model (Model # 2) is a better fit. For a credit instituion, avoiding false positives, that is, approving a loan to an unhealthy financial applicant, is more important than avoiding false negatives, or rejecting a healthy financial applicant. The recall score in the resampled model shows a much better ability to do this. A credit instituion wants to minimize the number of defaulted loans as possible. Due to this inherent fact, the resampled loan model should be used. 