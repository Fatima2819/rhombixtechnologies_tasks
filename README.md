# Titanic-survival-prediction
This project aims to predict the survival of Titanic passengers based on a set of features including age, gender, passenger class, and more. By leveraging a machine learning approach with the Titanic dataset, this project demonstrates the end-to-end data science workflow, from data exploration to model evaluation.

**Table of Contents**
1) Project Overview
2) Dataset Description
3) Project Steps
4) Data Exploration & Visualization
5) Data Preprocessing
6) Feature Engineering & Selection
7) Model Training
8) Model Evaluation
9) Results
10) Future Enhancements
11) Contributin
# Project Overview
This project was developed as part of my internship at Rhombix Technologies and serves as a hands-on application of data science and machine learning techniques. Using the famous Titanic dataset, the project predicts passenger survival outcomes based on available features. The model chosen is Logistic Regression, optimized for binary classification tasks like this.

# Dataset Description
The dataset used in this project is a modified version of the Titanic dataset from Kaggle. It contains information on 891 passengers, including:

PassengerId: Unique identifier for each passenger
Survived: Survival indicator (1 = Survived, 0 = Did not survive)
Pclass: Passenger’s class (1st, 2nd, or 3rd)
Name: Passenger’s name
Gender: Passenger’s gender
Age: Passenger’s age
SibSp: Number of siblings/spouses aboard
Parch: Number of parents/children aboard
Ticket: Ticket number
Fare: Fare paid for the ticket
Cabin: Cabin number (often missing)
# Project Steps
# Data Exploration & Visualization
Exploratory Data Analysis (EDA) was conducted to understand patterns in survival based on various factors:
Survival by Gender: Visualized higher survival rates among females.
Survival by Passenger Class: Observed that passengers in 1st class had a higher chance of survival.
Age Distribution and Survival: Examined age groups to identify any survival trends.
# Data Preprocessing
Handling Missing Values: Missing values in the Age and Fare columns were filled with the median and mean values, respectively.
Dropping Irrelevant Columns: The Cabin column, containing many missing values, was removed to streamline the model.
Encoding Categorical Variables: Gender and Embarked columns were converted into binary indicators.
# Feature Engineering & Selection
The following features were selected for training the model:
Pclass (Passenger class)
Age
SibSp (Number of siblings/spouses aboard)
Parch (Number of parents/children aboard)
Fare
Gender (Encoded)
Embarked (Encoded)
# Model Training
A Logistic Regression model was chosen due to its effectiveness with binary classification. The dataset was split into training (80%) and test (20%) sets, and the model was trained with a maximum of 200 iterations.
# Model Evaluation
The model was evaluated using the following metrics:
# Accuracy Score
Confusion Matrix: Visualized using Seaborn to depict true positives and negatives.
Classification Report: Precision, recall, and F1 scores provided a complete performance analysis.
# Results
The Logistic Regression model achieved high accuracy in predicting survival outcomes, with the following results:
Overall Accuracy: ~100%
Confusion Matrix: Showed precise predictions for both survival and non-survival cases.
Classification Report: Precision and recall values were excellent for both classes, confirming the model’s reliability.
# Future Enhancements
Exploring Additional Models: Trying models like Decision Trees, Random Forests, or Gradient Boosting to compare performance.
Hyperparameter Tuning: Conducting grid search or cross-validation to optimize model parameters.
Feature Engineering: Creating additional features like family size or title extraction from names for deeper analysis.
# Contributing
Contributions are welcome! Please create a pull request or open an issue if you have suggestions.
Embarked: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)
