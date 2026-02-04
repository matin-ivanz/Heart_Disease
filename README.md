# Heart Disease & ML(classification)

## Overview

- This project focuses on Exploratory Data Analysis (EDA), data visualization, feature engineering, and machine learning classification using the Heart Disease dataset. Patient information and medical examinations can show us what diseases the patient has, and with this data we can understand whether the patient has heart disease. After analyzing the data using a supervised machine learning model, it can be predicted that the patient has heart disease.

## Objective

- The goal of this project is to prepare medical datasets for analysis and demonstration of patient characteristics and machine learning for predicting heart disease in patients.

## Key Skills Demonstrated

- Exploratory Data Analysis (EDA) using Pandas & NumPy
- Data visualization with Matplotlib & Seaborn
- Feature engineering with features based on individual characteristics
- Statistical analysis and distribution interpretation
- Supervised classification model learning (Random Forest Classification)
- Data preprocessing and scaling with StandardScaler
- Model evaluation and performance analysis
- Model reinforcement and selection of the best values ​​for model parameters
- Writing clean, structured, and reproducible Python code

## Dataset

- Source: kaggle
- Name: UCI Heart Disease Data
- Rows: 920
- Columns: 16
- Link: https://www.kaggle.com/datasets/redwankarimsony/heart-disease-dataset

### Features

- id: Each patient's ID number
- age: Patient age in years
- sex: Gender of the patient
- dataset: Place of study
- cp: Type of chest pain
- trestbps: Resting blood pressure
- chol: Serum cholesterol
- fbs: blood sugar
- restecg: Resting electrocardiographic results
- thalch: Maximum heart rate
- exang: Exercise-induced angina
- oldpeak: Exercise-induced ST segment depression compared to rest
- slope: ST segment slope peak exercise
- ca: Number of main vessels
- thal: Heart rate
- num: Anticipated feature

## Feature Engineering

Three features were created based on the classification of some features:
age_group: Age grouping
high_bp: High and low blood pressure 140
high_chol: High and low cholesterol 240

These features help the model to be less error-prone.

## Tools

- Python
- Pandas
- Itertools
- Matplotlib
- Seaborn
- Scikit-learn

## Visualizations

The following plots are generated to analyze the data:

- Histogram (distribution by species)
- Scatter Plot (relationships between features)
- Heatmap (features correlations)
- Box Plot (outlier detection)
- Pie Chart (species distribution)
- Pair Plot (pairwise feature relationships)
- Violin Plot (distribution by species)

## Machine Learning

- Model: Support Classifier (Random Forest Classifier)
- Data Scaling: StandardScaler
- Change the type of data: LabelEncoder, OneHotEncoder
- Train/Test Split: applied before training
- Selecting critical columns for the prediction feature: SelectKBest(score_func=f_classif)
- Strengthening the model: GridSearchCV
- Accuracy of the model: roc_auc_score

## Model Evaluation

- Model: Random Forest Classifier
- Basic accuracy: Accuracy at its highest (80%)
- Accuracy after amplification: Accuracy has not changed because the data is not balanced.

## Results

- Men are more likely to suffer from this disease.
- In the Switzerland dataset, the ratio of infected to healthy people is higher.
- People with asymptomatic chest pain are more likely to have heart disease.
- People with flat ST segment elevation are more likely to have heart disease.
- People in the senior age group are more likely to be affected by this disease (from 55 to 80 years old).
- The number of individuals in each group in each characteristic is shown in the pie chart.
- There is a high correlation in the numerical characteristics of patients, and infected and healthy individuals do not differ much in these characteristics.
- The features are closely related but the correlations are low.
- The model accuracy is 80%, meaning there is an 80% chance that the model's prediction is correct.

## Conclusion

This project demonstrates a complete data science workflow:

- Data Cleaning
- Data Mining
- Visualization
- Feature Engineering
- Machine Learning Modeling
- Model Boosting

This project shows us what characteristics people with heart disease have and with these characteristics we can use the model to predict the disease.
