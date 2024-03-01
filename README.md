# Prop Firm Pass EA

This code is an example of a trading Expert Advisor (EA) for the MetaTrader 4 platform. The EA is designed to implement a breakout strategy based on a specified breakout period and threshold. The code includes necessary libraries and defines trading parameters, breakout strategy parameters, and risk management parameters.

## Trading Parameters

- `lotSize`: The lot size for each trade. Default value is 0.01.

## Breakout Strategy Parameters

- `breakoutPeriod`: The number of periods for breakout calculation. Default value is 20.
- `breakoutThreshold`: The minimum breakout percentage. Default value is 0.001.

## Risk Management Parameters

- `maxDrawdown`: The maximum allowable drawdown percentage. Default value is 0.05.

## Prop Firm Pass EA Class

This code defines a class `PropFirmPassEA` that implements the trading logic for the EA. The class includes a private trade object for executing trades. The constructor sets the expert magic number for the trade object.

The `OnTick()` function is the entry function for the EA. It gets the current price and previous price, calculates the breakout percentage, and opens a buy or sell trade if the breakout percentage exceeds the threshold.

## Initializing and Running the EA

The code creates an instance of the `PropFirmPassEA` class and initializes the EA in the `OnInit()` function. The `OnStart()` function runs the EA on every tick, calling the `OnTick()` function of the `PropFirmPassEA` instance. The EA runs until it is stopped.

## Stopping the EA

The `OnDeinit()` function is called when the EA is stopped. It closes all open trades using the `CloseAll()` function of the trade object.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that can work as described in the product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, please visit [ForexRobotEasy - Prop Firm Pass EA Review](https://forexroboteasy.com/forex-robot-review/prop-firm-pass-ea-review-optimized-forex-software-for-successful-trading/).
