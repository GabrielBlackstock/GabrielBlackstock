# README: SMA Crossover Strategy with Backtrader

## Overview
This document explains the implementation and results of a Simple Moving Average (SMA) Crossover strategy using the Backtrader framework for backtesting on cryptocurrency data. The strategy, performance metrics, and specific results are detailed below.

## Strategy Description
The SMA Crossover strategy is a common technical analysis approach used in trading. This strategy involves two lines: the Simple Moving Average (SMA) and the asset's price line. When the asset's price crosses above the SMA, it is considered a buy signal, and when the price crosses below, it is a sell signal.

In this implementation, we use a 50-period SMA on the price data of Bitcoin (BTC-USD). A signal to go long (buy) is generated when the price crosses above the SMA, and the position is closed when the opposite crossover occurs.

## Simple Moving Average (SMA)
The SMA is calculated by averaging the closing prices of an asset over a specified number of periods. In this case, we use a 50-period SMA, meaning the average price over the last 50 periods is used to determine the moving average at each point.

## SMA Crossover
The SMA Crossover occurs when the price line intersects with the SMA line. This intersection indicates a potential change in the asset's momentum and is used to trigger buy or sell signals in our strategy.

## Sharpe Ratio
The Sharpe Ratio is a measure used to evaluate the risk-adjusted return of an investment. It is calculated by subtracting the risk-free rate from the return of the investment and dividing the result by the investment's standard deviation of returns. A higher Sharpe Ratio indicates a more attractive risk-adjusted return.

## Good Sharpe Ratio
A Sharpe Ratio greater than 1 is considered good, indicating that the returns are better than the risk taken. Ratios above 2 are considered very good, and above 3 are excellent. In the context of this backtest, a Sharpe Ratio of 4.50 signifies an excellent risk-adjusted return.

## Results
- **Sharpe Ratio:** 4.5024605835703735
- **Number of Transactions: 17
- **Initial Portfolio Value: $1,000,000
- **Final Portfolio Value: $2,049,970.82
- **Return on Investment (ROI): 105.00%

These results indicate a highly successful backtest, with a significant ROI and an excellent Sharpe Ratio, suggesting that the strategy achieved returns that well-compensated for the risk incurred.

## Conclusion
The SMA Crossover strategy implemented in this backtest demonstrates a potent approach to trading Bitcoin, with substantial returns and a high Sharpe Ratio. It is crucial to remember that past performance is not indicative of future results, and this strategy should be tested in different conditions and assets to ensure its robustness.
