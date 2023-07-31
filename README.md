# Bitcoin Price Forecasting

This repository contains a Jupyter Notebook (`Bitcoin_Forecasting.ipynb`) that demonstrates various time series forecasting models to predict the future prices of Bitcoin. The notebook was automatically generated using Google Colaboratory.

## Get Data

The historical price data for Bitcoin has been collected from the CoinDesk API. The data spans approximately 8 years from October 1, 2013, to May 18, 2021, with 2787 samples.

The dataset has the following columns:
- Date: The timestamp of each sample.
- Closing Price (USD): The closing price of Bitcoin in USD on each corresponding date.

## Data Preprocessing

Since our focus is on predicting Bitcoin prices, we extract only the "Closing Price (USD)" column and create a new DataFrame for further analysis.

## Train and Test Split

In time series forecasting, the right way to split the data into train and test sets is to use a chronological split. In this notebook, 80% of the data is used for training, and the last 20% is used for testing.

## Modelling Experiments

We run a series of modelling experiments to determine the best performing model for Bitcoin price prediction. The models include:

0. Naïve model (baseline)
1. Dense model with horizon = 1 and window = 7
2. Dense model with horizon = 1 and window = 30
3. Dense model with horizon = 7 and window = 30
4. Conv1D model
5. LSTM model
6. Dense model with multivariate data
7. N-BEATs algorithm
8. Ensemble of multiple models optimized on different loss functions
9. Future prediction model for Bitcoin prices
10. Dense model with turkey 🦃 data introduced

Each model is evaluated based on its performance in predicting future Bitcoin prices.

## How to Use the Notebook

To use this notebook, simply run each cell sequentially to load the data, visualize the Bitcoin prices, split the data into train and test sets, and then run the modelling experiments. Each section is well-documented with explanations and comments to guide you through the process.

Feel free to experiment with different models, hyperparameters, and data preprocessing techniques to further improve the results.

Please note that this notebook assumes basic knowledge of time series forecasting and machine learning concepts. For a more detailed understanding of the models used, refer to the official documentation of the libraries and algorithms used in this notebook.

If you encounter any issues or have any questions, feel free to reach out to the author.

Happy forecasting!
