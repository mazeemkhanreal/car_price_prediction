# Car Price Prediction Using Regression

This project predicts car selling prices based on various features like fuel type, seller type, transmission type, and present price using a **Linear Regression model**.

## Overview

The project involves:
1. Exploratory Data Analysis (EDA) of car dataset.
2. Data preprocessing using encoding and scaling techniques.
3. Training a Linear Regression model to predict car prices.
4. Evaluating model performance using metrics like MAE, MSE, and R² score.
5. Visualizing relationships and predictions for better insights.

## Features

- Exploratory Data Analysis (EDA) with plots and statistical summaries.
- Data preprocessing using manual encoding, one-hot encoding, and feature scaling.
- Linear Regression model for price prediction.
- Performance evaluation with metrics and visualizations.
- Heatmaps and regression plots for feature correlation and actual vs predicted results.

## Libraries Used

- `pandas`: For data manipulation and analysis.
- `matplotlib` & `seaborn`: For data visualization.
- `scikit-learn`: For model building, preprocessing, and evaluation.

## Dataset

The dataset used in this project is named `car data.csv` and contains the following columns:
- `Car_Name`
- `Selling_Price`
- `Present_Price`
- `Fuel_Type`
- `Seller_Type`
- `Transmission`
- `Owner`

## Workflow

### 1. Data Exploration
- The dataset is loaded using pandas.
- Key statistical metrics and missing values are analyzed using `.info()`, `.describe()`, and `.isnull().sum()`.

### 2. Data Visualization
- Bar plots are used to visualize the relationship between categorical features (`Fuel_Type`, `Seller_Type`, `Transmission`) and `Selling_Price`.
- A heatmap shows correlations between numeric features.
- Regression plots visualize relationships like `Present_Price` vs `Selling_Price`.

### 3. Data Preprocessing
- **Encoding**: 
  - Manual encoding for `Fuel_Type` (`Petrol`, `Diesel`, `CNG`).
  - One-hot encoding for `Seller_Type` and `Transmission`.
- **Feature Scaling**:
  - Used `StandardScaler` to standardize numeric features.

### 4. Model Training
- Features (`X`) and target variable (`y`) are split into training and test datasets using `train_test_split`.
- Linear Regression is trained using the training data.

### 5. Model Evaluation
- Model predictions are evaluated using:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - R² Score
- The results are visualized with a regression plot comparing actual vs predicted prices.


