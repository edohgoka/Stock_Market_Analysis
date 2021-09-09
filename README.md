# Stock_Market_Analysis
In this project, we analyze the data of a particular stock (in our case, the **Apple** stock denoted by **AAPL**) and predict its price at the market close. To do this, some steps were taken:
- To start this project, we retrieved the stock data using the `yfinance` library.
- Then we analyzed the data to understand it by performing **EDA** (`plotly`, `pandas`, ...).
- performed Time Series Data processing (**Preparing data for modeling**)
- and built and trained a sequential model on **Tensorflow 2.0** (with recurrent layers `LSTM` and `Bidirectional`)

Some technical indicators have been taken into account when processing the data in order to add more features such as :
- exponential moving average (**EMA**)
- relative strength index (**RSI**)
- moving average convergence / divergence (**MACD**)
- Bollinger bands (**BBANDS**)
- ...

The values of these indicators have been scraped from [alphavantage](https://www.alphavantage.co/) using `requests` and `pandas`.
