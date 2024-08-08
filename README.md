# Heart Disease - ML Prediction
Build a heart disease prediction system using logistic regression. Demonstrate end-to-end functionality, from model training and evaluation to making and saving predictions.

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
  - [Making a predictive system](#making-a-predictive-system)
  - [Saving the trained model](#saving-the-trained-model)

## Project Overview
**Objective:** Develop a heart disease prediction system using logistic regression to classify whether a person has heart disease based on various health metrics.
**Outcome:** The project demonstrates a complete workflow from data preparation and model training to prediction and model persistence, showcasing an end-to-end approach to heart disease prediction.

## Dataset
This [dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset) dates from 1988 and consists of four databases: Cleveland, Hungary, Switzerland, and Long Beach V. It contains 76 attributes, including the predicted attribute, but all published experiments refer to using a subset of 14 of them. The "target" field refers to the presence of heart disease in the patient. It is integer valued 0 = no disease and 1 = disease.

**Content**

Attribute Information:
- age
- sex
- chest pain type (4 values)
- resting blood pressure
- serum cholestoral in mg/dl
- fasting blood sugar > 120 mg/dl
- resting electrocardiographic results (values 0,1,2)
- maximum heart rate achieved
- exercise induced angina
- oldpeak = ST depression induced by exercise relative to rest
- the slope of the peak exercise ST segment
- number of major vessels (0-3) colored by flourosopy
- thal: 0 = normal; 1 = fixed defect; 2 = reversable defect
The names and social security numbers of the patients were recently removed from the database, replaced with dummy values.

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
- Evaluate the performance of the trained LogisticRegression model by calculating its accuracy on both the training and testing datasets.
- Make predictions on the training data and the test data
- Compute and print the accuracy scores for each.

### Making a predictive system
- Prepare a single instance of input data for prediction by reshaping it into the required format,
- Use the trained logistic regression model to predict whether the person has heart disease and prints the result.

### Saving the trained model
- Save and load a trained logistic regression model and scaler using pickle.
- Prepare, standardize, and predict heart disease for a new input instance using the loaded model and scaler.
