# Energy-Consumption-Time-Series-Forecasting

Objective

The main goal of this project is to forecast short-term household energy consumption by applying multiple forecasting techniques and comparing their performance.

Dataset Description

The dataset used in this project is the Household Power Consumption dataset obtained from the UCI Machine Learning Repository. The data contains minute-level measurements of household electricity usage.

Key Attributes

Date

Time

Global_active_power

The Global_active_power variable is used as the target for forecasting.

Data Preprocessing

The following preprocessing steps were performed:

Combined Date and Time columns into a single datetime variable

Converted power measurements into numeric format

Removed missing and invalid values

Resampled minute-level data into hourly averages

Split the dataset into training and testing sets using an 80/20 ratio

Models Used
ARIMA

A classical statistical time-series model used to capture trends and autocorrelation within the data.

Prophet

A forecasting model designed to handle seasonality and trend changes, particularly effective for time-series data with daily and weekly patterns.

XGBoost

A machine learning regression model that leverages engineered time-based features such as hour of day, day of week, and weekend indicators.

Evaluation Metrics

Model performance was evaluated using the following metrics:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

Lower values indicate better forecasting accuracy.

Visual Analysis

The project includes visualizations to support analysis and evaluation, including:

Time series plots of hourly energy consumption

Training and testing data split visualization

Comparison of actual versus predicted energy consumption

These visualizations help in understanding model behavior and forecasting performance.

Tools and Technologies

Python

Pandas

NumPy

Matplotlib

Statsmodels

Prophet

XGBoost

Scikit-learn

How to Use This Repository

Users can run the project by installing the required Python libraries and executing the notebook cells sequentially in a Jupyter environment.

Results and Findings

The results show that Prophet and XGBoost perform better than ARIMA in capturing seasonal patterns. XGBoost benefits from engineered time-based features, leading to improved predictive accuracy.

Repository Structure

The repository is organized to include the dataset, notebook files, and documentation for ease of use and reproducibility.

Conclusion

This project demonstrates the application of time-series forecasting techniques to real-world energy consumption data. By comparing statistical and machine learning models, the project highlights the strengths and limitations of each approach.
