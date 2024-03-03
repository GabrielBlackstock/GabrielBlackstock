# Bullish Engulfing Candle Pattern Detection in XBTUSDTM Trading

This repository contains a Python script that identifies bullish engulfing candle patterns in the trading data of XBTUSDTM, which is a symbol for Bitcoin (BTC) traded against Tether (USDT) in the futures market. BTC is a significant cryptocurrency that often dictates the broader market movements.

## Engulfing Candle Pattern

An engulfing candle pattern is a type of reversal pattern seen on candlestick charts, typically at the end of a downtrend. A bullish engulfing pattern occurs when a smaller red (or black) candle is followed by a larger green (or white) candle, where the body of the latter completely engulfs the body of the former. This pattern indicates a potential reversal from bearish to bullish sentiment.

## Script Overview

The script uses the `ccxt` library to connect to the Kucoin Futures API and fetches the OHLCV (Open, High, Low, Close, Volume) data for the XBTUSDTM symbol. It then processes this data to identify potential buy signals based on the bullish engulfing pattern and additional conditions.

### Key Features:

- **Data Retrieval:** Fetches historical OHLCV data for XBTUSDTM from Kucoin Futures.
- **Engulfing Pattern Detection:** Identifies bullish engulfing patterns using a custom function that analyses daily price movements.
- **Buy Signal Generation:** Generates buy signals not only based on the engulfing pattern but also checks if the closing price is at least 4% higher than the opening price to catch significant bullish momentum. Additionally, it ensures that the price and volume two days prior were positive, adding another layer of confirmation to the signal.
- **Visualisation:** Utilises `mplfinance` to plot the candlestick chart, highlighting the buy signals with green arrows.

### Usage:

1. Install the necessary Python libraries: pandas, numpy, mplfinance, ccxt, and matplotlib.
2. Ensure you have valid API credentials for Kucoin Futures.
3. Run the script to analyse the data and visualise the buy signals.

## Interpretation

The script is designed to assist traders and analysts in identifying potential buying opportunities based on historical data. However, it's crucial to combine these signals with other forms of analysis and not rely solely on one indicator.

## Customisation

Users can modify the script to adjust the parameters, such as the percentage difference between the open and close prices or the timeframe of the data, to fit their trading strategy or analysis needs.

## Disclaimer

The script is for educational and analytical purposes only. Always conduct your due diligence and consult with a financial adviser before making trading decisions.

