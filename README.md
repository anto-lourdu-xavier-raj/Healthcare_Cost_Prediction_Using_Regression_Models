# Objective

The objective of this project is to build a predictive model that accurately forecasts medical costs based on various features of an individual, such as:

Age: The age of the person.

Sex: Gender (Male/Female).

BMI: Body Mass Index, a measure of body fat based on height and weight.

Children: Number of dependents.

Smoker: Whether the individual is a smoker (Yes/No).

Region: The region in the US (Northeast, Southeast, Southwest, Northwest).

# Introduction

Healthcare cost prediction is critical for insurance companies to determine premiums and for patients to anticipate their expenses. Using various features like age, BMI, and smoking status, this project aims to predict medical costs and identify the most influential variables affecting these costs. This regression problem provides insights that can be used to improve actuarial calculations and help individuals choose the best insurance plans for their needs.

# Dataset
The dataset used in this project contains 1338 records and includes the following columns:

Age

Sex

BMI

Children

Smoker

Region

Charges (target variable)

The dataset is sourced from the Medical Cost Personal Dataset, which is freely available and widely used for predictive modeling tasks.

# Project Workflow

# 1. Data Loading and Initial Analysis

The dataset is loaded using pandas, and basic exploratory data analysis (EDA) is performed to understand its structure and key statistics. Data cleaning ensures that no missing values exist, and categorical variables are replaced with numerical values for modeling.

# 2. Exploratory Data Analysis (EDA)

Key EDA steps include:

Visualization of categorical features (sex, smoker status, region) with count plots.

Visualization of charges by category with box plots.

Correlation heatmap to identify the relationships between the variables.

# 3. Data Preprocessing

Categorical variables are converted to numerical representations:

Male/Female to 1/0

Smoker/Non-smoker to 1/0

Region to numerical categories

# 4. Model Building

Two models are built and evaluated in this project:

Linear Regression Model

Provides a baseline for cost prediction.

Achieved an R² accuracy of 80% and a Mean Absolute Error (MAE) of 4174.

Random Forest Regressor

A more advanced model that improves prediction accuracy.

Achieved an R² accuracy of 90% and an MAE of 2485.

# 5. Model Evaluation

The performance of both models is evaluated using:

Mean Absolute Error (MAE): Measures the average magnitude of errors.

R² Score: Indicates the proportion of variance in the dependent variable predictable from the independent variables.

# 6. Actual vs Predicted Visualization

Scatter plots are generated to visualize the difference between actual and predicted medical costs for both models, with color-coded distinctions for easy interpretation.

# Results
The Random Forest Regressor outperformed Linear Regression, achieving a 90% accuracy in predicting healthcare costs.

The "Smoker" variable had the strongest correlation with medical costs, indicating that smoking status heavily influences healthcare expenses.

# Conclusion

This project successfully predicts healthcare costs based on individual features using machine learning models. The insights gained can help healthcare providers, insurers, and patients better understand cost factors and plan accordingly.

# Requirements

To run this project, install the following Python libraries:

pip install pandas matplotlib seaborn scikit-learn

# Running the Project

Clone the repository.

Load the dataset (insurance.csv).

Run the notebook or Python script to preprocess data, train models, and visualize results.
