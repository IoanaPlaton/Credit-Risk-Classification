# Module 12 Report Template

## Overview of the Analysis

* The purpose of this analysis was to determine how accurately the logistic regression model can predict the health of a loan or its risk using training data. 

* The data we were given included the following information: loan size, interest rate, borrower income, debt to income, number of credit accounts, derogatory marks, total debt, and loan status. 

* Using the data we were given, I first created a label variable for the loan status data column so it could be used as our comparison data point in the regression model later on. The remainder of the data was separated into our features, which would be used to predict the loan's status.

* From there, the data was split into training and testing data using the train_test_split module. Then, I applied the Logistic Regression Model using the training data to determine the training and testing data scores. Then, I saved the test data predictions versus the actuals into a data frame to use the confusion matrix on the results and determine the classification report outcomes on the training and testing data.

## Results
These are the training classification report results for the logistic regression model:

* Precision—the precision of the training data resulted in an accuracy of 100% when predicting a healthy loan and 85% when predicting a high-risk loan. 

* Recall scores—the recall score is 99% when predicting a healthy loan and 89% when predicting an unhealthy loan.

* The accuracy for precision and recall is in the high nineties, meaning our model is really accurate at predicting loan health.

These are the testing classification report results for the logistic regression model:

* Precision—the precision of the testing data resulted in an accuracy of 100% when predicting a healthy loan and an accuracy of 87% when predicting a high-risk loan. 

* Recall scores —the recall score is 100% when predicting a healthy loan and 89% when predicting an unhealthy loan.

* The accuracy for precision and recall is in the mid-nineties, meaning our model is pretty accurate at predicting loan health with the test data.

## Summary 
* Looking at the two classification reports for the training and test data, model performance stayed almost the same between the two data sets. Since we're getting strong precision and recall on the training and test dataset, it is a good indication that the model is likely to provide accurate results in real life.

* When we look at the prediction data and the results for the high-risk loan, we should note that the model's performance is not as accurate as it is at predicting healthy loans. One would need to take this percentage into account in a real-life setting and determine if a 15% chance of errors is okay.

* If we were solely using this model to predict health loans, yes, I would recommend it. However, if we were using it to find unhealthy loans, I would exercise caution, as it may miss out on risky loans.