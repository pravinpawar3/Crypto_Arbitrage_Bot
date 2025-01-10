# Crypto Arbitrage Bot - Identifies Risk-Free Opportunities

## Overview
The Crypto Arbitrage Bot is a Python-based tool designed to exploit arbitrage opportunities between the Coinbase and Kraken cryptocurrency exchanges. It aims to achieve risk-free profits by identifying price differences and executing trades accordingly. The bot performs real-time price monitoring and arbitrage simulations to optimize trading strategies.

![image](https://github.com/user-attachments/assets/418db030-52a5-478f-ba8e-31ec2dea0ae1)

![image](https://github.com/user-attachments/assets/48603384-47f9-48ae-a937-1953658afca2)

## Features
- **Real-time Data Fetching**: Integrates with Coinbase and Kraken APIs to fetch current cryptocurrency prices.
- **Arbitrage Detection**: Identifies arbitrage opportunities by comparing prices between exchanges.
- **Rebalancing Strategies**: Implements strategies to rebalance the portfolio and maintain optimal trading positions.
- **Performance Metrics Tracker**: Monitors profitability and tracks key performance metrics such as balance, profits, buy/sell signals, and API call times.

## Requirements
- Python 3.7+
- Libraries:
  - `os`
  - `requests`
  - `time`
  - `matplotlib`
  - `datetime`

## Run the Bot

### Parameters
Define the parameters for running the bot in the script.

- **symbol**: The cryptocurrency symbol for Coinbase (e.g., `"BTC-USD"`).
- **kraken_pair**: The cryptocurrency pair for Kraken (e.g., `"XXBTZUSD"`).
- **initial_balance**: The starting balance in USD.
- **iterations**: The number of iterations for the simulation.
- **interval**: The time interval between iterations in seconds.

### Example

```bash
python arbitrage_bot.py --symbol BTC-USD --kraken_pair XXBTZUSD --initial_balance 1000 --iterations 100 --interval 60
```

### Example Output

The script will output the following:
- Real-time prices from Coinbase and Kraken.
- Arbitrage opportunities.
- Performance metrics over multiple iterations.

It will also generate plots for the following metrics:
- **Balance Over Time**
- **Profits Over Time**
- **API Call Times**
- **Buy/Sell Signals Over Time**

## Code Explanation

- **get_coinbase_price**: Fetches the current price of a cryptocurrency from Coinbase.
- **get_kraken_price**: Fetches the current price of a cryptocurrency from Kraken.
- **simulate_arbitrage**: Simulates arbitrage opportunities and tracks metrics.
- **plot_metrics**: Plots the tracked metrics for visualization.

## License
This project is licensed under the MIT License.
```
