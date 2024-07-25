# CODTECH-Task1
# Linear Regression on Housing Prices

## Introduction

This project demonstrates the implementation of a linear regression model to predict housing prices using the Boston Housing dataset. The dataset consists of various features that impact the housing prices in the Boston area, including socio-economic and physical characteristics of the houses and neighborhoods.

## Objective

The main goal of this project is to develop a predictive model using linear regression to estimate the median value of owner-occupied homes (`medv`). The model uses the following features:

- **CRIM**: Per capita crime rate by town.
- **ZN**: Proportion of residential land zoned for lots over 25,000 sq. ft.
- **INDUS**: Proportion of non-retail business acres per town.
- **CHAS**: Charles River dummy variable (1 if tract bounds river; 0 otherwise).
- **NOX**: Nitric oxides concentration (parts per 10 million).
- **RM**: Average number of rooms per dwelling.
- **AGE**: Proportion of owner-occupied units built prior to 1940.
- **DIS**: Weighted distances to five Boston employment centers.
- **RAD**: Index of accessibility to radial highways.
- **TAX**: Full-value property tax rate per $10,000.
- **PTRATIO**: Pupil-teacher ratio by town.
- **B**: \(1000(Bk - 0.63)^2\) where \(Bk\) is the proportion of Black people by town.
- **LSTAT**: Percentage of lower status of the population.

## Data Preparation and Exploration

The dataset was examined for missing values or anomalies. It was found to contain 506 samples and 14 attributes, including the target variable `medv`. After confirming that there were no missing values, the dataset was split into features (`X`) and target (`y`).

## Model Implementation

1. **Data Splitting**: The dataset was divided into training and testing sets with an 80-20 split to ensure the model's ability to generalize.

2. **Model Training**: A `LinearRegression` model from the `scikit-learn` library was trained using the training data.

3. **Evaluation**: The model's performance was assessed on the test data using the Mean Squared Error (MSE) and R-squared (R²) metrics.

## Results

- **Mean Squared Error (MSE)**: Calculated to evaluate the average squared differences between actual and predicted values.

- **R-squared (R²)**: Assessed to determine how well the model explains the variability of the target variable.

## Visualization

A scatter plot was created to illustrate the relationship between actual and predicted housing prices. A red dashed line indicating perfect predictions was included for comparison.

## Prediction

The trained model was used to predict housing prices for a new data point with the following attributes:

- CRIM: 0.05
- ZN: 15.0
- INDUS: 2.0
- CHAS: 0
- NOX: 0.6
- RM: 6.0
- AGE: 70.0
- DIS: 4.0
- RAD: 1
- TAX: 296.0
- PTRATIO: 18.0
- B: 396.9
- LSTAT: 5.0

The predicted price for this data point was successfully output using the trained model.

## Conclusion

The linear regression model offers a straightforward method for predicting housing prices based on multiple features. The results suggest the model performs reasonably well, with potential for further refinement. Future improvements could involve feature engineering, normalization, and exploring more sophisticated models such as polynomial regression or other machine learning algorithms.

This project highlights the essential steps involved in implementing linear regression for predictive analysis, including data preparation, model training, evaluation, and interpretation of results. These models can be instrumental in real estate analytics, providing stakeholders with valuable insights for informed decision-making.

## Getting Started

To run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repository.git
