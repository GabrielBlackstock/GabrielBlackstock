# EMA 12-26 Trend Visualisation Project

## Overview
The EMA 12-26 Trend Visualisation tool is a Python script that provides a graphical representation of cryptocurrency market trends based on the crossover of Exponential Moving Averages (EMAs) over 12 and 26 periods. This project utilises weekly data, which is often favoured by traders seeking stronger and less noisy signals compared to daily data. The visualisation helps identify potential trends which could be used to inform trading strategies.

## Visualisation Details
The script generates a plot with the following elements:
- **Green Dots**: Represent periods where the market is considered to be in an uptrend, identified by the 12-period EMA being above the 26-period EMA.
- **Red Dots**: Indicate a downtrend where the 12-period EMA falls below the 26-period EMA.
- **Yellow Dots**: Occur where there is a crossover and the EMAs are equal, suggesting a neutral or transitioning market.

These colours provide a clear and immediate visual cue for trend direction. The use of EMAs rather than simple moving averages (SMAs) ensures that the signals are more responsive to recent price changes, providing a more current view of market momentum.

## Significance of the 12-26 EMAs
The 12 and 26 period EMAs are significant in trading analysis because they form the basis for the Moving Average Convergence Divergence (MACD), a widely-used momentum indicator in technical analysis. The difference between these two averages can signal potential bullish or bearish momentum and is considered a cornerstone for various trading strategies.

## Usage of Weekly Data
This project specifically utilises weekly OHLCV (open, high, low, close, volume) data to calculate EMAs and generate signals. Weekly data was chosen to filter out the day-to-day market noise and provide stronger signals that are more suited for medium to long-term trend analysis, which can be particularly beneficial for swing traders.

## Running the Script
Ensure you have the `ccxt` library installed to fetch data from Kucoin Futures, and `matplotlib` and `pandas` libraries for data manipulation and visualisation. Update the API details with your credentials before executing the script.

## Conclusion
The EMA 12-26 Trend Visualisation script is a powerful tool for traders who rely on technical analysis to guide their trading decisions. By providing a clear visual representation of the market trend based on reliable EMA indicators, it offers valuable insights into market momentum and potential trend reversals.
