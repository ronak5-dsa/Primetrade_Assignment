# Trader Behavior Analysis Based on Bitcoin Market Sentiment
## Objective
The objective of this project is to analyze how Bitcoin market sentiment influences trader performance. By combining the Fear & Greed Index with Hyperliquid trading data, the analysis aims to identify patterns in profitability, win rates, and trading behavior under different market conditions.

## Datasets Used

### 1. Bitcoin Fear & Greed Index Dataset

* Date
* Sentiment Score
* Sentiment Classification (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

### 2. Hyperliquid Historical Trader Dataset

* Account
* Coin
* Trade Direction
* Trade Size
* Execution Price
* Closed PnL
* Timestamp

## Methodology

1. Cleaned and standardized date formats across both datasets.
2. Extracted trading dates from timestamp records.
3. Merged trading activity with daily market sentiment data.
4. Performed exploratory data analysis on profitability and trading outcomes.
5. Compared BUY and SELL performance across sentiment categories.
6. Analyzed win rates and trader profitability distributions.


## Key Findings

### 1. Market Sentiment Influences Profitability

Average trader profitability varied significantly across market conditions.

| Sentiment     | Average Closed PnL |
| ------------- | -----------------: |
| Extreme Greed |              67.89 |
| Fear          |              54.29 |
| Greed         |              42.74 |
| Extreme Fear  |              34.54 |
| Neutral       |              34.31 |

Traders achieved the highest average profit during Extreme Greed periods, suggesting that strong bullish sentiment creates favorable trading opportunities.

### 2. Fear Periods Generated the Highest Total Profit

Although Extreme Greed produced the highest average profit per trade, Fear periods generated the highest cumulative profit due to significantly higher trading activity.

This indicates that traders tend to participate more actively during uncertain market conditions.


### 3. Win Rates Improve in Bullish Markets

| Sentiment     | Win Rate (%) |
| ------------- | -----------: |
| Extreme Greed |        46.49 |
| Fear          |        42.08 |
| Neutral       |        39.70 |
| Greed         |        38.48 |
| Extreme Fear  |        37.06 |

Trades executed during Extreme Greed periods had the highest probability of being profitable, while Extreme Fear periods recorded the lowest win rates.


### 4. Buy and Sell Strategies Behave Differently

The relationship between sentiment and trade direction revealed an interesting pattern.

* BUY trades performed best during Fear periods.
* SELL trades outperformed BUY trades during Greed and Extreme Greed periods.
* The highest average profit was observed for SELL trades during Extreme Greed.

This suggests that buying during pessimistic conditions and selling during optimistic conditions was generally more profitable within this dataset.


### 5. Profitability Is Highly Concentrated

The most profitable trader generated more than 2.1 million in realized profit, while several others earned profits exceeding one million.

This indicates that trading success is not evenly distributed and that a relatively small number of traders contribute a large share of overall profits.


## Conclusion

The analysis demonstrates a clear relationship between market sentiment and trader performance. Extreme Greed periods were associated with the highest average profitability and win rates, while Fear periods generated the greatest overall trading activity and cumulative profits.

The findings also suggest that contrarian behavior—buying during fearful periods and selling during greedy periods—was associated with stronger trading outcomes. These insights may help traders better understand how market psychology influences trading performance and decision-making.
