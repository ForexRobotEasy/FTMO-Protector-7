# FTMO Protector 7 ReadMe File

## Product Description

This code is for the FTMO Protector 7 Expert Advisor, developed by the Forex Robot Easy Team. The FTMO Protector 7 is designed to safeguard forex trades by implementing a maximum daily loss limit. The Expert Advisor continuously monitors the daily profit/loss and closes all trades and disables further trading if the maximum daily loss is reached.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - FTMO Protector 7 Review](https://forexroboteasy.com/forex-robot-review/ftmo-protector-7-review-safeguard-your-forex-trades/). Please note that ForexRobotEasy is not the official developer of this product; we are only providing a sample code that can work as described in this product. To find the official developer of this product, please refer to MQL5.

## Input Parameters

- MaxDailyLoss: Maximum daily loss in account currency. Default value is set to 100.0.

## Global Variables

- g_MidnightBalance: Holds the balance at midnight.
- g_CurrentBalance: Holds the current balance.
- g_DailyProfitLoss: Holds the daily profit/loss.

## Expert Advisor Start Function

The OnTick() function is the entry point for the Expert Advisor. It performs the following tasks:

1. Calculates the midnight balance at 01:00 system time.
2. Calculates the real-time daily profit/loss.
3. Checks if the target profit/loss is achieved.
4. Disables all Expert Advisors and closes all trades and orders if the maximum daily loss is reached.
5. Executes your trading logic (to be implemented by the user).

## Calculate Midnight Balance Function

The CalculateMidnightBalance() function calculates the balance at midnight by retrieving the account equity.

## Calculate Daily Profit/Loss Function

The CalculateDailyProfitLoss() function calculates the daily profit/loss by subtracting the midnight balance from the current balance.

## Disable Expert Advisors Function

The DisableEAs() function disables all Expert Advisors by removing them from the chart.

## Close All Deals and Orders Function

The CloseAllDealsAndOrders() function closes all open trades and orders by iterating through each position and calling the OrderClose() function.

Please note that this code serves as a sample and should be customized to fit your specific trading strategy and requirements.

For more information about the FTMO Protector 7 Expert Advisor, please visit [Forex Robot Easy - FTMO Protector 7 Review](https://forexroboteasy.com/forex-robot-review/ftmo-protector-7-review-safeguard-your-forex-trades/).
