# BTC Days in Price Brackets (USD)

**Original by EasyBird**

A TradingView Pine Script (v5) indicator. It counts how many daily closes Bitcoin has spent in each US-dollar price bracket since Sep 17, 2014, and shows each bracket's share of all days. The numbers match the Bitcoin brackets chart at https://andresblitz.com/bitcoin/.

## What it does
- Counts days using **Bitstamp BTC/USD** daily closes (`BITSTAMP:BTCUSD`), whatever symbol is on your chart.
- Uses $3,000 brackets by default. You can also pick $2k, $4k, $5k, $10k or $15k.
- Draws a dotted horizontal line at each bracket and a label like `$72k  24d · 0.6%`. The current bracket is highlighted in orange and marked `← now`.
- On a chart that isn't in USD (BTCCAD, for example), only the line positions are converted to that currency at today's exchange rate. Counts and labels stay in USD.

## Install on TradingView
1. Open a chart, ideally `BITSTAMP:BTCUSD` on the **1D (daily)** timeframe.
2. Open the **Pine Editor** at the bottom of the screen.
3. Paste in the contents of `btc_days_in_brackets_usd.pine`.
4. Click **Save**, then **Add to chart**.
5. In the indicator settings you can change the start date, the bracket size, the font size (Normal, Large or Huge) and how far the labels sit from the last bar.

## Notes
- Use the daily timeframe. Other timeframes skew the counts.
- If your chart's history starts after 2014, the earliest days won't be counted.
- This is for watching only, not for trading.
