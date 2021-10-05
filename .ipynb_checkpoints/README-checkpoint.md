# Awesome_Group
Backtesting with Python 

At the end of the day, investors and traders are here to make money and people claim all the time that they can beat the market. 
Our goal was to find out whether we could optimise our profits in a way that was considerably better than just buying and holding those assets over the same period. 

We did this by selecting three popular and well documented trading strategies and using backtesting with financial data in order to compare them against one another, find whether one is more superior than the others, or whether one strategy works best for one stock compared to another.

We decided to focus on the period of time before, during and after the Global Financial Crisis of 2008, to work out whther these strategies could have been implemented to either limit losses, or to profit from the crash itself. At the end of our research period, we would compare our results.

To find this out, used pandas datareader to grab historic data from Yahoo finance for 3 stocks from different industries; We chose Apple, Ford and Bank of America. 

Luckily this data was already clean and other than removing NANs from the dataframes after calculating averages, we didn't have to do much else.

The three key strategies we decided to use were simple moving averages, relative strength index, and the moving average convergence divergence.

#Quick Overview of our Strategies

##SMA:
Simple moving average uses constantly updated average price data over a chosed period and then making trades based on when these moving averages cross one another on a chart. We used the 20 day MA and the 50 day MA, a made a buy signal when the 20 moves above the 50 day, and a sell signal when the 20 day moves below the 50 day.

##RSI:
Relative strength index is an oscillating indicator designed to measure a stock's speed and size of price changes over a chosen time period. The average gains divided by average losses over chosen time period gives us the relative strength value. It's then plotted on a graph between 0 and 100. Many traders use this indiactor to determine if a stock is overbought, or oversold, indicating a trend reversal and therefore a buy or sell signal. For example, if a stock has risen rapidly in a short period of time and may reverse lower.

##MACD:
Moving average convergence divergence is a trend-following momentum indicator that shows the relationship between two moving averages of an asset's price. It's calculated by subtracting the 26-period exponential moving average (EMA) from the 12-periof EMA.
This calucatation, when plotted, gives us the MACD line. A 9 day EMA of the MACD is then plotted over the top of the MACD line. This "signal line" then functions as the buy or sell signal. The MACD line reacts to price movements faster than the signal line, so when the MACD crosses above it's signal line it can trigger a buy signal and when it crosses below, a sell signal. 

