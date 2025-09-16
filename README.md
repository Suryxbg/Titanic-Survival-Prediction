# Titanic-Survival-Prediction

## Project Objective
The goal of this project is to perform exploratory data analysis (EDA) and feature engineering on the Titanic dataset. The main objective is to uncover patterns and relationships between passenger attributes (age, sex, class, etc.) and survival outcomes, which can later be used for predictive modeling.

## Dataset Used
- <a href="https://github.com/Suryxbg/Titanic-Survival-Prediction/blob/main/train.csv">Titanic_Dataset</a>

## Key Questions (KPIs)
During the analysis, the following key questions were addressed:
- What percentage of passengers survived overall?
- How did gender and class impact survival chances?
- Did age distribution play a role in survival rates?
- What role did family size have on survival?
- How did fare values vary across different survival outcomes?

## Process

- Data Import & Inspection
  - Loaded the dataset into pandas.
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

<img width="1484" height="1180" alt="dashboard_image_Titanic" src="https://github.com/user-attachments/assets/fd17b99a-acf1-45e4-8f2c-382ea728320c" />


## Project Insights 

- Gender effect: Female passengers had significantly higher survival rates.
- Class effect: First-class passengers had better chances of survival compared to third class.
- Age distribution: Children had slightly better survival rates than older passengers.
- Fare: Higher fares correlated with higher survival probability.
- Family size: Passengers with small family groups had better survival chances compared to those traveling alone or with very large families.

## Conclusion 

- The survival patterns suggest that socio-economic status and gender biases strongly influenced rescue priorities during the Titanic disaster, with women and higher-class passengers prioritized.
- The role of fare highlights that economic inequality was indirectly linked to survival chances, as wealthier passengers were often placed in safer areas of the ship.
- Family size analysis shows a nuanced outcome: moderate family groups had support advantages, whereas being alone or in a very large family reduced survival probability.
- Collectively, these findings indicate that survival was less about random chance and more about social structures (class, wealth, and gender norms) that governed evacuation practices.



