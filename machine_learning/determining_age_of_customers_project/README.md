# Project: **Determining age of customers**

## Description and Purpose of Project:

The supermarket chain Good Seed would like to explore whether Data Science can help them adhere to alcohol laws by making sure they do not sell alcohol to people underage. The purpose of this project was to conduct this evaluation by using methods of Computer Vision while keeping in mind the following specifications:

- The shops are equipped with cameras in the checkout area which are triggered when a person is buying alcohol
- Computer vision methods can be used to determine age of a person from a photo
- The task then is to build and evaluate a model for verifying people's age

The shops are equipped with cameras in the checkout area which are triggered when a person is buying alcohol Computer vision methods can be used to determine age of a person from a photo. The purpose of this project was to build and evaluate a model for verifying people's age For this project, we were provided with photographs of people with their ages indicated.

The project was built based on the folowing structure: 
```
1. Perform exploratory data analysis of 'age' column to get an overall impression of the dataset.
2. Train and evaluate the model (it needs to be done on the GPU platform).
3. Combine your code, output and findings (from the previous points) in the final Jupyter notebook.
4. Make conclusions of the model evaluation, add them to the notebook.
```
## Business value:

This business value from this project include the implementation of computer vision to determine the age of customer's when they are purchasing alcohol. The use of computer vision could reduce sales of alcohol to people who are underaged. 

## Tools and concepts used in project:

- pandas
- tensorflow.keras.preprocessing.image.ImageDataGenerator
- matplotlib.pyplot
- seaborn
- PIL.Image
- tensorflow
- ResNet50
- tensorflow.keras.models.Sequential
- tensorflow.keras.layers.GlobalAveragePooling2D
- tensorflow.keras.layers.Dense
- tensorflow.keras.layers.Dropout
- tensorflow.keras.layers.Flatten
- tensorflow.keras.optimizers.Adam 
- inspect 

## Table of contents:
```
1  Project: Determining age of customers
  1.1  Libraries Used for Analysis
2  Load Data
3  Exploratory Data Analysis
  3.1  Distribution of 'real_age' values
  3.2  Distribution of ouliers for 'real_age' values
  3.3  Distribution of underage 'real_age' values
  3.4  Distribution of underage vs. legal age to buy alcohol values.
4  Conclusion from Exploratory Data Analysis
5  Modelling
6  Prepare the Script to Run on the GPU Platform
  6.1  Output
7  Conclusions
```
