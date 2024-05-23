# House Price Prediction Using Different Regression Models

## Overview

This project aims to build a predictive model to estimate house prices for different regions in the USA using different regression models and compares them. The model is designed to assist real estate agents by providing estimated prices based on various features of the houses and the areas they are located in.

##### The project utilizes three different regression models:
- **Linear Regression**: This model is used for predicting house prices based on linear relationships between the input features and the target - variable.
- **Ridge Regression**: Ridge regression is employed as a regularization technique to prevent overfitting by adding a penalty term to the linear regression equation.
- **Random Forest Regressor**: Random Forest Regression is a powerful ensemble learning method that uses multiple decision trees to predict house prices based on the input features.

## Dataset

The dataset provided for this project contains 5000 rows and 7 columns, with each row representing a house. The columns in the dataset are as follows:

- **Avg. Area Income**: The average income of households in the city where the house is located.
- **Avg. Area House Age**: The average age of houses in the same city.
- **Avg. Area Number of Rooms**: The average number of rooms for houses in the same city.
- **Avg. Area Number of Bedrooms**: The average number of bedrooms for houses in the same city.
- **Area Population**: The population of the city.
- **Price**: The price at which the house was sold.
- **Address**: The address of the house.


## Requirements
To run this project, you need the following libraries:

- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn

You can install these libraries using pip:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn
```

## Project Structure
The project consists of the following main components:
1. Data cleaning: Handling missing values or removing null values.
1. Exploratory Data Analysis (EDA): Analyzing the data to understand the relationships between different features and the target variable (price).
2. Data Preprocessing:  Feature selection, splitting the data and normalizing/standardizing the data.
3. Model Building: Creating and training the regression models.
4. Model Evaluation: Evaluating the model's performance using appropriate metrics.
5. Predictions: Using the model to make predictions on new data.
6. Comparison: Comparing Linear regression, Ridge regression and Random Forest Regressor models

## Results

The performance of each model on the test data is as follows:
| Model                    | MAE         | MSE             | RMSE       | R2       |
|--------------------------|-------------|-----------------|------------|----------|
| Linear Regression        | 81,116.43   | 10,062,094,881.38 | 100,309.98 | 0.914735 |
| Ridge Regression         | 81,116.81   | 10,061,930,865.79 | 100,309.17 | 0.914737 |
| Random Forest Regression| 93,587.25   | 13,962,366,782.58 | 118,162.46 | 0.881685 |

## Conclusion

- Removing the 'Avg. Area Number of Bedrooms' feature improved the performance of all models to varying degrees.
- Linear Regression and Ridge Regression performed similarly, capturing the relationships between features and prices effectively.
- Random Forest Regression, although slightly less accurate,

This predictive model can assist real estate agents in estimating house prices more accurately, aiding in decision-making processes and enhancing customer service. For different datasets the accuracy of model will differ, and Random Forest Regression might be more accurate in case of non-linear relationships.

