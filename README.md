# Bitcoin Co-Movement with Global Stock Market Benchmarks

This analysis studies how Bitcoin (BTC) co-moves with global equity markets and related assets (ETH, BTC futures)
during different regional market hours.

## Assets
- BTC-USD, ETH-USD
- SPY (S&P 500 ETF), QQQ (Nasdaq 100 ETF)
- ^FTSE (UK FTSE 100), ^HSI (Hang Seng Index), ^AXJO (ASX 200)
- BTC=F (CME Bitcoin Futures)

## Data
- Source: Yahoo Finance
- Frequency: 5-minute bars, 2020 – present
- All timestamps in UTC

## Method
1. Download 5-minute close prices.
2. Compute log returns.
3. Define market sessions (US, UK, HK, AU).
4. Compute conditional correlations:
   - corr(BTC, asset | region open)
   - corr(BTC, asset | region closed)
5. Compute BTC realized volatility for each regime.

## Output
- Correlation and volatility tables
- Optional plots
