# Day-night-trading-strategy
It explains the day night trading strategy and uses jupyter notebook to validate the same and draw important conclusions from the same. Uses apple and Amazon stock for validating the conclusion.
What is day-night Trading and Why it works?
`Day-Night trading strategy basically refers to buying stocks when the stock market are about to close and selling in on the next day. The strategy takes advantage of the overnight price fluctuations and generate profit from that.
Investors are known to overreact to unexpected events and price moves. This overreaction may lead to mispricing which can then be taken advantage of by initiating a trade in the opposite direction.

It is found that returns increased with the magnitude of event day loss, consistent with the overreaction hypothesis. And they found that reversals were higher for stocks without accompanying news releases, consistent with previous behavioral models.
Whenever a stock lost more than 10% from the intraday, hypothetical buy trades were placed in the last 15 minutes of the trading session and the trades were closed at five-minute increments the following day, from 9:35 am through 4:00 pm.

It is found that returns were strongest during the first five minutes of the trading day and gains tailed off towards the end of the session.
This information is based on the paper Large Price Declines, News, Liquidity, and Trading Strategies: An Intraday Analysis, from Fehle and Volodymyr.



How can we improve day night
Generally large one-day losses often lead to significant reversals overnight. Returns from the strategy increase with capitalization and that returns are highest when there is no significant news story to accompany the loss. The highest gains may come from opening the trade on the close and exiting the trade at the next day’s open.
Taking other news relating to the industry should be taken into consideration.


Model
In the model created in Jupyter notebook. Two stocks are taken Amazon and Apple and their historical prices are taken from - 1 of January 2011   to   31  December 2019.
1.The model first calculates the:
•	Returns_n =Night returns (closing price of previous day – opening price of today) 
•	Returns_d =daily returns (Close-Open).  
•	100 dollars are invested in the stock and NASDAQ index.
Theory 1:   Whenever the daily return of stock is negative, that day we invest the whole sum before the closing that day and sell on the following day open price.  Based on the assumption that stock usually opens at a high price and on the day when there is negative return, there would be a positive reversal at night.
Theory 2:    It buys the stock before the closing each day and sells it on next day opening.
•	NASDAQ on other hand calculates the daily return.
Observation: It is observed that that AMAZON stock using our model, made a profit of around 334% while comparing that with index NASAQ daily return which gives a return of around 50% from Theory 1.
While from Theory 2 there is a 900% profit.
The increase in APPLE stock using our model is nearly same as compared to index.
While from Theory 2 the profit comes out to be 800 %.

Note: The brokerage is not taken into consideration, because the no of transaction comes around 1097 and taking brokerage into consideration we get negligible return from the day- night transaction.


2. The model also calculates further how much the stock price has risen throughout the day as compared to during the night.
•	Calculating the monthly sum of the night return during that month and monthly sum of daily return of stock.
•	Just to get a better understanding and comparison of stock prices changes during day and night we assume that stock price is 100 dollars at the start.
•	Then the changes in prices gives us the rise in stock price due to night and day respectively.
Note: The brokerage is not taken into consideration.

Observation: It is observed that the stock increased around 10 times during the night while during the day there was comparatively no increase.  Thus, the rise in stock prices of amazon is all during the night and negligible during the day.



RESULT
Thus it can be safely assumed that the rise in amazon stock price from 181 to 1874  dollar is all during the night while there is comparatively no increase during the day. The rise in stock price mostly due to night is an important conclusion.
The same conclusions comes out for apple stock where the rise in stock price from 7 to 72 dollars is all during the night
Thus, the day- night strategy works, but when the transaction cost is taken into consideration the profit is negligible which is a setback of this theory.
Other thesis papers also agrees with the above said theory:
Decomposing returns into day (open to close) and night (close to open) returns, it has been found that the US equity premium (as measured by the S&P 500) over the last decade is solely due to overnight returns. The equity premium in the adjacent open to close (daytime) period is zero or even negative, a puzzling finding that implies no reward for bearing risk in daytime volatility. Specifically, for the individual stocks in the S&P 500 index from 1993 to 2006, we find that the average night returns (depending on how we estimate average returns: trade prices versus midquote methods, cross-sectional versus pooled averaging) range from 2.82 basis points (t-statistic = 3.86) to 4.76 basis points (t-statistic = 17.83); day returns range from -2.85 basis points (tstatistic = -6.02) to 0.22 basis points (t-statistic = 0.16); and the difference in returns between night and day (i.e., the night minus day return spread) ranges from 2.61 basis points (t-statistic = 1 For example, daytime rate of information flow is estimated to be seven times that of the overnight rate (George and Hwang (2001). 2 See, for example, French and Roll (1986), Jones, Kaul and Lipson (1994), George and Hwang (2001), and Ronen (1997). 3 1.74) to 7.61 basis points (t-statistic = 11.86).










