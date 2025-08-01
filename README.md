# moving-average-crossover-backtest
This project implements and backtests a simple trading strategy based on moving average crossovers using historical stock price data. The goal is to evaluate how effective this strategy would have been over time and explore its potential risks and rewards.

## Problem Statement
Retail investors often use moving average (MA) indicators to make trading decisions. One popular approach is the Moving Average Crossover Strategy, where a short-term MA crossing above a long-term MA signals a buy, and a downward cross signals a sell.

Can this simple rule-based strategy outperform a passive "buy and hold" approach?

## Tools & Technologies
Python

Pandas – data manipulation

yfinance – to fetch historical stock data

Matplotlib / Seaborn / Plotly – visualization

NumPy – numerical calculations

Jupyter Notebook – interactive exploration

## Strategy Logic
Short-Term MA (e.g., 50-day)

Long-Term MA (e.g., 200-day)

Buy Signal: When short-term MA crosses above long-term MA

Sell Signal: When short-term MA crosses below long-term MA

## Data Used
Source: Yahoo Finance via yfinance

Stock Ticker: (e.g., AAPL, MSFT, SPY — can be changed)

Date Range: Default is past 10 years

## Key Metrics Evaluated
Cumulative Returns

Daily Returns

Volatility

Sharpe Ratio

Maximum Drawdown

Win Rate of Trades

## Sample Visuals (to include)
Equity Curve: Strategy vs Buy & Hold

Signal Plot: Buy/Sell markers on stock price

Histogram of daily returns

Rolling Sharpe ratio

