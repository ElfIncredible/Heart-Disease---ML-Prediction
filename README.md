# Heart Disease - ML Prediction
The goal of this project is to predict if someone has a heart disease or not depending on the data provided.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Machine Learning Prediction](#machine-learning-prediction)
- [Install dependencies](#install-dependencies)
- [Data collection and processing](#data-collection-and-processing)
- [Splitting features and target](#splitting-features-and-target)
- [Splitting training data and test data](#splitting-training-data-and-test-data)
- [Model training - Logistic Regression](#model-training---logistic-regression)
- [Model evaluation - Accuracy score](#model-evaluation---accuracy-score)

## Project Overview

## Dataset

## Machine Learning Prediction
### Install dependencies
Set up the necessary imports for preprocessing data, splitting it into training and testing sets, creating a logistic regression model, and evaluating its accuracy.

### Data collection and processing
- Load the dataset from a CSV file into a DataFrame
- Inspect it by displaying the first few rows, checking its dimensions, summarizing statistics, and listing column names. I
- Check for missing values and examine the distribution of the target variable, which indicates whether the heart is defective (1) or healthy (0).

### Splitting features and target
- Separate the dataset into features (X) and the target variable (Y),
- Display the first few rows of each.
- Print the names of the feature columns for future use, such as in a web app interface.

### Splitting training data and test data
- Split the dataset into training and testing sets, ensuring the target variable distribution is preserved.
- Initialize a StandardScaler and fit it to the training data to prepare for feature scaling.

### Model training - Logistic Regression
Create a LogisticRegression model instance and then trains (or fits) the model on the training data (X_train and y_train). This process involves adjusting the model's parameters to learn the relationship between the features and the target variable, enabling it to make predictions on new data.

### Model evaluation - Accuracy score
