# Green Light Setup

A browser-based trading journal and manual backtesting dashboard for the Green Light Setup strategy.

## Features

- Manual trade journal with asset-wise trade tracking
- Fixed USD risk planning and minimum 1:2 risk-to-reward planning
- Up to four independent attempts per asset per day
- Daily P&L and selected-period net P&L
- Asset performance and attempt-wise re-entry analysis
- Equity curve with one point per completed trade
- Portfolio and risk analytics
- CSV export and JSON backup/restore
- Responsive dark interface for desktop, tablet and mobile

## Run locally

1. Download or clone this repository.
2. Open `GreenLight.html` in Google Chrome or Microsoft Edge.
3. Record completed trades in the trade journal.

No server or build process is required.

## Data storage and backups

Trade records are stored in the browser's local storage on the device and browser where the app is opened. Data is not automatically synchronised to GitHub or between devices.

Use the application's JSON backup feature regularly. Keep backups in a secure location.

## Important limitations

- This is a manual journal and performance-analysis tool. It does not automatically fetch historical candles, detect the setup, execute trades or place broker orders.
- Pip/tick size and pip/tick value depend on the broker and instrument contract specifications. Verify these before relying on calculated P&L.
- The application is an educational tracking tool, not investment advice.

## Repository structure

```text
green-light-setup/
├── GreenLight.html
├── README.md
└── .gitignore
```

## Suggested next steps

- Add automated tests for P&L, risk, attempt limits and date filters.
- Add optional cloud database synchronisation if multi-device access is required.
- Review broker-specific contract specifications before adding automatic sizing.
