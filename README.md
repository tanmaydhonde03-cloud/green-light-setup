# Green Light Setup

A standalone, browser-based trading journal and performance dashboard for manually recording and reviewing trades.

## Features

- Dashboard with total trades, win rate, daily P&L and selected-period net P&L
- Manual trade entry, editing and deletion
- Asset-wise performance and attempt analysis
- Equity curve and risk observations
- Date-range filtering
- CSV export and JSON backup/restore
- Responsive dark trading-terminal interface

## Run locally

1. Download `GreenLight.html` from this repository.
2. Open the file in a modern browser (Chrome, Edge or Firefox).
3. Record trades in the Trade Journal section.

No installation or server is required.

## Data storage

Trade records are saved in the browser's local storage on the device and browser where the app is used. They are not automatically synced across devices or browsers. Use the JSON backup option regularly and restore the backup when moving to another device.

## Important limitations

This is a manual trade journal and performance-analysis tool. It does not fetch live or historical market candles, automatically identify the strategy setup, perform candle-by-candle backtesting, or place trades.

Confirm pip/tick size, contract specifications and pip/tick value with your broker before relying on risk calculations. Instrument specifications can differ by broker.

## Risk settings

The configured example risk is USD 15 per attempt, with a maximum of four attempts per asset per day and a minimum risk-reward ratio of 1:2. Treat these as journal controls, not a guarantee of trading outcomes.

## Files

- `GreenLight.html` — standalone application
- `.gitignore` — excludes local backup/export files
