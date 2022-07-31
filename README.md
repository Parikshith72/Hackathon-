# Hackathon-
Problem Statement:
MyHom is a finance company that lends housing loans at the best and most affordable interest rates to customers. In recent times, the company incurred heavy losses due to loan defaults. Most applicants failed to repay the loan as per the promissory note.
In order to avoid such losses, the company has decided to build a system for identifying the loan defaulters automatically based on data. This will help the company identify potential applicants and ensure the process's smooth running.
Now, the company challenges the Data Science community to build a smart AI system to predict the probability of an applicant defaulting the loan or not in the future
 
Data Assessment:
The initial view of the dataset revealed many null values.
First, we checked the train dataset columns for completeness compared to the test dataset. That was fine. Initial analysis also revealed that some data features were embedded as numeric and also categorical.

Data Cleaning:

Checking the null value which is only the education class was imputed by constant value as per the majority count.
The categorical variable(proof_submitted) that was previously embedded as a categorial(string) was converted into numeric(int) by one hot encoding.
Removing the unwanted data that doesn’t show any hidden pattern with the target class.

Feature Engineering:
smooting used for data balencing
Feature Engineering was done by manipulating the existing class to make the pattern with the target class


Model Selection:

Transformed data were trained on 5 models:
XG boost
Naive Bayes
Random forest_with grid search
XGboost was ultimately able to properly estimate the majority of the true values after training with all 4models. In addition, the notebook's other model was cleared out to display only random_forest with grid search initial steps.
