# Project: **ML Model Predicting the Recovery of Gold**

## Description and Purpose of Project:
Zyfra, a company that develops efficiency solutions for heavy industry, needed a  prototype of a machine learning model to predict the amount of gold recovered from gold ore. They provided with data for extraction and purification stages of gold recovery. To build the machine learning model, Zyfra provided us with following documentations about the different processes that occur during the recovery of gold: 
- Mined ore undergoes primary processing to get the ore mixture or rougher feed, which is the raw material for flotation (also known as the rougher process). After flotation, the material is sent to two-stage purification.
1. Flotation: Gold ore mixture is fed into the float banks to obtain rougher Au (gold) concentrate and rougher tails (product residues with a low concentration of valuable metals).
The stability of this process is affected by the volatile and non-optimal physicochemical state of the flotation pulp (a mixture of solid particles and liquid).
2. Purification: the rougher concentrate undergoes two stages of purification. After purification, we have the final concentrate and new tails.

The process can be explained in the image below:

<img src="Image (1).png" height = 400>

For the calculation of gold recovery, we used the following formula: 
<img src="Image (2).png" height = 200>

where:

- C — share of gold in the concentrate right after flotation (for finding the rougher concentrate recovery)/after purification (for finding the final concentrate recovery)
- F — share of gold in the feed before flotation (for finding the rougher concentrate recovery)/in the concentrate right after flotation (for finding the final concentrate recovery)
- T — share of gold in the rougher tails right after flotation (for finding the rougher concentrate recovery)/after purification (for finding the final concentrate recovery)

For the evaluation metric, we used sMAPE, symmetric Mean Absolute Percentage Error dpicted below: 
<img src="Image (3).png" height = 200>

The denotation of sMAPE are the following:

<img src="Image (4).png" height = 100>
Value of target for the observation with the i index in the sample used to measure quality. 

<img src="Image (5).png" height = 100>
Value of prediction for the observation with the i index, for example, in the test sample.

<img src="Image (6).png" height = 100>
Number of observations in the sample.

<img src="Image (7).png" height = 100>
Summation over all observations of the sample (i takes values from 1 to N).

Using the models, we need to predict two values:
- rougher concentrate recovery rougher.output.recovery
- final concentrate recovery final.output.recovery

The values will be go into the final metric, which includes these two values:

<img src="Image (8).png" height = 200>

## Business value:

The business value from this project include providing a machine learning model that help Zyfra predict the amount of gold that can be extracted from gold ores. 
## Tools and concepts used in project:

- pandas
- numpy 
- datetime 
- seaborn 
- matplotlib.pyplot 
- scipy.stats
- DecisionTreeClassifier
-  DecisionTreeRegressor
- sklearn.model_selection (cross_val_score, KFold, GridSearchCV)
- LinearRegression
- RandomForestRegressor
- sklearn.metrics (mean_absolute_error, mean_squared_error, make_scorer)
- DummyRegressor
## Table of contents:
```
1  Libraries Used for Analyss
2  Importing the Data files
  2.1  source_data
    2.1.1  source_data preprocessing
      2.1.1.1  fixing datatype for the columns in source_data
      2.1.1.2  fixing the missing values
  2.2  train_data
    2.2.1  train_data preprocessing
      2.2.1.1  fixing datatype for the columns in train_data
      2.2.1.2  fixing the missing values
  2.3  test_data
    2.3.1  test_data preprocessing
      2.3.1.1  fixing datatype for the columns in test_data
      2.3.1.2  fixing the missing values
  2.4  preparing the data
3  Analyzing the data
  3.1  Gold concentrations
  3.2  Lead concentrations
  3.3  Silver concentrations
  3.4  Comparing Feed Particle Size and Concentration Distributions
    3.4.1  Feed Distribution rougher.input.feed_size
    3.4.2  Feed Distribution primary_cleaner.input.feed_size
    3.4.3  Comapring Total Concentrations of Substances at Different Stages
      3.4.3.1  Raw Feed Total Concentrations
      3.4.3.2  Rougher Concentrate Total Concentrations
      3.4.3.3  FInal Concentrate Total Concentrations
    3.4.4  Saving train_data and test_data After Removal of Outliers
4  Models
  4.1  Creating LinearRegression Model
  4.2  DecisionTreeRegressor Model
  4.3  RandomForestRegressor Model
  4.4  Selecting the Best Model
5  Conclusion
```
