# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
    The purpose of this analysis is to use various techniques to train and evaluate a model based on loan risk.

* Explain what financial information the data was on, and what you needed to predict.
    The financial data being analyzed is a dataset of historical lending activity from a peer-to-peer leanding services company to which we are building a model that can identify the 
    creditworthiness of borrowers. The dataset contains features such as laon size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, and the loan status

lending_df.head()

* Stages of the Machine Learning Process:
1. Data Split:
    * the dataset was split into training and testing sets to evaluate each model's performance
    
2. Model Training:
    * the original dataset consists of 75036 data points classified as low risk and 3500 data points classified as high risk. The objective of each model is to predict the classification of laons given to borrowers in the testing sets.
    * the training data was used to fir the model to the data
    * Models used to test the original data:
        * Logistic Regression
        * Random Forest Classifier
        * K-Neighbors Classifier

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * For the healthy loans (0), the precision is 1.00, indicating that all of the predictions for this label were correct. The recall is also 1.00, meaning that all of this label were correctly identified.
    * The precision for the High-Risk Loan (1) is 0.95 which indicates that 95% of the predictions for this label were correct. The recall came back as 0.87 indicating 87% of this label were correctly identified.
    * the overall accuracy of the model is 0.99 which indicates that it has correctly identified the loan risk for 99% of the instances

* Machine Learning Model 2:
    * For the healthy loans (0), the precision is 1.00, indicating that all of the predictions for this label were correct. The recall is also 1.00, meaning that all of this label were correctly identified.
    * The precision for the High-Risk Loan (1) is 0.85 which indicates that 88% of the predictions for this label were correct. The recall came back as 0.88 indicating 88% of this label were correctly identified.
    * the overall accuracy of the model is 0.99 which indicates that it has correctly identified the loan risk for 99% of the instances

* Machine Learning Model 3:
    * For the healthy loans (0), the precision is 0.99, indicating that 99% of the predictions for this label were correct. The recall is also 1.00, meaning that all of this label were correctly identified.
    * The precision for the High-Risk Loan (1) is 0.93 which indicates that 93% of the predictions for this label were correct. The recall came back as 0.84 indicating 84% of this label were correctly identified.
    * the overall accuracy of the model is 0.99 which indicates that it has correctly identified the loan risk for 99% of the instances
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
Using the original data, Logistic Regression worked the best displaying higher correct predictions and recall out of the 3 models used.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Considering the objective of these models is to accurately identify healthy loans and high-risk loans, the logistic regression model using the original data stands to be the optimal choice. With this in mind, if a resampling of the original data was available, I believe that Logistic Regression would outperform the other models in identifying the objective.


