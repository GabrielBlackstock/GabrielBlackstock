# README: RSI Signal Strategy with Backtrader

## Overview

This document explains the implementation and results of a Relative Strength Index (RSI) Signal strategy using the Backtrader framework for backtesting on stock data. The strategy, performance metrics, and specific results are detailed below.

## Strategy Description

The RSI Signal strategy is based on the Relative Strength Index (RSI) indicator, which is commonly used in technical analysis to identify overbought or oversold conditions in an asset. In this implementation, we use the RSI to generate buy signals when the RSI falls below a certain threshold (oversold) and sell signals when it rises above another threshold (overbought). We apply this strategy to Tesla (TSLA), a volatile stock known for its price fluctuations.

## Relative Strength Index (RSI)

The RSI is a momentum oscillator that measures the speed and change of price movements. It ranges from 0 to 100 and is typically used to identify overbought or oversold conditions in an asset.

## RSI Signal Strategy

The RSI Signal strategy involves buying when the RSI falls below a specified threshold (oversold) and selling when it rises above another threshold (overbought). This strategy aims to capitalize on short-term price movements based on RSI signals.

## Results

- Sharpe Ratio: 0.67
- Number of Transactions: 13
- Initial Portfolio Value: $1,000,000.00
- Final Portfolio Value: $4,103,519.15
- Return on Investment (ROI): 310.35%

## Interpretation of Sharpe Ratio

The Sharpe Ratio measures the risk-adjusted return of an investment. In this context:

- A Sharpe ratio of 0.67 is considered sub-optimal, as it is below 1.0, indicating that the returns are not sufficient to justify the risk taken.

## Conclusion

The RSI Signal strategy implemented in this backtest demonstrates a potent approach to trading Tesla (TSLA), with substantial returns. However, the sub-optimal Sharpe Ratio suggests that further refinement of the strategy may be necessary to improve risk-adjusted returns.
It is essential to remember that past performance is not indicative of future results, and this strategy should be tested in different conditions and assets to ensure its robustness.
