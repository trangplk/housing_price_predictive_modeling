# housing_price_predictive_modeling

## Overview
This Jupyter Notebook is dedicated to cleaning and preprocessing data for a real estate dataset from https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques. It includes importing necessary packages, importing the data, handling missing values, and implementing multiple regression, random forest, and gradient boosting models.

### Requirements
- Python 3.10
- Libraries: pandas, numpy, seaborn, matplotlib, sklearn.

### Data Import and Preprocessing
The dataset is read from a CSV file. Initial steps involve dropping irrelevant columns, setting display options for pandas, and inspecting the data types and basic statistics.

#### Handling Missing Values
- Categorical missing values are filled with 'None'.
- Null values in 'MasVnrArea' are replaced with 0.
- 'LotFrontage' missing values are replaced with the neighborhood average.
- Rows with null 'Electrical' are dropped.

### Exploratory Data Analysis
- A heatmap is used to visualize the correlation between different features.
- Distribution of the target variable ('SalePrice') is checked, which is right-skewed.

### Model Implementation
The dataset is divided into 2 sets: training set and testing set for validation.  Evaluation metrics include: MAE, MSE, RMSE.

Three different models are implemented:
1. **Multiple Regression Model**
2. **Random Forest Model**
3. **Gradient Boosting**

### Conclusion
- Gradient Boosting demonstrates superior performance compared to Multiple Linear Regression and Random Forest.
- While Multiple Linear Regression is more accurate than Random Forest, the latter shows less deviation in predictions.

### Usage
To use this notebook:
1. Ensure all the required libraries are installed.
2. Run each cell sequentially to avoid dependency issues.
