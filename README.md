# Twitter-Sentiment-Based-Investing
This project explores an investing strategy based on Twitter sentiment data to identify and invest in stocks with positive social media engagement. By leveraging sentiment analysis, the aim is to create a portfolio that can potentially outperform traditional market benchmarks.

# Steps Overview
1. Loading Twitter Sentiment Data

First, we load the Twitter sentiment dataset. We set the index, calculate the engagement ratio (which measures the level of social media activity), and filter out stocks that do not have significant Twitter activity. This ensures we focus on stocks with notable social media presence.

2. Aggregate Monthly and Calculate Average Sentiment

Next, we aggregate the data on a monthly level. We calculate the average sentiment for each stock for the month, providing a clearer picture of overall market sentiment towards each stock over time.

3. Select Top 5 Stocks Based on Their Cross-Sectional Ranking

For each month, we rank the stocks based on their sentiment scores and select the top 5 stocks. These rankings help us identify the most positively viewed stocks on social media for each month. We fix the start date for each selected stock to the beginning of the next month.

4. Extract the Stocks to Form Portfolios at the Start of Each New Month

We create a dictionary containing the start of each month and the corresponding selected stocks. This structure helps us organize and manage the selected stocks over time.

5. Download Fresh Stock Prices for Only Selected/Shortlisted Stocks

We then download the latest stock prices for the selected stocks at the start of each new month. This ensures we have up-to-date price information for our portfolio.

6. Calculate Portfolio Returns with Monthly Rebalancing

With the fresh stock prices, we calculate the returns for our portfolio. We rebalance the portfolio at the start of each month based on the newly selected stocks. This monthly rebalancing helps maintain the strategy's alignment with current sentiment trends.

7. Download NASDAQ/QQQ Prices and Calculate Returns to Compare to Our Strategy

Finally, we download the prices for the NASDAQ index or QQQ ETF and calculate their returns. We compare these returns to the returns of our sentiment-based portfolio to evaluate the performance of our strategy.

By following these steps, we can develop an investing strategy that leverages Twitter sentiment to identify and invest in stocks with positive social media engagement, potentially leading to superior returns.
