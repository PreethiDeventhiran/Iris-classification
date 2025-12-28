# 🏠 House Price Prediction using Machine Learning

## Project Overview

This project focuses on building a regression-based machine learning model to predict house prices using various property-related features such as size, location, and other attributes.

The project demonstrates an end-to-end machine learning workflow including data preprocessing, feature engineering, model training, evaluation, and prediction.  
It was developed as part of a Machine Learning Internship task.

---

## Problem Statement

House prices are influenced by multiple factors and often exhibit non-linear behavior.  
The objectives of this project are to:

- Analyze the housing dataset
- Handle missing values appropriately
- Perform feature transformation and encoding
- Train and compare multiple regression models
- Evaluate models using suitable performance metrics
- Demonstrate predictions on new, unseen data

---

## Dataset

- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/bhanupratapbiswas/house-price-prediction  

Each row represents a house, and each column represents a feature affecting house price.  
The target variable is the **house price**.

---

## Technologies Used

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Jupyter Notebook  

---

## Project Workflow

### 1. Data Loading
- Loaded the dataset using Pandas
- Inspected data structure, data types, and basic statistics

### 2. Exploratory Data Analysis (EDA)
- Checked for missing values
- Analyzed feature distributions
- Studied the distribution of the target variable

### 3. Data Preprocessing
- Handled missing values using statistical methods
- Applied log transformation to the target variable to reduce skewness
- Encoded categorical features using One-Hot Encoding
- Scaled numerical features using StandardScaler

### 4. Feature Engineering
- Separated numerical and categorical features
- Used `ColumnTransformer` and `Pipeline` for clean and reproducible preprocessing

### 5. Model Training
The following regression models were trained and compared:
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

### 6. Model Evaluation
Models were evaluated using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

Residual analysis was also performed to examine prediction behavior.

### 7. Model Selection
Gradient Boosting Regressor showed the best performance based on evaluation metrics and was selected as the final model.

### 8. Model Saving
The trained model was saved using `joblib` to allow reuse without retraining.

### 9. Prediction
The saved model was used to demonstrate house price prediction on new input data.

---

## Evaluation Metrics Explained

- **MAE (Mean Absolute Error):**  
  Measures the average absolute difference between actual and predicted prices.

- **RMSE (Root Mean Squared Error):**  
  Penalizes larger errors more heavily and is sensitive to outliers.

---

## Project Structure

