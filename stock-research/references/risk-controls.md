# Risk Controls and Trade Planning

Use this reference when the user asks for a trade plan, entry/exit levels, position sizing, stop loss, take profit, portfolio risk, or "买入/卖出/持有" style decisions.

## Core Rules

- Treat capital preservation as part of the analysis, not an afterthought.
- Define invalidation before upside targets.
- Size positions from loss tolerance, not conviction alone.
- Avoid averaging down unless the user explicitly has a preplanned scale-in framework and the thesis remains valid.
- Avoid concentrated, leveraged, or illiquid trades unless risks are explicitly analyzed.
- Warn about event risk before earnings, regulatory decisions, binary trial results, and macro releases.

## Trade Plan Template

Use this structure when enough data is available:

1. Setup type: breakout, pullback, reversal, range trade, event-driven, long-term accumulation, or avoid/no-trade.
2. Bias and horizon: bullish/bearish/neutral, with expected holding period.
3. Entry zone: price area or confirmation condition. Avoid exact precision when the data does not justify it.
4. Invalidation: fundamental trigger or technical level that means the setup failed.
5. Stop/risk: stop level, max loss per trade, and whether stop is hard, mental, or event-based.
6. Position size: derive from risk budget when the user provides portfolio size; otherwise give a formula.
7. Targets: partial profit zones, valuation target, or catalyst-based exit.
8. Monitoring: events, metrics, and price/volume behavior that would require review.

## Position Sizing

If portfolio size and max risk are known:

```text
shares = floor(max_loss_amount / abs(entry_price - stop_price))
position_value = shares * entry_price
portfolio_weight = position_value / portfolio_value
```

If only risk tolerance is known, use percentages:

- Conservative: risk 0.25%-0.5% of portfolio on one trade.
- Moderate: risk 0.5%-1.0% of portfolio on one trade.
- Aggressive: risk 1.0%-2.0% of portfolio on one trade, only with liquidity and gap-risk checks.

For gap-prone stocks, reduce size or avoid holding through events because realized loss can exceed stop-loss assumptions.

## Stop-Loss Guidance

Match stops to setup type:

- Technical stop: below support, below breakout retest, above resistance for shorts.
- Volatility stop: multiple of ATR when price noise is high.
- Thesis stop: exit when the key fundamental assumption breaks.
- Time stop: exit if the expected catalyst does not occur or price fails to confirm within the planned window.

Do not place stops at obvious round numbers without explaining why the level matters.

## Portfolio-Level Checks

Before presenting a plan, check:

- Correlation: multiple positions exposed to the same factor, sector, currency, or macro driver.
- Liquidity: average volume, bid/ask spread, and exit feasibility.
- Concentration: single-name and sector exposure.
- Event clustering: several holdings reporting earnings in the same window.
- Downside asymmetry: whether a small expected upside is paired with large gap risk.

## Language for Buy/Sell/Hold Requests

Use phrasing like:

- "在以下条件满足时，这个 setup 更值得考虑..."
- "如果已经持有，关键是看这几个失效信号..."
- "如果没有仓位，追涨的风险点是..."
- "我不会把它写成无条件买入；更稳妥的计划是..."

Avoid phrasing like:

- "一定会涨"
- "稳赚"
- "满仓"
- "无脑买入"
- "保证止损有效"

## Options and Leverage

Only discuss options, margin, futures, or leveraged ETFs when the user asks for them or they are central to the security. Include:

- Expiration, implied volatility, liquidity, spread, assignment risk, and max loss.
- Scenario table for underlying price moves.
- Warning that leverage can create losses larger than expected and stops may not execute at planned prices.
