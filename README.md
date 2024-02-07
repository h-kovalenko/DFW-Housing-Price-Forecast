# Data Analysis and Forecasting of Median Housing Prices in Dallas-Fort Worth-Arlington, TX
This project focuses on analyzing and forecasting the median housing prices in the Dallas-Fort Worth-Arlington area using various time series forecasting models. The data spans from August 1, 2017, to June 1, 2023, and is sourced from  <a href="https://fred.stlouisfed.org/series/MELIPRMSA19100">FRED</a>.
### Introduction
The goal of this project is to provide insights into the future trends of median housing prices in the Dallas-Fort Worth-Arlington area. We employ three different time series forecasting models, namely Exponential Smoothing (ETS), Seasonal-Trend decomposition using LOESS (STL), and Seasonal Autoregressive Integrated Moving Average with eXogenous regressors (SARIMAX).

### Code Overview
The provided Python code uses libraries such as Matplotlib, Pandas, Statsmodels, and others for data visualization, analysis, and modeling. It follows the following steps:

* **Data Loading and Visualization:** Load data from the CSV file, rename columns, and plot the median housing prices over time.

* **Modeling with ETS:** Apply the Exponential Smoothing (ETS) model, plot the results, and calculate accuracy metrics.
  
* **Modeling with STL:** Apply the Seasonal-Trend decomposition using LOESS (STL) model, plot the decomposition, and use STLForecast based on Exponential Smoothing (ES).

* **Modeling with SARIMAX:** Install necessary library (pmdarima) and apply the Seasonal Autoregressive Integrated Moving Average with eXogenous regressors (SARIMAX) model. Plot the results and calculate accuracy metrics.

* **Future Forecasting with SARIMA:** Prepare for forecasting into the future using SARIMA, generate predictions with confidence intervals, and plot the forecast for the next 24 months.


### Models Graphs
* **ETS Model:**
  
![alt text](graphs/ETS%20Model.png?raw=true)

* **STL Model:**
![alt text](graphs/STL%20model.png?raw=true)

* **SARIMA Model:**
![alt text](graphs/SARIMA%20model.png?raw=true)

* **SARIMA forecast:**
![alt text](graphs/SARIMA%20forecast.png?raw=true)


### Model Evaluation Metrics

| Model   | RMSE   | RMSPE | MAE     | MSE           | MAPE    | AIC   | BIC    |
|---------|--------|-------|---------|---------------|---------|-------|--------|
| ETS     | 21199.5| 0.447 | 15205.5 | 4.494e+08      | 0.0328  | 934.3 | 967.8  |
| STL     | 29019.4| 0.619 | 22926.1 | 8.421e+08      | 0.05    | 990.6 | 1000.4 |
| SARIMAX | 23762.1| 0.5   | 16338.4 | 5.646e+08      | 0.0354  | 821.5 | 826.6  |
