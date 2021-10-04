Group members:
Toby
Satoru
Hao

Backtesting with Python 

The main goal of our project is to select known trading strategies and use backtesting or order to compare them against one another, and find whether one is more superior than the others, or whether one strategy works best for one stock etc. 

3 key strategies 
    Moving averages - Toby
    RSI - Hao
    MACD - Satoru 

Which of these strateiges is the most successful? 
And if it's dependant on stocks, which strategy works best for which stock?

pip install pandas-datareader
import pandas_datareader as pdr
asx200 = pdr.get_data_yahoo("ticker")


Compare to each other using backtesting 


Potential stocks
Google
Hut8
Bank of America