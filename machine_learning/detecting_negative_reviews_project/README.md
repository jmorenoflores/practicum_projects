# Project: **ML to Automatically Detect Negative Reviews.**

## Description and Purpose of Project:

The Film Junky Union, a new edgy community for classic movie enthusiasts, is developing a system for filtering and categorizing movie reviews. The purpose of this project was to train a model to automatically detect negative reviews. For our exploratory data analysis and training/validation/testing components of the project, we used a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. The goal of this project was to reach an F1 score of at least 0.85. 

The following structure was used in this project:
```
1. Load the data.
2. Preprocess the data, if required.
3. Conduct an EDA and make your conclusion on the class imbalance.
4. Preprocess the data for modeling.
5. Train at least three different models for the given train dataset.
6. Test the models for the given test dataset.
7. Compose a few of our own reviews and classify them with all the models.
8. Check for differences between the testing results of models in the above two points, and explain them.
9. Present findings.
```
## Business value:
The business value from this project include the implementation of a system that filters and categorizes movie reviews. 

## Tools and concepts used in project:
- math
- numpy
- pandas
- matplotlib
- matplotlib.pyplot
- seaborn
- tqdm
- re
- sklearn.metrics
- DummyClassifier
- nltk
- TfidfVectorizer
- LogisticRegression
- nltk.corpus.stopwords
- nltk.tokenize.word_tokenize
- nltk.stem.WordNetLemmatizer
- spacy
- LGBMClassifier
- GridSearchCV
- RandomizedSearchCV
- torch
- transformers.BERT

## Table of contents:
```
1  Initialization
2  Load Data
  2.1  Preparing the columns for Analysis
    2.1.1  review colmn
    2.1.2  pos column
    2.1.3  ds_part column
3  EDA
4  Evaluation Procedure
5  Normalization
6  Train / Test Split
7  Working with models
  7.1  Model 0 - Constant
  7.2  Model 1 - NLTK, TF-IDF and LR
  7.3  Model 2 - spaCy, TF-IDF and LR
  7.4  Model 4 - spaCy, TF-IDF and LGBMClassifier
  7.5  Model 9 - BERT
8  My Reviews
  8.1  Model 1
  8.2  Model 2
  8.3  Model 4
  8.4  Model 9
9  Conclusions
```
