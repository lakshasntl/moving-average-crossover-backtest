
# Moving Average Crossover Backtest – NVDA

### Project Overview

This project implements and evaluates a simple **moving average crossover strategy** on **Nvidia (NVDA)** stock using Python. The goal is to assess how a rule-based trading approach compares to a passive "buy-and-hold" investment over the period from 2015 to 2024.

---

### Strategy Logic

The **Moving Average Crossover Strategy** generates trading signals based on the relationship between two moving averages:

* **Short-Term MA**: 50-day moving average
* **Long-Term MA**: 200-day moving average

**Buy Signal**: When the 50-day MA crosses above the 200-day MA
**Sell Signal**: When the 50-day MA crosses below the 200-day MA

---

### Tools & Technologies

* Python (Jupyter Notebook)
* `pandas`, `numpy` – data manipulation
* `yfinance` – stock data retrieval
* `matplotlib`, `seaborn` – visualizations

---

### Data Source

* **Ticker**: NVDA (Nvidia Corporation)
* **Date Range**: January 2015 – December 2024
* **Source**: Yahoo Finance via `yfinance` package
* **Auto-adjusted prices** to account for stock splits and dividends

---

### Performance Evaluation

| Metric           | Strategy | Buy & Hold |
| ---------------- | -------- | ---------- |
| **Total Return** | `26110.30%` | `28357.38%`   |
| **Sharpe Ratio** | `1.54`  | `1.41`    |

---

### Interpretation
Both the strategy and a buy-and-hold approach delivered exceptional returns on NVDA from 2015 to 2024, reflecting the company's explosive long-term growth. While buy-and-hold slightly outperformed in total return, the moving average crossover strategy achieved comparable gains with the added benefit of potentially reduced exposure during market downturns. This demonstrated how simple rule-based signals can track performance while offering a more controlled risk profile. 

---

### Visuals Included
* Equity curve: Strategy vs. Buy & Hold
* Buy/Sell signal plot with price + moving averages
* Distribution of daily returns

---

### Key Takeaways

* Backtesting provides a data-driven way to evaluate trading logic
* Strategy success depends on market conditions (e.g., trending vs. volatile)
* Even simple strategies can yield insights into market behavior and timing

---

### Next Steps

* Test on other tickers (e.g., SPY, TSLA, MSFT)
* Try different MA window combinations (e.g., 10/50 or 20/100)
* Add more metrics: max drawdown, trade count, win rate
* Build a Streamlit app to interactively visualize strategy performance
