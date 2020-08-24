## Fetching-Financial-Data

This repository includes a number of libraries and short examples to demonstrate how we can pull financial data(mostly for equities). It's basically everything you need to get that financial data and start performing analysis/building algorithms on top of that.

Seperate notebook for each different library has been included - 

1. [yfinance](https://github.com/ranaroussi/yfinance) - uses a RESTful API to connect to Yahoo Finance and pull the required data.
2. [yahoofinances](https://github.com/JECSand/yahoofinancials) - uses web scraping to pull data from Yahoo Finance, therefore can be slow when compared to yfinance. Also, we cannot get intraday data using this library(in yfinance, we can).
3. [alphavantage](https://github.com/RomelTorres/alpha_vantage) - Requires an API key(free), this is an amazing option to fetch intraday data, yfinance can also do this, but this is another alternative in case yfinance stops supporting that.

Get Your API Key here - https://www.alphavantage.co/support/#api-key

4. financial-data-webscraping - To scrape financial data such as Balance sheets, income statements and cashflow statements for fundamental analysis using BeautifulSoup.
5. [FundamentalAnalysis](https://github.com/JerBouma/FundamentalAnalysis) - Amazing library, does all the heavy-lifting for you, and does all the magic behind the scenes, to get you the data in a clean format, however this can be used only for a handful of stock exchanges(shown in notebook), if you are looking at stocks in the US, you just have the perfect tool for the task. This also required an API key, and remember that you can make only 250 Calls per API key, so you either need to upgrade or get multiple API keys. Amazing package, shout out to Jeroen Bouma.

Get your API Key here - https://financialmodelingprep.com/developer/docs/


### Why am I demonstrating multiple libraries ?

We never know which one goes out of support, at what time. For example, pandas datareader used to be the most popular choice once, but it stopped supporting Yahoo finance API, therefore, it became outdated.

### My Recommendation

* I personally prefer yfinance for technical analysis, because it has an easy-to-use API and very convenient most of the times.

* For Fundamental analysis, FundamentalAnalysis package is the best, as it requires no data cleaning and can be used directly to get detailed financial statements of a company, however it has coverage limitations and doesn't cover a lot many stock exchanges, so you can choose between Web Scraping and FundamentalAnalysis package as per your requirement.
