# Bitcoin Market Sentiment vs Trader Performance Analysis

## Objective
Explore the relationship between Bitcoin market sentiment (Fear/Greed Index) and trader performance using historical trading data from Hyperliquid, to uncover patterns that can inform smarter trading strategies.

## Datasets
1. **Bitcoin Fear & Greed Index** — daily market sentiment classification (Extreme Fear → Extreme Greed)
2. **Historical Trader Data (Hyperliquid)** — individual trade records including execution price, size, side, direction, and closed PnL

## Methodology
- Merged trade-level data with daily sentiment classification by date
- Aggregated Closed PnL, win rate, and average trade size by sentiment category
- Analyzed position direction (long/short) distribution across sentiment regimes

## Key Findings

1. **Fear breeds profit.** Traders achieved their highest average PnL (₹71.79/trade) during Fear days, with the largest average trade size (₹9,087) — traders who stay active and size up during fear-driven dips are rewarded.

2. **Greed erodes returns.** Despite Greed having the second-highest trade volume (38,626 trades), it produced the lowest average PnL (₹33.26/trade) — a sign of overtrading and herd behavior underperforming.

3. **Extreme Greed has the best win rate (44.9%)** but smaller average trade size (₹3,227) — traders take more frequent, smaller, higher-hit-rate positions during euphoric markets, likely scalping rather than conviction trades.

4. **Extreme Fear sees the fewest trades (8,813)** — participation drops sharply during panic, but traders who remain active post a respectable ₹64.81 avg PnL, suggesting only more disciplined traders stay active.

5. **Positioning skews short-heavy during Greed/Extreme Greed** (contrarian shorting into euphoria), while Fear shows more balanced long/short activity.

## Actionable Takeaway
A sentiment-aware strategy — increasing exposure during Fear/Extreme Fear and reducing size or being more selective during Greed — aligns with the top-performing trade patterns observed in this dataset.

## Files
- `notebook.ipynb` — full analysis code
- `sentiment_analysis.png` — visualization of PnL, win rate, and trade size by sentiment

## Tools
Python, Pandas, Matplotlib, Google Colab
