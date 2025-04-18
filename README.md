
# Stock Price Prediction

This project utilizes Long Short-Term Memory (LSTM) neural networks to predict the future stock closing prices of Axis Bank based on historical data. The model is trained on past prices to learn temporal patterns and then used to forecast upcoming trends.


The notebook implements a multi-layer LSTM architecture for time series forecasting. It uses historical stock price data to train and evaluate the model. The focus is on accurately predicting closing prices using a lookback window of past values.




## Dependencies

To run this notebook, ensure the following packages are installed:

1.numpy

2.pandas

3.matplotlib

4.scikit-learn

5.tensorflow
## Installation

Install my-project with npm

```bash
  git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

```

Install NumPy:

```bash
pip install numpy
```
Install Pandas:

```bash
pip install pandas
```
Install Matplotlib:

```bash
pip install matplotlib
```
Install Scikit-learn:

```bash
pip install scikit-learn
```
Install TensorFlow:

```bash
pip install tensorflow
``` 
## Features

- Time-Series Forecasting using LSTM neural networks
- Configurable lookback window for sequence generation
- Data normalization using MinMaxScaler
- Multi-layer LSTM architecture with Dropout and Batch Normalization
- Evaluation using RMSE, MAE, and R² Score
- Training optimized with EarlyStopping and ReduceLROnPlateau
- Visual comparison of predicted vs actual stock prices
- Modular code structure for easy experimentation and tuning
## Performance Metrics

The model's performance was evaluated using three key regression metrics:

- **RMSE (Root Mean Squared Error):**  
  - Train RMSE: 26.64  
  - Test RMSE: 66.55  
  Indicates how much the predictions deviate from actual values, with higher penalties for larger errors.

- **MAE (Mean Absolute Error):**  
  - Test MAE: 31.06  
  Reflects the average magnitude of prediction errors in the same units as the data.

- **R² Score (Coefficient of Determination):**  
  - Test R² Score: 0.9648  
  Shows that the model explains ~96.5% of the variability in the test data.

These metrics suggest that the LSTM model performs well, generalizing effectively to unseen stock price data.
## Dataset

- **Source:** Manually downloaded or scraped from a stock exchange or financial API (e.g., Yahoo Finance, NSE India)
- **File Name:** `AXISBANK.csv`
- **File Format:** CSV (Comma-Separated Values)

###  Sample Data Preview
| Date       | Open   | High   | Low    | Close  | Volume |
|------------|--------|--------|--------|--------|--------|
| 2022-01-01 | 680.50 | 690.00 | 670.75 | 685.10 | 1234567 |
| 2022-01-02 | 685.10 | 695.25 | 680.00 | 692.75 | 1104321 |
| ...        | ...    | ...    | ...    | ...    | ...     |

> Note: In this project, only the `Close` price is extracted and normalized before feeding into the LSTM model. Other columns (Open, High, Low, Volume) are ignored for simplicity but can be included for model enhancement.

## Authors

- [Madhurya Mishra](https://github.com/madhurya-ops)
- [Chaitanya Bansal](https://github.com/Chai-B)
- [Kanhaiya Sharma](https://github.com/kanhaiyas103)

