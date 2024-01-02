# The Renegade EA ReadMe File

The Renegade EA is a forex trading robot developed by the Forex Robot Easy Team. It is designed to automate trading operations on the MetaTrader 5 platform.

For detailed reviews and trading results of this product, please visit the official website: [Renegade EA Review](https://forexroboteasy.com/forex-robot-review/renegade-ea-review-top-forex-software-for-audusd-m5-chart/)

**Disclaimer:** ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Global Variables

- `LotSize`: Initial lot size for trading
- `StopLoss`: Stop loss in pips
- `TakeProfit`: Take profit in pips
- `MagicNumber`: Magic number for trade identification

## Expert Advisor Start Function

The `OnTick()` function is the entry point for the expert advisor. This function is called on every tick of the market. The trading logic should be implemented within this function.

Example Trading Logic:
1. Check if trading is allowed by calling the `IsTradeAllowed()` function.
2. Get the current price using the `SymbolInfoDouble()` function.
3. Open a buy trade if the current price is above the previous candle's high.
4. Open a sell trade if the current price is below the previous candle's low.

## Check if Trade is Allowed

The `IsTradeAllowed()` function is used to check if trading is allowed based on certain trade restriction logic.

Example Trade Restriction Logic:
- Check if the 'Time Travel EA' is enabled.
- Apply additional trade restrictions based on the 'Time Travel EA'.
- Return `false` if trade is not allowed.
- Return `true` if trade is allowed.

**Note:** The code provided is a sample and should be customized based on individual trading strategies and requirements.

For more information on using the Renegade EA, please refer to the official documentation and contact the official developer through MQL5.
