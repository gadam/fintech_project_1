# Cryptocurrency Analysis and Forecast

Our project is to explore the correlations between the cryptocurrency market and traditional finance markets, through looking at indicators including the S&P 500, United States interest rates and gold prices. Furthermore, through the use of *Meta’s Prophet API*, we have forecasted price changes in a selection of cryptocurrencies and compared the result to the actual price change over a 60-day period. 

For the collection of our cryptocurrency and commodities data, we utilised the *Yahoo Finance API* which allowed us to pull historical daily closing prices for our selected tickers. Additionally, we retrieved economic data using the *Federal Reserve Bank of St Louis (FRED) API*. From here we gathered data on the S&P 500, interest rates, GDP, and CPI.

Once we successfully retrieved and cleaned our data, we built a data frame of the cryptocurrencies using the *Pandas library*, and started comparing it to the economic data to check for any correlations. We were surprised to see a near perfect positive correlation with the S&P 500, and a lower-than-expected positive correlation with Gold. 

After looking at the correlations, we calculated the daily change percentages for the cryptocurrencies to look at which provided investors with the highest returns, as well as looking at the distribution of returns to see a visual representation of volatility of each asset. 

Finally, we utilised the *Meta Prophet API* to forecast prices directly from the data we had, for the next 2 months of price movement. After testing different lengths of time to forecast for, due to the volatility of the cryptocurrency market we decided to use 2 months. We split the data frame to feed the API data up until 2 months ago, so we can compare what actually happened to the results of the forecast. 



# Acknowledgments
- [Pandas Library](https://pandas.pydata.org/docs/)
- [YFinance API](https://pypi.org/project/yfinance/)
- [Meta Prophet API](https://facebook.github.io/prophet/)
- [hvPlot Library](https://hvplot.holoviz.org/user_guide/)