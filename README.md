# Predictive Maintenance for Aircraft Engines Using NASA Turbofan Data
Overview
This project uses NASA's CMAPS dataset to predict the Remaining Useful Life (RUL) of aircraft engines. The goal is to apply predictive maintenance to reduce operational costs and avoid unexpected engine failures by leveraging machine learning techniques.

Problem Statement
The goal of this project is to predict the Remaining Useful Life (RUL) of turbofan engines based on sensor data collected over time. By accurately predicting RUL, we aim to prevent failures and reduce downtime in industrial applications.

Data Source
The dataset used for this project is the NASA Turbofan Engine Degradation Simulation Data Set, available through NASA's Prognostics Center of Excellence.

Project Workflow
Data Loading and Preprocessing

Load data for multiple engine units and clean the dataset by removing unnecessary columns.
Handle missing data and calculate the RUL of each engine unit.
Feature Engineering

Create rolling means and exponential moving averages for each sensor to better capture short- and long-term trends in the sensor data.
Transform and scale the data for better model performance.
Modeling

Train machine learning models using XGBoost to predict RUL based on the preprocessed data.
Fine-tune hyperparameters to improve the prediction accuracy.
Evaluation

Evaluate the model using Root Mean Squared Error (RMSE) on the validation set.
Analyze feature importance to understand which sensor data contributes the most to the prediction.

Key Features
Rolling Means & Exponential Moving Averages: Feature engineering to capture sensor trends.
XGBoost Model: A powerful gradient boosting algorithm for regression tasks.
Feature Importance: Visualize which sensors are most critical for predicting RUL.
Results
RMSE on validation set: 36.88
Feature Importance: A plot of the most important features (sensors) contributing to the RUL predictions.
Future Improvements
Explore advanced time-series models like LSTMs and GRUs for better accuracy.
Build an API to serve real-time predictions for engine monitoring.
Create a real-time dashboard to visualize sensor data and RUL predictions.
Conclusion
This project demonstrates the power of machine learning for predictive maintenance, showcasing how industrial data can be used to reduce downtime and improve operational efficiency.
