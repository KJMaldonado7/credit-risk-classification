# Credit Risk Classification Module 20 Report


## Overview of the Analysis

The purpose of the analysis was to create a logistic regression model that could predict whether a loan was a "Healthy" or a "High Risk" loan. The financial data used to create the logistic model was contained in the "lending_data.csv" file found in the Resources folder. The data included information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts held, number of derogatory marks, and total debt. 

Based on this data, we wanted to predict the loan's status. 

To conduct the analysis, the necessary libraries were imported into a Jupyter Notebook. Then, the data in the "lending_data.csv" file was read into a Pandas dataframe. 

After reviewing the newly created dataframe (df_lending_data), the data was separated into labels and features. The labels used in this analysis was 0 (or a "Healthy" loan) and 1 (or a "High-Risk" loan). The data was then split into training and testing datasets by using train_test_split. The random_state of 1 was used. 

From here, a logistic regression model was created and fit to the training data. Then, the model could be used to make predictions. 


## Results

* Balanced Accuracy Score
  * 0.9520479254722232 or 95.2%
  * A perfect score, or a 1 (100%) would indicate that the model perfectly predicts both 
    labels. A score of 95.2% suggests that the model performs very well at predicting both 
    Healthy loans and high risk loans

* Confusion Matrix
  * High Accuracy
     * 18663 loans were accurately classified as healthy Loans, whereas only 102 were 
       inaccurately classified as high-risk loans
     * 563 loans were accurately classified as high risk loans, and 56 were inaccurately 
       classified as health loans
       
* Classification Report
  *  In the classification report, we see that the model had a high accuracy, recall, and f1 
     score. 

## Summary

Overall, the logistics regression model performs very well as it has an accuracy of 99% in predicting healthy and high risk loans. With the most important label to predict is healthy loans, which has a higher recall score and precision score than high risk loans. 
