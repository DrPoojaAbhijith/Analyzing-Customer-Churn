# Capstone-Project : Analyzing Customer Churn


![image](https://github.com/DrPoojaAbhijith/Analyzing-Customer-Churn/assets/160575120/7b764ead-3a3e-4dcc-acd9-4dd66d4e530b)


## Table Of Contents
1.	Problem Statement
2.	Project Objective
3.	Data Description
4.	Data Pre-processing steps and inspiration
5.	Choosing the algorithm for the project
6.	Motivation and reasons for choosing the algorithm
7.	Conclusion
 
## Problem Statement
A telecom company named “Neo” whose customers are churning out to its competitors. we have to analyze the data of our company and find insights and stop your customers from churning out to other telecom companies.

## Project Objective

![image](https://github.com/DrPoojaAbhijith/Analyzing-Customer-Churn/assets/160575120/11ef81c0-a6f3-491e-acf7-a75d61549b20)


## 1. Data Manipulation: 
● Extract the 5th column and store it in ‘customer_5’ 

● Extract the 15th column and store it in ‘customer_15’ 

● Extract all the male senior citizens whose payment method is electronic check and store the result in ‘senior male electronic’ 

● Extract all those customers whose tenure is greater than 70 months or their monthly charges is more than $100 and store the result in ‘customer total tenure’

● Extract all the customers whose contract is of two years; payment method is mailed check and the value of churn is ‘Yes’ and store the result in ‘two mail yes’ 

● Extract 333 random records from the customer churn data frame and store the result in ‘customer_333’ 

● Get the count of different levels from the ‘Churn’ column


## 2. Data Visualization: 
● Build a bar-plot for the ’Internet Service’ column: 

a. Set x-axis label to ‘Categories of Internet Service’ 

b. Set y-axis label to ‘Count of Categories’ 

c. Set the title of plot to be ‘Distribution of Internet Service’ 

d. Set the color of the bars to be ‘orange’ 

● Build a histogram for the ‘tenure’ column: 

a. Set the number of bins to be 30 

b. Set the color of the bins to be ‘green’ 
c. Assign the title ‘Distribution of tenure’ 

● Build a scatter-plot between ‘Monthly Charges’ and ‘tenure’. Map ‘Monthly Charges’ to the y-axis and ‘tenure’ to the ‘x-axis’: 

a. Assign the points a color of ‘brown’ 

b. Set the x-axis label to ‘Tenure of customer’ 

c. Set the y-axis label to ‘Monthly Charges of customer’ 

d. Set the title to ‘Tenure vs Monthly Charges’ 

e. Build a box-plot between ‘tenure’ & ‘Contract’. Map ‘tenure’ on the y-axis & ‘Contract’ on the x-axis.

## 3. ML MODEL IMPLEMENTATION: 

### Linear Regression:
Build a simple linear model where dependent variable is ‘Monthly Charges’ and independent variable is ‘tenure’: 

a. Divide the dataset into train and test sets in 70:30 ratio. 

b. Build the model on train set and predict the values on test set 

c. After predicting the values, find the root mean square error 

d. Find out the error in prediction & store the result in ‘error’ 

e. Find the root mean square error

### 4. Logistic Regression: 

● Build a simple logistic regression model where dependent variable is ‘Churn’ and independent variable is ‘Monthly Charges’: 

a. Divide the dataset in 65:35 ratio 

b. Build the model on train set and predict the values on test set 

c. Build the confusion matrix and get the accuracy score 

d. Build a multiple logistic regression model where dependent variable is ‘Churn’ and independent variables are ‘tenure’ and ‘Monthly Charges’ 

e. Divide the dataset in 80:20 ratio 

f. Build the model on train set and predict the values on test set 

g. Build the confusion matrix and get the accuracy score 5. 

### Decision Tree: 
● Build a decision tree model where dependent variable is ‘Churn’ and independent variable is ‘tenure’: 

a. Divide the dataset in 80:20 ratio 

b. Build the model on train set and predict the values on test set 

c. Build the confusion matrix and calculate the accuracy

### 6. Random Forest: 
● Build a Random Forest model where dependent variable is ‘Churn’ and independent variables are ‘tenure’ and ‘Monthly Charges’: 

a. Divide the dataset in 70:30 ratio 

b. Build the model on train set and predict the values on test set 

c. Build the confusion matrix and calculate the accuracy

## Data Description
![image](https://github.com/DrPoojaAbhijith/Analyzing-Customer-Churn/assets/160575120/b0567de5-567a-4939-9dae-58660bf8c692)

 
### Data Pre-processing steps and inspiration

1. **Loading the Dataset:** The initial step involves loading the dataset into the analysis environment, typically using libraries like Pandas in Python, ensuring accessibility for further examination.

2. **Checking for Data Types:** It is imperative to inspect the data types of each column to ensure consistency and appropriateness for subsequent analyses and operations.

3. **Preprocessing Data:** In the Preprocessing step we have created new data frames according to the tasks which are given in the ‘Task’s to be performed’.  

5. **Handling Outliers:** Since The Features in the dataset is categorical there is no scope for outliers.


## 6. Exploring and finding the Inferences from the Data: 
•	 I have plotted all the categorical features in one frame with the help of ‘for loop’ and I found the below inferences

•	**Gender:** As Per Gender Column there is no big difference in Churning

•	**Senior Citizen:** As Per Gender Senior Citizen the people who are not senior citizen is having more Churn

•	**Partner:** The People Who has no Partner is churning more

•	**Dependents:** The People has no dependents has more churn

•	**Phone Services:** People who are having Phone services has more churn

•	**Multiple Lines:** People who has no Phone services has churning less

•	**Internet Services:** People who has Fiber Optic Services is having more Churn

•	**Online Security:** People who not having Online security has churning more, may be the concerns about their privacy

•	**Online Backup:** People who not having Online Backup has churning more

•	**Device Protection:** People who not having Device Protection has churning more

•	**Tech Support:** People who not having Tech Support has churning more

•	**Streaming TV:** People who has not facility of Streaming TV is Churning More

•	**Streaming Movies:** People who has not facility of Streaming Movies is Churning More

•	**Contract:** People who has month to month subscription is Churning More

•	**Paperless Billing:** People who has Paperless Billing has churning more, may be the people who has paper bill not have any concerns about their expenditure towards the telephone services

•	**Payment Method:** The Electronic Check Payment method has highest Churning comparing to the others

•	**Churn:** Overall Churning is less than the entire population in the dataset


## Inferences from other features:
•	**Distribution of Internet Service:** The Fibber Optic services is having high Subscriptions compared to DSL

•	**Distribution of Tenure:** There is a max subscription for tenure 0 to 3 months and 70 months tenure. Apart from that most of the tenure distributed more or the same.

•	**Tenure V/s Monthly Charges:** There is a positive correlation between the tenure and monthly charges. As the tenure increases the monthly charges are also increasing.

•	**Tenure V/s Monthly Charges:** There is a positive correlation between the tenure and monthly charges. As the tenure increases the monthly charges are also increasing.

•	**Tenure V/s Contract:** for two-year contract most of the people choose tenure for 50 to 70 months which high.

•	And for one year contract the people are chosen 30 to 60 months tenure.

•	For Month to Month Contract the people chosen 0 to 30 months tenure. When we compare Two year and Month to Month Contract in terms of tenure there is a opposite behaviours. May be the people who is choosing the MOM subscriptions new to the telecom services. Or they may consider that this telecom sim as a secondary option. The telecom company need to focus more on them.

## Choosing the algorithm for the project
Here we have chosen different model’s that can predict weather the customer will Churn or not. Models listed below:

1.	**Linear Regression**
   
•	Motive for this model is to predict the monthly charges depending on the tenure.

•	In this model our independent feature would be tenure and dependent feature is to be Monthly Charges

•	And we will evaluate the model performance with the help of RMSE.

•	And we also find error in prediction and store it in variable called ‘error’.

2.	**Logistic Regression**
   
•	Motive for this model is to predict weather the customer will churn or not based on the monthly charges.

•	We will evaluate the model with accuracy score function.

•	And create confusion matrix to find how many correctly and wrongly predicted values.

3.	**Multiple Logistic Regression**
   
•	In this model we have two independent features and one dependent feature.

•	Motive for this model is to predict weather the customer will churn or not based on the tenure and monthly charges.

•	We will evaluate the model with accuracy score function.

•	And create confusion matrix to find how many correctly and wrongly predicted values.


4.	**Decision Tree**
   
•	Motive for this model is to predict weather the customer will churn or not based on the tenure 

•	We will evaluate the model with accuracy score function.

•	And create confusion matrix to find how many correctly and wrongly predicted values.

5.	**Random Forest**
    
•	In this model we have two independent features and one dependent feature.

•	Motive for this model is to predict weather the customer will churn or not based on the tenure and monthly charges.

•	We will evaluate the model with accuracy score function.

•	And create confusion matrix to find how many correctly and wrongly predicted values.

6.	**Grid Search CV**
    
•	This is a hyperparameter tool which will help to increasing in the model performance.

•	**Listed parameters below:**

•	**N estimators:** This parameter specifies the number of trees in the forest. Increasing the number of trees generally improves performance, but at some point, the benefits diminish and training time increases.

•	**Max depth:** Controls the maximum depth of each tree in the forest. Deeper trees can capture more complex relationships in the data, but they are more prone to overfitting. Experiment with different values to find the right balance.

•	**Min Sample Split:** Specifies the minimum number of samples required to split an internal node. Increasing this parameter can help prevent overfitting by requiring a certain number of samples in each split.

•	**Min Sample Leaf:** Sets the minimum number of samples required to be at a leaf node. Increasing this parameter can also help prevent overfitting by creating simpler trees with fewer leaf nodes.

•	**Max features:** Determines the number of features to consider when looking for the best split. Using a smaller value can reduce overfitting by forcing each tree to consider a subset of features.

•	**Boot Strap:** Controls whether bootstrap samples are used when building trees. Setting this parameter to True (the default) enables bootstrapping, which can introduce randomness and improve generalization.


## Motivation and reasons for choosing Model’s

1. **Linear Regression**
    
•	Motive for choosing this model is to predict the target which is continues in nature. Which is regression problem.

•	In this model our independent feature would be tenure and dependent feature is to be Monthly Charges. Both our models are continuing in Nature.

2.	**Logistic Regression**
    
•	The Target is a classification output. That the customer will churn or not. For such problems Logistic Regression will work well. 

•	And it is a Simple Logistic Regression as there is only one dependent and one independent features.

3.	**Multiple Logistic Regression**
    
•	The Target is a classification output. That the customer will churn or not. 

•	And it is a Multiple Logistic Regression as there is more than one predictor. For such problems Multiple Logistic Regression will work well.

4.	**Decision Tree**
    
•	Decision tree models are adept at handling classification and regression problems. 

•	by recursively partitioning the input space into regions, making predictions based on the majority class or average value within each region. 

•	This allows them to handle both categorical and numerical data, making them versatile for a wide range of predictive tasks in various domains.


5.	**Random Forest** 
•	Random Forest offers high predictive accuracy by averaging predictions from multiple decision trees, making it robust to overfitting. 
•	It handles non-linear relationships well, provides feature importance insights, and is resilient to outliers and missing data. With its scalability, ability to handle large datasets, and no assumptions about data distribution, Random Forest is a versatile choice suitable for various machine learning tasks.


## Conclusion

•	Based on the analysis conducted and the model’s performance on the dataset, it can be concluded that the Liner Regression for predicting Monthly Charges and Simple & Multiple Logistic Regression and Decision Tree and Random Forest will be fit and suitable for weather the customer Churn or Not.

•	**In Linear Regression we got the evaluation matrix which is RMSE we got RMSE Score is 5.86**

•	**In Logistic Regression we got the accuracy score 73%.**

•	**In Multiple Logistic Regression** we got the accuracy score 80%. Which is higher than the simple logistic regression model.

•	**In Decision Tree** we got the accuracy score 76%. Which is Lower than the simple logistic regression model.

•	**In Random Forest** we got the accuracy score 78%. Which is Lower than the simple logistic regression model.

# Thank You!

