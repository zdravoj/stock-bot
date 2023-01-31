# Stock Bot
Automates a combination of trading strategies to maximize returns.

## Purpose
The goal of Stock Bot is to increase or maintain the purchasing power of its financial capital. More specifically, the real rate of return for the overall portfolio should increase with every additional trading or investment strategy incorporated into the bot.

## Restrictions
By definition, Stock Bot is a trader, not an investor. The bot can only utilize financial vehicles which allow it to:

1. Engage and disengage from the vehicle quickly (a purchase or sell must execute within a maximum of one week, and preferably instantly).
2. Restrict its holding time to a maximum of one financial quarter.

Vehicles such as government bonds, real estate, futures contracts, etc. are unacceptable within its scope.

Additionally, the bot must remain risk-averse, and so cannot engage in trades or contracts which carry the potential of unrealized losses, nor those in which the bot must accurately predict the future value of a stock. Specifically, it cannot engage in:

1. Short selling
2. Options contracts

This aversion to risk also requires that any trade, no matter how confident the bot is in its potential profit, cannot place a significant portion of the portfolio at risk of total loss. No individual trade can exceed 10% of the total portfolio value. This value is likely to decrease as additional strategies are incorporated into the bot.

## Overall strategy
Because of its restrictions (both those defined above, and because it is a computer), it can only approach trading algorithmically. The bot does not attempt to maximize the returns of any particular trade, rather, it employs strategies that focus on the returns of groups of trades, where individual trading losses are acceptable (and expected) only when the aggregate losses are outweighed by the aggregate profits.

Some strategies are defined by time, such that the bot makes purchases and holds them for a definite amount of time. These strategies are generally based on the historical upward movement of a stock, such as the cascading momentum strategy currently being tested.

For strategies not specified according to time frames, trades are approached probabilistically, where the bot only engages in a purchase when the rise in a stock price is expected to meet or exceed the sell target. Naturally, the bot also implements a stop loss for every trade of this type.

## Current state
The bot does not currently exist in any meaningful form. As of now, some basic strategies are being backtested against historical prices in a primitive sandbox environment.
