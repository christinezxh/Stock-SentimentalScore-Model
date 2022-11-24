# Stock and SentimentalScore Association

## Introduction
In order to understand how stock/market related articles could influence the daily return and market move. Specifically, we manage to explore if there’s an association, or even casual relationship between the sentimental scores of the articles and the daily return/market move of **SE and DOCU** by <u>training simple/multiple linear regression models, logistic regression, decision tree, and random forest. <u>

The data we decided to use are scraped from www. finance.yahoo.com, as Yahoo Finance generally update the market-sensitivity related articles frequently. With selenium package and the designed parsing script of finance.yahoo.com, **119 articles** were downloaded successfully into pandas DataFrame. 

**Average, maximum, and minimum sentimental scores** are calculated on both sentence and paragraph level; in the end, the sentimental scores of both title and the whole article are calculated and stored into the DataFrame. The historical closing data and the Daily Return are downloaded and calculated from Yahoo Finance historical data. Specifically, Daily Return with one day lag is calculated because sometimes it might take a day or so for the market to reflect any changes discussed in the articles. Market Move and Market Move with one day lag are based on daily return/daily return lag, with 1 being market moving upward and 0 otherwise.


Copyright: This project is not intended for public use, it is done for River Tuolumne Capital.
