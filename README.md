# Stock News Sentiment
This is the final project for the Foundations of Financial Data Science course at Stevens Institute of Technology. 

## Introduction
Financial news articles can have significant impact on stock prices. However, there are tons of news articles released every day and it is very difficult to keep track of how these articles can impact prices. One simple approach is to look at the sentiment of these articles and try to see if there is a relationship between sentiment and stock returns. 

In this project, I use the Reuters News Database to investigate this relation between the news article sentiment and stock prices. 

# Approach
Reuters News Database aggregates many news articles released from various news outlets and classifies them with respect to the companies that the article refers to and it stores the sentiment for these articles as well. 

I used this database to get company specific news articles, calculated my own sentiment based on the text and aggregated the sentiment daily. This creates a daily time series of sentiment of a given company. Correlation of the daily sentiment time series is compared to daily return of that specific stock. 

The relation between lagged time series is also examined to see if there is some causality between the sentiment and stock returns.

# Example
In this repo, I calculate the correlation of MSFT news sentiment to MSFT stock returns. Sentiment scores are derived from MSFT related articles from the Reuters News database over the period 2010-2012. While the original project was much wider in scope in terms of the number of companies and the number of years examined, the approach taken was similar. 

The results for MSFT indicate that sentiment and returns are not correlated for MSFT or there doesn't seem to be a causation. 


View .md file for the R markdown analysis.
