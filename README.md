# Titanic-Survival-Prediction

## Project Objective
The goal of this project is to perform exploratory data analysis (EDA) and feature engineering on the Titanic dataset. The main objective is to uncover patterns and relationships between passenger attributes (age, sex, class, etc.) and survival outcomes, which can later be used for predictive modeling.

## Dataset Used
- <a href="https://github.com/Suryxbg/Titanic-Survival-Prediction/blob/main/train.csv">Dataset</a>

## Key Questions (KPIs)
During the analysis, the following key questions were addressed:
- What percentage of passengers survived overall?
- How did gender and class impact survival chances?
- Did age distribution play a role in survival rates?
- What role did family size have on survival?
- How did fare values vary across different survival outcomes?

## Process

- Data Import & Inspection
  - Loaded the dataset (train.csv) into pandas.
  - Inspected shape, columns, datatypes, and missing values.
  - Dropped irrelevant identifiers such as PassengerId.

- Data Cleaning
  - Handled missing values in Age and Embarked columns.
  - Checked for duplicate records and outliers using boxplots and violin plots.
  - Converted categorical variables (Sex, Embarked) into usable formats.

- Exploratory Data Analysis (EDA)
  - Univariate analysis: distribution of Age, Fare, Pclass, Survived.
  - Bivariate analysis: relationship between survival and Sex, Pclass, Family Size.
  - Multivariate analysis: interaction of multiple factors on survival rates.
  - Visualizations created using Matplotlib and Seaborn.

- Feature Engineering
  - Created Family Size feature = SibSp + Parch + 1.
  - Grouped age into bins (Children, Teens, Adults, Seniors).
  - Transformed skewed variables (like Fare) for better distribution.
  - Encoded categorical features (Sex, Embarked) for model readiness.

- Model Readiness
  - Split data into features (X) and target (y).
  - Ensured all features were numeric and scaled where necessary.
  - Saved cleaned dataset for future predictive modeling.
 
## Dashboard

- <a href = "<img width="1484" height="1180" alt="dashboard_image_Titanic" src="https://github.com/user-attachments/assets/85f44fe5-a999-40da-9686-a57287525d69"/>"


