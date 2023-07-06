# credit-risk-classification

## Overview of the Analysis

In this challenge, the main goal of our analysis was to develop a machine learning model to accurately predict credit risk for loans. The data at hand comprised various financial information such as loan size, interest rate, borrower income, debt-to-income ratio, and other pertinent details about a borrower's financial status. The key prediction task was to classify each loan as '0' (healthy loan) or '1' (high-risk loan).

To approach this classification task, we implemented the logistic regression model. We also applied resampling methods to our training data to address the imbalance in our dataset, which primarily consisted of healthy loans ('0') with a smaller fraction of high-risk loans ('1').

The stages of the machine learning process we went through involved reading the data, preprocessing, splitting the data into training and testing sets, model fitting, making predictions, and evaluating model performance.

## Results

The following metrics were used to evaluate our models: balanced accuracy score, precision, and recall. These metrics provide a comprehensive view of the model's performance across both classes.

Machine Learning Model 1: Initial Logistic Regression Model

*Accuracy Score: 0.952
*Precision Score: For healthy loans, it was 1.00 and for high-risk loans, it was 0.85
*Recall Score: For healthy loans, it was 0.99 and for high-risk loans, it was 0.91
*Machine Learning Model 2: Logistic Regression with Resampled Training Data

*Accuracy Score: 0.994
*Precision Score: For healthy loans, it was 1.00 and for high-risk loans, it was 0.84
*Recall Score: For healthy loans, it was 0.99 and for high-risk loans, it was 0.99

## Summary

In terms of balanced accuracy, precision, and recall, the logistic regression model trained on resampled data (Model 2) outperformed the initial logistic regression model (Model 1). Particularly, Model 2 displayed superior recall for high-risk loans, which is crucial as it signifies the model's ability to correctly identify the riskier loans.

The decision on which model to use largely depends on the problem at hand. In this scenario, considering that the cost of misclassifying a high-risk loan as a healthy one could be substantial, it is crucial to use a model that minimizes such false negatives. Hence, Model 2, with its high recall score for high-risk loans, is the recommended model.

The success of these models lies in their ability to balance the act of minimizing false positives and negatives (high precision and recall scores), and accurately predicting the loan's risk status (high accuracy scores). In the context of credit risk, a machine learning model that performs well in these areas could be incredibly useful for companies when assessing the risk level of potential loans.
