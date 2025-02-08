# Boston Housing Price Prediction

This project aims to predict housing prices in Boston using several machine learning models. The goal is to compare the performance of different models and choose the one that best fits the data.

## Overview
The project leverages various regression models to predict the median value of owner-occupied homes in Boston. The dataset includes various features such as crime rate, average number of rooms, property tax rate, etc. The models are evaluated using metrics like Mean Squared Error (MSE) and R-squared (R²).

## Models Used
1. **Linear Regression**
2. **Decision Tree**
3. **Random Forest**
4. **Gradient Boosting**
5. **XGBoost**

For each model, the performance is compared based on MSE and R² scores, and the results are presented in a table for easy comparison.

## Dataset
The dataset used in this project is the [Boston Housing Dataset](https://www.kaggle.com/datasets/camnugent/boston-housing). The dataset contains the following features:
- **CRIM**: Crime rate per capita
- **ZN**: Proportion of residential land zoned for large plots
- **INDUS**: Proportion of non-retail business acres
- **CHAS**: Charles River dummy variable (1 if tract bounds river, 0 otherwise)
- **NOX**: Nitrogen oxide concentration
- **RM**: Average number of rooms per dwelling
- **AGE**: Proportion of owner-occupied units built before 1940
- **DIS**: Weighted distance to employment centers
- **RAD**: Index of accessibility to radial highways
- **TAX**: Property tax rate
- **PTRATIO**: Pupil-teacher ratio by town
- **B**: Proportion of residents of African American descent
- **LSTAT**: Percentage of lower status population
- **MEDV**: Median value of owner-occupied homes (target variable)

You can download the dataset from [here](https://github.com/selva86/datasets/blob/master/BostonHousing.csv).

## Requirements
- Python 3.x
- Libraries: pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn

## How to Run the Project
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/SepehrAHJ/boston-housing-prediction.git

## Results

Here is a comparison of the model performances based on **Mean Squared Error (MSE)** and **R-squared (R²)**:

| Model                    | Mean Squared Error (MSE) | R-squared (R²) |
|--------------------------|--------------------------|----------------|
| Linear Regression         | 23.6544                  | 0.7244         |
| Decision Tree             | 10.4161                  | 0.8580         |
| Optimized Decision Tree   | 9.9080                   | 0.8649         |
| Random Forest             | 8.8667                   | 0.8791         |
| XGBoost                   | 6.9362                   | 0.9054         |
| Gradient Boosting         | 6.0134                   | 0.9180         |

**Interpretation:**
- **Gradient Boosting** performed the best in terms of both MSE and R² score, suggesting it is the most accurate model for predicting housing prices in this dataset.
- **Random Forest** and **XGBoost** also performed well, with similar performance to XGBoost.
- **Linear Regression** and **Decision Tree** performed slightly worse compared to the other models, but they still provide a good baseline for the predictions.

The results can be further analyzed and visualized in the project for better understanding.
