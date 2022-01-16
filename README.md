# algo-trading-backtester

The goal of this project was to implement machine learning models and backtesting algorithms in a Google Colab notebook to find the optimal algorithmic trading strategy between a machine learning model and a simple moving average (SMA) crossover strategy for any stock or crypto asset. We first determined the optimal SMA window pairs that would provide the highest net profit and/or Sharpe ratio for a SMA crossover algorithmic trading strategy by backtesting a variety of moving average window pairs using Gridsearch from sci-kit learn. We then compared the results of this backtest to a machine learning SVM model to see which outperformed the other, if any.

## Technologies

This project leverages Python 3.7 in Google Colab with the following libraries:
- pystan
- fbprophet
- hvplot
- holoviews
- fastquant
- streamlit
- sklearn
- pandas
- numpy
- matplotlib

## Installation Guide

To use this notebook, simply open the Google Colab notebook and run the notebook. The required installations should be listed in the first cell of the notebook. Simply run the cell to install the required libraries.

## Usage

To use this notebook, simply run the cells in order. This notebook allows for various user customizations pertaining to the asset of choice and the time period to run the backtest analysis. If you would like to customize these features, feel free to adjust the arguments in the first cell after the import.

The original line of code is listed as:

```
price_df = get_stock_data('TSLA', '2018-01-01', '2021-12-31')
```

Users may choose any stock or crypto as well as any time period. The date format must be in YYYY-MM-DD. To choose a crypto, the function get_stock_data must be replaced with get_crypto_data.

## Contirbutors
Austin Do (austindotech@gmail.com), Nev Douglas, Kanika Sharma (ksharmaconnect3@gmail.com), Jason Muenzen (jmuenzen@gmail.com), Max Gregory (maximillian.gregory@gmail.com)


## License

MIT
