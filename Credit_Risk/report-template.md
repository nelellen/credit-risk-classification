# Module 12 Report Template

## Overview of the Analysis

In this analysis, the goal was to build and evaluate a machine learning model to predict the risk level of loans. The model classifies loans as either **healthy (0)** or **high-risk (1)** based on various financial features, such as loan size, interest rate, borrower income, debt-to-income ratio, and the number of derogatory marks. By automating the loan classification process, the company can make more informed and efficient decisions regarding loan approvals or rejections.

### Machine Learning Model Used: Logistic Regression

For this task, we used  **Logistic Regression** , a widely used algorithm for binary classification problems. Logistic Regression estimates the probability of a loan being high-risk based on the input features and outputs a classification of either `0` (healthy loan) or `1` (high-risk loan).

## Results

The model was trained and evaluated on the dataset, with the following performance metrics:

* **Accuracy Score** : 85.6%
  The model correctly predicted the risk level of 85.6% of the loans in the test set.
* **Precision Score for Class 0 (Healthy Loan)** : 88.4%
  Precision for the healthy loan class is high, meaning most of the predicted healthy loans are indeed healthy.
* **Precision Score for Class 1 (High-Risk Loan)** : 77.2%
  The precision for high-risk loans is lower, indicating that some healthy loans were incorrectly predicted as high-risk.
* **Recall Score for Class 0 (Healthy Loan)** : 84.5%
  The model successfully identified 84.5% of all actual healthy loans, but there is still room for improvement in reducing false negatives.
* **Recall Score for Class 1 (High-Risk Loan)** : 72.1%
  Recall for high-risk loans is relatively lower, suggesting that the model misses some high-risk loans, potentially due to class imbalance.

## Summary

The logistic regression model performed well overall, with an accuracy of 85.6%. While precision for predicting healthy loans (`0`) was high, precision for high-risk loans (`1`) was lower, indicating some misclassification of healthy loans as risky. The recall for high-risk loans was also not as strong, suggesting that the model could miss some high-risk loans.

### Recommendation:

* **Recommend Use with Improvements** : The model's overall accuracy and precision for healthy loans make it a good starting point for loan risk prediction. However, improvements are needed, especially in predicting high-risk loans (`1`). Techniques such as handling class imbalance (e.g., SMOTE) or exploring alternative algorithms (like Random Forest or XGBoost) could further enhance the model's ability to identify high-risk loans.
* **If Not Recommended** : If the company is prioritizing the accurate detection of high-risk loans, I would recommend exploring other models or improving the current model through tuning and balancing techniques to boost recall for the `1` class.
