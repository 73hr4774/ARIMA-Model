# Temperature Forecasting using SARIMA

This project demonstrates temperature forecasting using the SARIMA (Seasonal Autoregressive Integrated Moving Average) model in Python. It utilizes a time series dataset of hourly temperature readings and aims to predict future temperature values.

## Dataset

The dataset used in this project contains hourly temperature data and is stored in the file `temperature-1.csv`. It includes the following columns:

- **Unnamed: 0:** Index column.
- **Datetime:** Timestamp of the temperature reading.
- **Hourly_Temp:** Hourly temperature value.

## Methodology

1. **Data Loading and Preprocessing:** The dataset is loaded using Pandas, and the 'Datetime' column is converted to a datetime object. The 'Unnamed: 0' column is dropped, and 'Datetime' is set as the index.
2. **Data Visualization:** The hourly temperature data is visualized using Matplotlib to understand its patterns and trends.
3. **Stationarity Check:** The Augmented Dickey-Fuller test is used to check the stationarity of the time series data. If the data is not stationary, differencing is applied to make it stationary.
4. **SARIMA Model:** A SARIMA model is fitted to the data, considering the order of autoregressive (AR), integrated (I), and moving average (MA) components, as well as seasonal components.
5. **Forecasting:** The fitted SARIMA model is used to forecast future temperature values for a specified number of steps.
6. **Forecast Evaluation:** The forecasted values are compared to the actual values to assess the model's performance.

## Results

The project provides a forecast of hourly temperatures for the next 24 hours. The forecasted values are presented along with a 95% confidence interval. A plot is generated to visualize the original data, the forecast, and the confidence interval.

## Dependencies

- Python 3
- Pandas
- NumPy
- Matplotlib
- Statsmodels

## Usage

1. Clone the repository: `git clone <repository_url>`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the Jupyter notebook: `jupyter notebook temperature_forecasting.ipynb`

## Contributing

Contributions to this project are welcome. Please follow the standard GitHub workflow for submitting pull requests.

## License

This project is licensed under the MIT License.
