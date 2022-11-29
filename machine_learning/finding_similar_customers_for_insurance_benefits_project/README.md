# Project: Finding Similar Customers for Insurance Benefits

## Description and Purpose of Project:

The *Sure Tomorrow* insurance company wanted to solve several tasks with the help of Machine Learning and use principles of linear algebra. The purpose of this project was to to evaluate that possibility, and solve the following tasks:

- Task 1: Find customers who are similar to a given customer by creating a K nearest neighbors algorithm and test with difference distances (Manhattan, Euclidean). This will help the company's agents with marketing.
- Task 2: Predict whether a new customer is likely to receive an insurance benefit. Determine if a prediction model can do better than a dummy model.
- Task 3: Predict the number of insurance benefits a new customer is likely to receive using a linear regression model.
- Task 4: Protect clients' personal data without breaking the model from the previous task by encrypting their data. 

For this project, it was necessary to develop a data transformation algorithm that would make it hard to recover personal information if the data fell into the wrong hands. This is called data masking, or data obfuscation. But the data should be protected in such a way that the quality of machine learning models doesn't suffer. Therefore, in this project we also showed how data obfuscation doesn't affect the quality of machine learning models and showed how the algorithm works correctly.

The project instructions were the following: 

- Load the data.
- Check that the data is free of issues — there is no missing data, extreme values, and so on.
- Work on each task.
- Draw conclusions.

## Business value:
The business value from this project include helping the marketing campaigns to find similar customers and predict whther a customer is likely to receive an insurance benefit.
## Tools and concepts used in project:
- Data encrypting
- Linear Algebra 
- numpy
- pandas
- seaborn
- sklearn.linear_model
- sklearn.metric
- KNeighborsClassifier
- sklearn.preprocessing
- matplotlib.pyplot
- math 

## Table of contents:
```
1  Initialization
2  Load Data
3  Processing Data for Analysis
  3.1  Processing gender column
  3.2  Processing age column
  3.3  Processing income column
  3.4  Processing family_members column
  3.5  Processing insurance_benefits column
  3.6  Description of df after data processing
4  EDA
5  Task 1. Similar Customers
  5.1  Non-scaled df , finding 10 nearest neighbors using dist. metrics: Euclidean and Manhattan
  5.2  Scaled df , finding 10 nearest neighbors using dist. metrics: Euclidean and Manhattan
  5.3  Conclusions From calculating the 10 Nearest Neighbors
6  Conclusion for task 2
7  Conclucion for Task 3
8  Proof That Data Obfuscation Can Work with LR
9  Test Linear Regression With Data Obfuscation
10  Appendix B: Properties of Matrices
```
