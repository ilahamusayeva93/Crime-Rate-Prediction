# Crime Rate Prediction Analysis

## Overview

This repository contains an R script for predicting crime rates using the "crimes.csv" dataset. The analysis involves data loading and exploration, outlier handling, model training using both base R and H2O.ai, and evaluation of the model's performance.

## Script Details

### 1. Library Imports

- **Libraries:** The script imports various R libraries for data manipulation, visualization, and modeling, including `tidyverse`, `data.table`, `skimr`, `h2o`, and others.

### 2. Data Loading and Exploration

- **Data Loading:** The raw crime dataset is loaded using `fread`.

- **Data Exploration:** The script provides a glimpse of the data, checks for missing values, and displays outliers for numeric variables.

### 3. Outlier Handling

- **Outlier Definition:** Columns to process are defined, and a copy of the raw data is created.

- **Outlier Handling:** Outliers are handled using the IQR method, and the original and processed data are combined.

### 4. Model Training

- **Linear Regression with Base R:** A linear regression model is fitted using base R, and multicollinearity is checked and handled using VIF.

### 5. H2O.ai Model Training

- **Initialize H2O:** The H2O library is initialized, and data is converted to H2O format.

- **Model Training:** The script splits the data into training and testing sets, fits a generalized linear model using H2O.ai, and displays coefficients and p-values.

### 6. Model Evaluation

- **Performance Metrics:** The script predicts on the test set, calculates RMSE, R-squared, and Adjusted R-squared, and visualizes the results using ggplot2 and plotly.

### 7. Train Set Evaluation and Visualization

- **Train Set Metrics:** The script predicts on the training set, calculates metrics, and visualizes the results alongside the test set.

### 8. Final Summary

- **Summary Metrics:** The script provides a final summary with key metrics for both the train and test sets.

## Dataset Information

### Description

The "crimes.csv" dataset reflects reported incidents of crime that occurred in the US. The analysis aims to uncover patterns to decrease and prevent crime rates.

### Analysis Requests

1. **Multicollinearity:** Detect and handle multicollinearity using VIF.
2. **Feature Standardization:** Standardize features.
3. **Train-Test Split:** Split data into train and test sets using seed=123.
4. **Linear Regression Model:** Build a linear regression model with a maximum p-value of 0.05.
5. **Metrics Calculation:** Calculate RMSE and Adjusted R-squared.
6. **Overfitting Check:** Check for overfitting.

## How to Use

To replicate the analysis:

1. Ensure you have R and the required libraries installed.
2. Place the "crimes.csv" dataset in the same directory as the script.
3. Run the script in an R environment, considering any specific package dependencies.

## Author

- **Ilaha Musayeva**
- **Date: 10.25.2023**


