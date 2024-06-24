# Airline-Passenger-Forecasting

![Airline Logo](https://example.com/path/to/airline-logo.png)
![Forecasting Logo](https://example.com/path/to/forecasting-logo.png)

This repository contains a time series analysis and forecasting project for airline passenger data using the ARIMA (AutoRegressive Integrated Moving Average) model. The steps include data preprocessing, stationarity testing, ADF (Augmented Dickey-Fuller) test, plotting ACF (AutoCorrelation Function) and PACF (Partial AutoCorrelation Function), fitting an ARIMA model, forecasting future values, and evaluating the model using RMSE (Root Mean Squared Error).

## Project Structure

- `airline-passenger-forecasting.ipynb`: The Jupyter Notebook containing the entire code for data analysis, preprocessing, stationarity testing, ARIMA model fitting, forecasting, and evaluation.

## Data

The dataset used in this project is the monthly number of international airline passengers from January 1949 to December 1960. The data is sourced from [this CSV file](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv).

## Steps Performed

1. **Data Loading and Preprocessing**
   - Load the dataset using pandas.
   - Log transform the data to stabilize variance.

2. **Stationarity Testing**
   - Split the data into two halves and calculate the mean and variance for each half.
   - Perform the Augmented Dickey-Fuller (ADF) test to check for stationarity.

3. **Autocorrelation and Partial Autocorrelation Plots**
   - Plot ACF and PACF plots to determine the order of AR and MA terms for the ARIMA model.

4. **ARIMA Model Fitting**
   - Fit an ARIMA model with the specified (p,d,q) order.
   - Forecast the next 12 months' values using the fitted model.

5. **Model Evaluation**
   - Calculate the RMSE of the forecasted values.
   - Plot the original and forecasted values for comparison.


## How to Use

1. Clone this repository.
2. Ensure you have the necessary dependencies installed.
3. Open the `airline-passenger-forecasting.ipynb` file in Jupyter Notebook.
4. Run the notebook cells to perform the analysis and forecasting.

## Conclusion

This project demonstrates the process of time series analysis and forecasting using the ARIMA model. It highlights the importance of data preprocessing, stationarity testing, and model evaluation in building an effective forecasting model.
