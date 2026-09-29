# Air Quality Forecasting using Machine Learning

## Project Overview

This project analyses historical air-quality measurements from the UCI Air Quality Dataset and uses machine learning to predict future carbon monoxide (CO) concentration.

The project includes data preprocessing, exploratory data analysis, feature engineering, machine-learning prediction, model evaluation, error analysis, and feature importance.

## Objectives

- Understand and preprocess air-quality data
- Analyse air-quality patterns and relationships
- Create useful time-based features
- Predict future CO concentration
- Evaluate the machine-learning model
- Analyse prediction errors
- Identify important features

## Dataset

The project uses the UCI Air Quality Dataset.

Dataset source:

https://archive.ics.uci.edu/dataset/360/air+quality

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook

## Machine Learning Model

Random Forest Regressor

## Features Used

The model uses:

- Previous CO concentration
- Temperature
- Relative humidity
- Hour of the day
- Day of the week

## Target Variable

The target variable is the next CO concentration measurement.

## Data Preprocessing

The dataset contains `-200` values representing missing measurements. These values were replaced with missing values and numerical data was interpolated.

Date and time information was also combined into a single datetime column.

## Exploratory Data Analysis

The project analyses:

- CO concentration distribution
- CO concentration over time
- Relationship between temperature and CO
- Correlation between air-quality variables

## Model Evaluation

The model is evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

## Data Leakage Prevention

Since this is a time-series prediction problem, the data was split chronologically.

The first 80% of the observations were used for training and the final 20% were used for testing.

Previous CO measurements were used as features to predict the next CO measurement.

## Project Structure

```text
air-quality-forecasting/
│
├── Air_Quality_Forecasting.ipynb
└── README.md
