# credit-risk-classification


Explain the purpose of the analysis.
This analysis examines historical lending activity from a peer-to-peer lending services company. My goal was to build a model that can identify the crediworthiness of borrowers. The data used in this       analysis classified each loan as being healthy(0) or being at high-risk(1).

Explain what financial information the data was on, and what you needed to predict.
The model was created to predict if a loan would be classified as being healthy or high-risk by using financial information on each borrower which included: loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total debt.

Provide basic information about the variables you were trying to predict (e.g., value_counts).
I was trying to predict whether or not the loan status was "healthy" or "high-risk"

Describe the stages of the machine learning process you went through as part of this analysis.
I started with reading the csv file containing the data and creating a Pandas DataFrame. I then separated the desired target, or dependent variable from the data. In this case the target variable used was "loan status" which was labled as either a 0 which was considered as healthy or 1 for being high-risk. This target data was defined as being the "y" variable and the rest of the data was defined as "X". Once the data was separated, it was split into training and testing datasets by using train_test_split from sklearn. From here I created a Logistic Regression model and fit the data. Then I used the data in the model to make my predictions. I then created a confusion matrix and classification report to analyze the results.

Briefly touch on any methods you used (e.g., LogisticRegression, or any other algorithms).
I used LogisticRegression. This uses binary variables with only two possible outcomes. In this case it was "0" for "Healthy" and "1" for "High-Risk". The model makes predictions and outputs the probability score.

Results
Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1:
Description of Model 1 Accuracy, Precision, and Recall scores.
Accuracy: 0.99
Precision: 1.00 for "Healthy", 0.85 for "High-Risk"
Recall: 0.99 for "Healthy", 0.91 for "High-Risk"
Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

Which one seems to perform best? How do you know it performs best?
Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the 1's, or predict the 0's? )
In this case I would believe that it is more important to predict the "1" for "High-Risk" because if you were a lender it would be more problematic if you had more "High-Risk" borrowers than anticipated.

If you do not recommend any of the models, please justify your reasoning. 
I would recommend trying to make a model where the precision for the High-Risk lenders was more accurate. The precision of 0.85 is not terrible but there is room for improvement.
