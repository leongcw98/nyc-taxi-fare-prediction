# New York City Taxi Fare Prediction

## Overview

The goal of this project is to predict taxi fare prices in New York City using historical trip data. By applying various machine learning models, the project aims to forecast fare amounts based on features such as pickup and dropoff locations, time, and the number of passengers.

## Dataset

The dataset used for this project can be downloaded from [Kaggle: 2014 New York City Taxi Trips](https://www.kaggle.com/kentonnlp/2014-new-york-city-taxi-trips). It includes the following features:

1. **pickup_latitude**: Latitude of the pickup location
2. **pickup_longitude**: Longitude of the pickup location
3. **dropoff_latitude**: Latitude of the dropoff location
4. **dropoff_longitude**: Longitude of the dropoff location
5. **fare_amount**: Fare amount for the trip
6. **pickup_datetime**: Date and time of pickup
7. **passenger_count**: Number of passengers

## Techniques Used

- **Feature Engineering**: Creating new features and transforming existing ones to enhance model performance.
- **Data Visualization**: Using visual tools to explore and understand data patterns and relationships.
- **Data Preprocessing**: Cleaning and preparing data, including handling missing values and encoding categorical variables.
- **Machine Learning Modeling**: Implementing and comparing various regression models to predict fare prices.

## Algorithms Used

- **MeanRegressor**: A baseline model predicting the mean of fare amounts.
- **Linear Regression**: A basic model assuming a linear relationship between features and fare.
- **Ridge Regression**: A regularized linear regression model to address multicollinearity.
- **Random Forest**: An ensemble method that uses multiple decision trees to improve prediction accuracy.
- **Gradient Boosting (XGBoost)**: An advanced ensemble technique that builds models sequentially to correct the errors of previous models.
- **Hyperparameter Tuning**: Bayesian Optimization was used to fine-tune the XGBoost model for optimal performance.

## Results

- **Best Model**: XGBoost Regressor with Bayesian Optimization
- **Performance Metric**: Achieved a Root Mean Squared Error (RMSE) of 3.215, demonstrating effective predictive performance.
- **Feature Importance**: `trip_distance` was identified as the most influential feature in predicting fare amounts.

## Conclusion

The XGBoost Regressor, optimized with Bayesian techniques, provided promising results with a low RMSE. The identification of `trip_distance` as a key predictor underscores its importance in fare prediction and offers valuable insights for future improvements.

## Future Plans

- **Model Improvement**: Explore additional features and more advanced techniques to enhance model accuracy.
- **Data Collection**: Gather more data to improve model robustness and accuracy.
- **Feature Engineering**: Conduct further analysis to refine and select features that enhance the model.
- **Model Deployment**: Consider deploying the model in real-world scenarios and establish monitoring practices.
- **Exploratory Data Analysis (EDA)**: Perform additional EDA to gain deeper insights and improve feature selection.

## Installation

### Clone the Repository

```bash
git clone https://github.com/leongcw98/new-york-city-taxi-fare-prediction.git
cd new-york-city-taxi-fare-prediction
