# Car Purchase Amount Prediction Model

## Overview

This project aims to predict car purchase amounts using machine learning based on historical sales data. The model analyzes various factors such as age, annual salary, credit card debt, net worth, and customer demographics to predict the amount a customer is likely to spend on a car purchase.

## Dataset

The project utilizes the "car_purchasing.csv" dataset, which contains information about customer demographics, financial details, and car purchase amounts.

## Methodology

The following steps were undertaken to develop the prediction model:

1. **Data Loading:** The dataset was loaded into a pandas DataFrame.
2. **Data Exploration:** The dataset was explored to understand its structure, features, data types, and distributions. Missing values, outliers, and correlations between variables were checked.
3. **Data Cleaning:** Outliers were handled using the IQR method for numerical features, and potential data issues were addressed.
4. **Data Wrangling:** Categorical variables were transformed into numerical representations using one-hot encoding. New features, such as interaction terms and ratios, were created to potentially improve model performance. Multicollinearity among features was checked to ensure model stability.
5. **Data Splitting:** The dataset was split into training, validation, and testing sets to train, tune, and evaluate the model.
6. **Model Training:** A linear regression model was trained using the training data to predict car purchase amounts.
7. **Model Evaluation:** The model's performance was evaluated using metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared on the validation and testing sets.
8. **Data Visualization:** The model's performance and insights obtained from the analysis were visualized using scatter plots, residual plots, and feature importance bar charts.

## Results

The trained linear regression model achieved a very high R-squared value (approximately 0.99999997) on the testing set, indicating a strong fit to the data and accurate predictions. The MAE and RMSE were also relatively low, suggesting accurate predictions.

## Usage

To use the model for prediction, follow these steps:

1. Load the trained model from the saved model file.
2. Preprocess the input data using the same steps as in the data cleaning and wrangling stages.
3. Use the model's `predict` method to predict the car purchase amount for the input data.

## Conclusion

The car purchase amount prediction model provides valuable insights into the factors influencing car purchases. It can be used by businesses to optimize marketing strategies, target potential customers, and forecast sales growth.

## Future Work

Further improvements to the model can be explored, such as:

* Exploring non-linear models like decision trees or random forests.
* Incorporating additional relevant features.
* Fine-tuning hyperparameters to optimize model performance.
