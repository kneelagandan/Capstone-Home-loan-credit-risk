# Capstone-Project 1 - Home Loan Credit Risk 

# Final Report -https://github.com/kneelagandan/Capstone-Home-loan-credit-risk/blob/main/Milestone%20Report/Home_Loan_Milestone_Report.pdf

# Problem Statement:

Home Credit is an organization that serves the unbanked population with access to loans. Such individuals that do not have a built-up credit score have a challenging time securing loans from financial institutions.
Home Credit strives to broaden financial inclusion for the unbanked population by providing a positive and safe borrowing experience. In order to make sure this underserved population has a positive loan experience; Home Credit makes use of a variety of alternative data--including telco and transactional information--to predict their clients' repayment abilities
So, problem statement would be predicting how likely each applicant is of repaying a loan?

# Modeling & In-Depth Analysis:

Preprocessing data set before creating ML modeling:
1.	Imputer – Added SimpleImputer & strategy to calculate ‘’Median” for the set, transformed data set.
2.	Scaler – Added MinMaxScaler for all feature value range from 0-1 for computation 
Created Train & Test data set with 33 % test size. Which is going to be applied in ML Models 

Early Models: As data set belongs to Supervised Machine learning, applied below Algorithms  

# Metrics to be used: ROC-AUC Score

# Machine Learning Algorithm Used:
-	Logistic Regression
-	Random Forest
-	Naïve Bayes
-	XGB Boost
-	Ensemble Modeling (combined above 4)
-	Deep Learning – Keras


# Conclusion:
Bayesian Optimization was used to tune the XG Boost Classification models. Subsequently, a kfold cross validation with 8 splits was conducted to evaluate the validity of the models.
The averaged CV result was a roc_auc of 0.740 with a standard deviation of 0.005.
Also, we can refer Neural Network Keras model for the prediction which has0.844 roc_auc score
This is a significant improvement on the early models that did not include as many variables and only relied on the mean groupings of past financial transactions. 

It can therefore be concluded that the new variables significantly help in the identification of features that might make someone more likely to have challenges in repaying a loan.

