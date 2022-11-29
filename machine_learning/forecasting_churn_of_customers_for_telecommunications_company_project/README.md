# Project: **Forecasting Churn of Clients for Interconnect Company.**

## Description and Purpose of Project:
The telecommunications company, Interconnect, would like to be able to forecast their churn of clients. If it's discovered that a user is planning to leave, they will be offered promotional codes and special plan options. Interconnect's marketing team has collected some of their clientele's personal data, including information about their plans and contracts.

The purpose of this project was to create a Machine Learning model that predicts which costumers are at 'risk' of leaving the telecommunications company. The datasets provided from Interconnect include the costumers's personal information; information about their costumer's contracts; and information about costumers' phone and internet plans. Our tasks included pre-processing the data for analysis, for each of the datasets, including check for missing data, errors in data entry, and duplicates. After processing each of the datasets, we joined the the tables into one dataset that contained all the relevant data for each of the costumers. We joined the datasets by using the costumer ID column. By using this joined dataset, we observed and explored the data of the costumers to get an insight of the distribution of values in columns and inbalance of target classes.

For the rest of the project, we created machine learning models and selected the best model, with the highest AUC-ROC score. The threshold for the selected model was an AUC-ROC score was 0.85, and also our baseline was a logistic regression model. Any models that perfomed worse, in terms of AUC-ROC score, than the logistic regression model were not considered for testing. The reason that we selected a logistic regression model as our baseline is because other models allow for hyperparameter tuning, as well as the use of optimization techniques such as gradient descent. We decided to keep all the columns from the datasets providesd, with the exception of the column 'enddata'. The reason we removed this column was because we created the target feature, 'churned', and keeping the enddate column would have caused to have redundant data.

The model combinations perfomed in this project include:

0. Logistic regression model with encoded categorical data, as a baseline. This model was used as the baseline to compare it agaisnt models that allow for gradient descent optimization, and/or hyperparameter tuning.

i. Logistic Regression Model, with upsampled class 1 in target; class 0 unchanged in target

ii. Logistic Regression Model, with unchanged class 1 in target; class 0 downsampled in target;non-standarized numerical columns

iii. Random Forest classifier with unchanged class 1 in target; class 0 unchanged in target; non-standarized numerical columns

iv. Random Forest classifier with upsampled class 1 in target; class 0 unchanged in target; standarized numerical columns

v. Random Forest classifier with unchanged class 1 in target; class 0 downsampled in target; standarized numerical columns

vi. KNeighborsClassifiers Model with Upsampled class 1 in target, class 0 unchanged in target, and standarized numeric columns

vii. CatboostClassifier Model with unchanged class 1 in target; class 0 unchanged in target

## Business value:

The business value from this project was to retain the customers that are at risk of leaving the services from the Interconnect company. 

## Tools and concepts used in project:

- pandas
- numpy
- matplotlib.pyplot
- seaborn
- LogisticRegression
- RandomizedSearchCV
- GridSearchCV
- sklearn.metrics 
- sklearn.utils.shuffle
- RandomForestClassifier
- StandardScaler
- OrdinalEncoder
- CatBoostClassifier
- KNeighborsClassifier

## Table of contents:
```
1  Libraries Used for Analysis
2  Pre-Processing Datasets for Analysis
  2.1  df_personal dataset
  2.2  df_contract dataset
  2.3  df_phone dataset
    2.3.1  Checking duplicates or Errors in Data Entry and Datatype
  2.4  df_internet dataset
    2.4.1  Checking duplicates or Errors in Data Entry and Datatype
3  Merging all Datasets for Analysis.
4  Exploratory Data Analysis and Pre-processing Data for Merged Dataset, df_data
  4.1  Fixing Missing Values in columns and Checking if column if Useful for Machine Learning Models
    4.1.1  gender column
    4.1.2  seniorcitizen column
    4.1.3  partner column
    4.1.4  dependents column
    4.1.5  begindate column
    4.1.6  enddate column
    4.1.7  type column
    4.1.8  paperlessbilling column
    4.1.9  paymentmethod column
    4.1.10  monthlycharges column
    4.1.11  multiplelines column
    4.1.12  internetservice column
    4.1.13  onlinesecurity column
    4.1.14  onlinebackup column
    4.1.15  deviceprotection column
    4.1.16  techsupport column
    4.1.17  streamingtv column
    4.1.18  streamingmovies column
    4.1.19  Monthly Charges and Total Charges
    4.1.20  churned column class inbalance
  4.2  Work plan:
  4.3  Libraries used for Machine Learning models
  4.4  Preparing Data for Machine Learning Training, Testing, and Validation
    4.4.1  Splitting dataset into training and testing datasets
    4.4.2  OHE for Logistic Regression algorithm
    4.4.3  OrdinalEncoding for RandomForestClassifer Models
    4.4.4  Upsampling Class 1 in Target Column 'churned'
    4.4.5  Donwsampling Class 0 in Target Column 'churned'
  4.5  Model 0: Logistic Regression Model, Baseline
  4.6  Model 1: Logistic Regression Model, with upsampled class 1 in target; class 0 unchanged in target
  4.7  Model 2 : Logistic Regression Model, with unchanged class 1 in target; class 0 downsampled in target
  4.8  Model 3:Random Forest classifier with unchanged class 1 in target; class 0 unchanged in target;
  4.9  Model 4: Random Forest classifier with upsampled class 1 in target; class 0 unchanged in target; standarized numerical columns
  4.10  Model 5: Random Forest classifier with unchanged class 1 in target; class 0 downsampled in target; standarized numerical columns
  4.11  Model 6. KNeighborsClassifiers Model with Upsampled class 1 in target, class 0 unchanged in target, and standarized numeric columns
  4.12  Model 8. CatboostClassifier Model with unchanged class 1 in target; class 0 unchanged in target
5  Testing Models with test dataset
  5.1  Model 0, baseline
  5.2  Model 3
6  Conclusion From testing
7  Solution Report
```
