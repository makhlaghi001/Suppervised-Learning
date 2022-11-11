### Module 12 Analysis Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The purpose of this Anlysis was to take a highly imblanced credit lending data set, and fit it within a logistic regression model, against both original data and resampled data.   

* Explain what financial information the data was on, and what you needed to predict.

The dataset would is a set of credit lending data set, which consists of 77,536 rows and 8 columns. The columns aras as follows:
   
   loansize, 
   
   Interest Rate, 
   
   Borrower Income, 
   
   Debt to Income, 
   
   Number of Accounts, 
   
   Deragatory Marks, 
   
   Total Debt, 
   
   Loan Status. 
   
In this analysis we are predicting the result/outcome for loan status. This is to indicate if the model will be able to predict the creditworthiness of borrowers.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

The variable that was predicted in this model, was the loan status of individuals. This was to indicate their credit worthiness through scores of 1 and 0. 1 being highly risky and 0 for healthy loans. 

* Describe the stages of the machine learning process you went through as part of this analysis.

Split the Data into Training and Testing Sets

Created a Logistic Regression Model with the Original Data

Predicted a Logistic Regression Model with Resampled Training Data

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

Some of the methods that where used in this analysis to calculate:

Value counts - To check balance of lables X and y

train_test_split- was used to split the data in to X and y, training and testing data.

Logistic Regression Model- was used to creat prediction of the y_pred on both original and resampled data


Random Over Sampler- was used in order to balance the imbalnced data set and fit into the model, in order to do prediction.


For both original and resampled dataset perdiction we generated and calculated the following:

   accuracy score of the model.
    
   Generate a confusion matrix.
   
   Generated the classification report.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
      
 Model 1 provided with us with a,
 
 
   Accuracy rate of 99%
   
   percision rate of 100% on healthy loands and 87% on the unhealthy loans
   
   recall rate of 100% on healthy loans and 89% on the unhealthy loans. 
     


* Machine Learning Model 2:
 
Accuracy rate of 99%
 
percision rate of 100% on healthy loands and 87% on the unhealthy loans
 
However recall rate improved on the prediction of unhealthy loans. The model predicted 100% on healthy loans and 100% on the unhealthy loans. 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?


he oversampled data set perfomed better, as it improved the unhealthy recall rate to 100%. 


* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )


It is more importtan to predict the 1's, as we donot want the loans to defult. 

If you do not recommend any of the models, please justify your reasoning.
