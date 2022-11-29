# Project: **Determining Price of Vehicles with Machine Learning**

## Description and Purpose of Project:

Rusty Bargain used car sales service is developing an app to attract new customers. In that app, you can quickly find out the market value of your car. You have access to historical data including: technical specifications, trim versions, and prices. For this project, we built a maching learning model with use of numerical method techniques to determine the value of vehicles. 

Rusty Bargain was interested in the following:
- the quality of the prediction
- the speed of the prediction
- the time required for training For this project

In this project, we trained different models with various hyperparameters (some models had various implementations of gradient boosting.) The main point of this step was to compare gradient boosting methods with random forest, decision tree, and linear regression. Similarly, we analyzed the speed and quality of the models and used the RMSE metric to evaluate the models. Since the Linear regression model is not very good for hyperparameter tuning, we used it as a sanity check of other methods. Somethign we kept in mind is that if gradient boosting performs worse than linear regression, something definitely went wrong.

## Business value:

Provide Rusty Bargain Used Cars Sales Service with a machine learning model that predicts a reasonable value of their vehicles, based on historical data. 

## Tools and concepts used in project:
- pandas
- numpy
- matplotlib.pyplot
- sklearn.preprocessing.OrdinalEncoder
- sklearn.preprocessing.StandardScaler
- LGBMRegressor
- sklearn.model_selection.GridSearchCV
- sklearn.model_selection.RandomizedSearchCV
- sklearn.metrics
- datetime 
- RandomForestRegressor 
- DecisionTreeRegressor
- sklearn.metrics.make_scorer
- lightgbm
- CatBoostRegressor
- XGBRegressor 
- LinearRegression
## Table of contents: 
```
1  Project: Determining Price of Vehicles with Machine Learning
2  Data preparation
  2.1  fixing column names
  2.2  datecrawled column
  2.3  price column
  2.4  vehicletype column
  2.5  registrationyear column
  2.6  gearbox column
  2.7  power column
  2.8  model column
  2.9  mileage column
  2.10  registrationmonth column
  2.11  fueltype column 
  2.12  brand column
  2.13  notrepaired column
  2.14  datecreated column
  2.15  numberofpictures column 
  2.16  postalcode column
  2.17  lastseen column
  2.18  data after fixing errors in column
3  Model training
  3.1  Preparing datasets for model training
  3.2  RandomForestRegressor Model, Non-Scaled Features Data
  3.3  RandomForestRegressor Model, Scaled Features Data
  3.4  DecisionTreeRegressor Model, Non-scaled Features Data
  3.5  DecisionTreeRegressor Model, scaled Features Data
  3.6  CatboostRegressor
  3.7  Linear Regression Model
  3.8  Conclusion From Model Training
4  Model analysis
5  Conclusion
```
