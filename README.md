# Property_price_prediction
Property Price Prediction using Machine Learning

This project applies machine learning techniques to predict property prices based on multiple features such as location, house condition, size, furnishing, and other structural characteristics. The analysis covers the entire workflow — from data cleaning and exploratory data analysis (EDA) to model training, evaluation, and tuning.

Project Overview

Accurate property price estimation is a key problem in the real estate industry.
In this project, a dataset containing property details (size, age, number of bedrooms, bathrooms, furnishing type, etc.) is analyzed and modeled to predict the market price (USD) of a property.

The workflow follows standard data science practices:

Data Loading and Cleaning

Data Preprocessing and Feature Engineering

Exploratory Data Analysis (EDA)

Model Training (Linear Regression and Random Forest)

Hyperparameter Tuning

Model Evaluation and Comparison

Model Saving for Future Predictions

Machine Learning Methods Used

Multiple Linear Regression — Baseline model for continuous price prediction.

Random Forest Regressor — Ensemble method used to capture nonlinear relationships and improve accuracy.

GridSearchCV — Used for hyperparameter tuning and performance optimization.

Pipeline and ColumnTransformer — Automate preprocessing and ensure consistent transformations across training and testing datasets.

Technologies and Libraries
Category	Libraries
Data Analysis	pandas, numpy
Visualization	matplotlib, seaborn
Machine Learning	scikit-learn
Model Persistence	joblib
Utility	datetime
Project Workflow
1. Data Cleaning

Fixed column name inconsistencies (e.g., spacing, capitalization, spelling).

Corrected categorical entry mismatches in furnishing, location, and house_condition.

Handled missing values using the mode for categorical variables and median for numeric features.

2. Feature Engineering

Created a new feature house_age = current year - year built.

Encoded categorical variables using OneHotEncoder.

Standardized numeric features using StandardScaler.

3. Exploratory Data Analysis

Visualized distributions and relationships for key variables:

Property price, house age, lot size, and square footage.

Countplots for categorical variables like furnishing, location, and house condition.

4. Model Training and Evaluation

Split the dataset into 80% training and 20% testing sets.

Trained two regression models:

Linear Regression

Random Forest Regressor (tuned with GridSearchCV)

Evaluated models using:

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

R-squared (R²)
