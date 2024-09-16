# Introduction
This code is designed to perform a comprehensive analysis of stock pair trading using the Augmented Engel-Granger two-step cointegration test and the Augmented Dickey Fuller test. The analysis involves downloading historical stock prices, calculating returns, identifying highly correlated stock pairs, and implementing a trading strategy based on the spread of returns.

# Code Structure
The code is divided into several sections:

- **Data Preparation:** Downloads historical stock prices for a list of tickers using the yfinance library, calculates returns, and drops any dates with NaN values.
- **Correlation Analysis:** Calculates the correlation matrix of returns and identifies pairs with high correlation values (> 0.9).
- **Stock Pair Selection:** Selects two stocks (MA and V) for further analysis.
- **Augmented Engel-Granger Two-Step Cointegration Test:** Performs the cointegration test to determine if the two stocks are cointegrated.
- **Augmented Dickey Fuller Test:** Performs the ADF test to determine if the spread of returns is stationary.
- **Trading Strategy:** Implements a trading strategy based on the spread of returns, using z-scores to identify buy and sell signals.
- **Visualization:** Plots the spread of returns, z-scores, and trading signals for both stocks.

# Libraries Used
- `numpy` 
- `pandas`
- `matplotlib.pyplot`
- `yfinance` 
- `seaborn`
- `statsmodels.tsa.stattools`

# Output
The code generates several plots and prints the results of the cointegration and ADF tests. The plots include:

- The spread of returns for the selected stock pair
- Z-score values for the spread of returns
- Trading signals (buy and sell) for both stocks
- Historical prices for both stocks with trading signals marked

# Note
This code is for educational purposes only and should not be used for actual trading decisions without further testing and validation.
