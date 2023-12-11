# Financial_Portfolio

In this post, I will talk about the two portfolio comparison project I wrote. My goal is to be useful to those who develop software about financial markets. The libraries I use in the code are yfinance, pandas and matplotlib respectively.

First, let's start with the first code. This Python code is used to compare the performance of a specific portfolio (We call it Bayford Commodity Portfolio) and the GSCI Index over a specific period.

Using the yfinance library, I pulled historical data of specific stocks and the GSCI Index. I used this data to create a portfolio that included the average of the closing prices of stocks over a specific period. Then, I calculated the return of both the GSCI Index and the portfolio created exactly 1 year ago to date. Then, I normalized these two portfolio data so that we could see the difference more easily when we visualized them. Normalizing does not change the result, but it does change how easily we can see the result on the graph. Therefore, especially if the chart is long-term, it is much easier to make comparisons as the price change is larger. Finally, I took help from the matplotlib library to visualize these two returns.

Now there is the second code. This code, like the other one, shows the difference between portfolios.

Both codes compare the performance of a particular portfolio and the GSCI Index. However, these codes use different calculation methods, which leads to different results. In the first code, portfolio return is calculated as the average of closing prices of stocks over a given period. This assumes each stock has equal weight in the portfolio. In the second code, the portfolio return is calculated as the average of the daily return (percentage change) of each stock. This assumes that each stock has a certain weight in the portfolio. These weights are often based on an investment strategy or risk tolerance. These two different calculation methods represent different investment strategies and risk tolerances and therefore produce different results. The first method represents an investment strategy in which all stocks are equally important, while the second method represents an investment strategy that gives greater weight to certain stocks.

I hope these projects will help those who want to develop portfolio management software at the entry level.
