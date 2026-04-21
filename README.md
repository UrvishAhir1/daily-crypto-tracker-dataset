# Daily Crypto Tracker Dataset

A daily updated dataset of the top 100 cryptocurrencies by market capitalization.
This dataset provides both the latest market snapshot and a growing historical time-series for analysis.

## Overview

This repository contains structured cryptocurrency market data collected daily using the CoinGecko API.
The dataset is automatically updated daily via a GitHub Actions pipeline.

## Files

* **top_100_cryptocurrency_market_latest.csv** [View File](./top_100_cryptocurrency_market_latest.csv)

  Contains the latest snapshot of the top 100 cryptocurrencies.
  Always limited to 100 rows.

* **top_100_cryptocurrency_market_historical.csv** [View File](./top_100_cryptocurrency_market_historical.csv)

  Contains daily historical data.
  Each day adds one snapshot (100 rows), enabling time-series analysis.

## Update Frequency

* Updated automatically **once per day**
* Data reflects the market at the time of execution

## Features

| Column Name                 | Description                                  |
| --------------------------- | -------------------------------------------- |
| fetch_date                  | Date when data was collected                 |
| rank                        | Rank based on market capitalization          |
| rank_category               | Tier classification (Top 10, Top 50, Others) |
| id                          | Unique identifier of the cryptocurrency      |
| symbol                      | Trading symbol (e.g., BTC, ETH)              |
| name                        | Full name of the cryptocurrency              |
| current_price               | Current price in USD                         |
| market_cap                  | Market capitalization                        |
| total_volume                | 24h trading volume                           |
| volume_market_cap_ratio     | Volume to market cap ratio                   |
| high_24h                    | Highest price in last 24 hours               |
| low_24h                     | Lowest price in last 24 hours                |
| price_range_24h             | Difference between high and low prices       |
| price_change_percentage_24h | Percentage price change in last 24 hours     |
| last_updated                | Last update timestamp from source            |

## Use Cases

* Cryptocurrency market analysis
* Time-series forecasting
* Machine learning models
* Portfolio and risk analysis
* Trend and volatility studies

## Data Source

Data is sourced from the CoinGecko public API.

## Notes

* The dataset captures **daily snapshots**, not intraday changes
* Historical data grows incrementally with one entry per day per coin
* Missing or zero values may occur if not provided by the source API

## Acknowledgements

CoinGecko for providing free and accessible cryptocurrency market data.

## License

This dataset is licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) License.

---

**Author:** Urvish Ahir
