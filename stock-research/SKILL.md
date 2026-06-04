---
name: stock-research
description: Stock and ETF research workflow for public-market investing and trading decisions. Use when Codex needs to analyze an A-share, Hong Kong, US, or other listed security; compare stocks; build a watchlist; review earnings, filings, valuation, technicals, catalysts, sentiment, position sizing, stop-loss logic, or risk controls; draft a trading plan; or answer Chinese-language "炒股", "股票分析", "买不买", "持有还是卖出", "怎么看这只票" style requests.
---

# Stock Research

## Operating Principles

Treat stock work as current, high-stakes financial research:

- Verify current prices, filings, earnings dates, corporate actions, index changes, and news before relying on them.
- Prefer primary sources: exchange filings, company investor-relations pages, earnings releases, SEC EDGAR, HKEXnews, CNINFO, official exchange pages, central bank/statistics sources, and reputable data providers.
- Separate facts, estimates, and inference. Cite sources for current facts.
- Do not promise returns, claim certainty, or present a trade as personalized financial advice.
- Do not place trades, access brokerage accounts, or imply the user should execute without their own judgment.
- Use scenario framing, invalidation levels, and risk controls instead of one-line buy/sell calls.

## Intake

Identify the minimum missing context before deep analysis:

- Security: ticker/name, exchange/market, or comparable universe.
- Objective: quick view, deep research, earnings preview/review, valuation, technical setup, watchlist, or trade plan.
- Horizon: intraday, swing, medium-term, long-term.
- Style: fundamental, technical, event-driven, quantitative, income/dividend, or mixed.
- Constraints: risk tolerance, max drawdown, position size limits, market access, currency, and whether leverage/options are in scope.

If the user gives too little context, make conservative assumptions and state them. Ask a concise follow-up only when the missing context changes the analysis materially.

## Workflow

1. Build the factual base: current quote, market cap, sector, key financials, recent news, upcoming events, and relevant filings.
2. Form the thesis: bull case, bear case, key driver, time horizon, and what the market may already price in.
3. Check valuation and quality: growth, margin, cash flow, balance sheet, capital returns, peer multiples, and historical range.
4. Check technicals when useful: trend, support/resistance, volume, momentum, volatility, gap risk, and liquidity.
5. Identify catalysts and risks: earnings, guidance, regulation, macro, rates, FX, commodity inputs, management changes, lockups, dilution, and geopolitical risk.
6. Produce a decision framework: scenarios, probabilities if justified, key watch metrics, invalidation conditions, and a risk-controlled plan.

For a full workflow, read `references/research-workflow.md`. For trade plans, stops, position sizing, and risk limits, read `references/risk-controls.md`.

## Output Format

For most stock requests, respond with:

- Bottom line: concise view with confidence level and time horizon.
- Key facts: sourced current data and recent developments.
- Thesis: bull case, bear case, and the main debate.
- Valuation/technicals: include only what is relevant to the user's style.
- Catalysts: what could change the view and when.
- Risks: specific downside risks and invalidation signals.
- Plan: watchlist levels or scenario-based trade plan with risk controls, not a guaranteed instruction.

For Chinese users, answer in Chinese unless they request otherwise. Use market-specific terminology naturally, such as "A股", "港股", "美股", "财报", "估值", "支撑/压力", "止损", "仓位", and "催化剂".
