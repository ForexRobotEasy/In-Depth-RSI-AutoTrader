# RSI AutoTrader ReadMe

## Developer Information
- Developer: Forex Robot Easy Team
- Developer's site: [forexroboteasy.com](https://forexroboteasy.com/)

## Description
The RSI AutoTrader is a forex trading software based on the RSI indicator. It is designed to automatically execute buy and sell orders based on the RSI crossing certain levels. The software also has the option to close positions when the RSI crosses back below an overbought level or above an oversold level.

## Installation and Setup
1. Include the necessary libraries: `Trade.mqh` and `RSI.mqh`.
2. Initialize the `CTrade` and `CRSI` objects.
3. Set the desired overbought and oversold levels.
4. Customize other settings if desired.
5. Call the `OnStart()` function to start the trading process.

## Customizable Settings
- `customOverboughtLevel`: Set a custom overbought level (default: 70).
- `customOversoldLevel`: Set a custom oversold level (default: 30).
- `enableCloseAtOverbought`: Enable/disable closing positions when RSI crosses below overbought level (default: true).
- `enableCloseAtOversold`: Enable/disable closing positions when RSI crosses above oversold level (default: true).

## How It Works
1. The software will loop through each bar in the price chart.
2. It calculates the current RSI value using the `rsi.iRSI()` function.
3. If the RSI crosses above the overbought level and the RSI in the previous bar was below the overbought level, a buy position is opened.
4. If the RSI crosses below the oversold level and the RSI in the previous bar was above the oversold level, a sell position is opened.
5. If the 'close at overbought' option is enabled and the RSI crosses below the overbought level, all buy positions are closed.
6. If the 'close at oversold' option is enabled and the RSI crosses above the oversold level, all sell positions are closed.

## Product Description
The RSI AutoTrader is a powerful and fully automated forex trading software that is based on the popular RSI indicator. It allows traders to take advantage of overbought and oversold conditions in the market to execute buy and sell orders automatically.

With customizable settings for overbought and oversold levels, as well as options to close positions when the RSI crosses back below overbought or above oversold levels, the RSI AutoTrader offers flexibility and control to traders.

This software has been developed by the Forex Robot Easy Team, a reputable and experienced team in the forex trading industry. However, please note that ForexRobotEasy is not the official developer of this product. We are showcasing a sample code that can work as described in the product.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/in-depth-rsi-autotrader-review-zenkens-new-forex-ea/). To find the official developer of this product, please refer to MQL5.
