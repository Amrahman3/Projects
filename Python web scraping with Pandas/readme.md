This project is to showcase how to easily extract stock prices from online sources such as Yahoo! Finance. We will be using the stocks table from Wikipedia to isolate the stock tickers for the energy companies in S&P 500 and then use the tickers to extract the data with the yfinance library for further analysis. 

First, I downloaded and install all the required dependencies. 
Next, I used the Pandas reader to extract the table of stocks from Wikipedia, followed by exploration and transformation of the data. 
After isolating the tickers for the energy companies only, I proceeded to read and append the stock prices for a preset date range to the stk_price dataframe. 
After a quick check of the newly appended dataframe, I used Plotly to plot a candlestick chart with moving averages that can be zoomed in and out using the range finder (please ensure to run code in Jupyter notebook). 

Finally, I compiled all of the previous step into a function which can accept 4 parameters: stocks(stock tickers, list datatype), rolling(moving average window, list datatype), start_date(preset start date, datetime datatype), end_date(preset end date, datetime datatype). The function prints out a candlestick chart for the tickers and returns a data table of all the tickers.
