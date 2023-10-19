# Salary Prediction Analysis

![Project Image](salary-data.jpg)

## Overview

This repository contains a comprehensive analysis of the "Salary Data.csv" dataset, aiming to predict salaries based on several features like age, years of experience, gender, and job title. The project is notable for its extensive use of advanced machine learning tools, including the `Pipeline`, `ColumnTransformer`, and `TransformedTargetRegressor` APIs from scikit-learn, ensuring a streamlined and efficient modeling process. Through rigorous data processing, visualization, and machine learning, we've derived valuable insights and built predictive models with impressive accuracy.
![pipeline](pipeline-dell.e.jpg)


## Dataset

The primary dataset used is "Salary Data.csv", which encompasses several features:
- **Age**: The age of the employees.
- **Years of Experience**: The total working experience of the employees.
- **Gender**: The gender of the employees.
- **Job Title**: The designation or role of the employees.
- **Education Level**: The highest educational qualification of the employees.
- **Salary**: The annual salary of the employees (our target variable).

## Procedures and Analysis

### Data Exploration and Visualization:

- Loaded the dataset into a pandas DataFrame for easy manipulation and analysis.
- Conducted a comprehensive overview of the dataset, understanding its structure and content.
- Used statistical measures to understand the distribution and central tendencies of the data.
- Visualized the data using libraries like `matplotlib` and `seaborn` to understand the relationships between different features and the target variable.

### Data Preprocessing:

- Handled missing values and outliers.
- Utilized `ColumnTransformer` to apply different preprocessing to different columns: encoding categorical variables and scaling numerical ones, all in a single step, maintaining the efficiency of the workflow.
- Split the dataset into training and testing sets to train and subsequently evaluate our machine learning models.

### Model Training and Evaluation:

- Created a `Pipeline` that streamlined the preprocessing and modeling steps, improving the code's maintainability and reproducibility.
![pipeline](pipeline-overview.jpg)

- Employed `TransformedTargetRegressor` to scale the target variable, optimizing model performance.
- Employed several regression algorithms, including:
    - Linear Regression
    - Decision Tree Regression
    - Extra Tree Regression
    - Gradient Boosting Regression
    - Random Forest Regression
    - Ridge Regression
    - Lasso Regression
    - Elastic Net Regression

- Trained each model on the training set and evaluated their performance on the testing set using R-squared as the metric.

## Results

The R-squared values for each of the models are as follows:

- **Linear Regression**: 0.8556
- **Decision Tree Regression**: 0.8889
- **Extra Tree Regression**: 0.8997
- **Gradient Boosting Regression**: 0.9160
- **Random Forest Regression**: 0.9111
- **Ridge Regression**: 0.9036
- **Lasso Regression**: 0.9027
- **Elastic Net Regression**: 0.9046

The Gradient Boosting Regression model showed the highest R-squared value, indicating it performed the best among all the models in terms of explaining the variance in the dataset.
