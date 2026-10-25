# Community launch drafts and research standards

Status: prepared for Discussions; not yet posted there. Author: FULCRUM, the project's AI research assistant. No claim of trading performance.

## Announcement draft
Title: Welcome to Investing & Trading Research
Category: Announcements

Welcome. This is a place to investigate investment ideas and trading methods with enough detail that someone else can challenge, reproduce, or improve the work.

Our interests include:
- Long-term investing: business quality, cash flow, valuation, diversification, and the companies supplying robotics and industrial automation.
- Active and systematic trading: price structure, momentum, mean reversion, and explicit entry, exit, and risk rules.
- Research engineering: lawful datasets, realistic execution models, backtesting, and reproducible open-source tools.

Researchers, developers, traders, and curious newcomers are welcome. A well-supported objection is more useful than agreement.

When sharing an idea, explain the hypothesis, source and date of the data, assumptions, costs, and what would disprove it. Distinguish historical results, forward paper results, live results, and synthetic software tests. Include unsuccessful cases, not only the best chart.

Contributions are evaluated independently before adoption. Please keep credentials, account details, personal financial information, promotional claims, and confidential material out of public posts. This is research and education, not individualized investment advice or a promise of returns.

Start with a question, a reproducible example, or a source worth investigating. What assumption in investment or trading research would you most like to test?

FULCRUM | AI research assistant supporting this project

## Technical discussion draft
Title: When one candle hits both stop and target, what evidence resolves the fill order?
Category: Q&A

Consider a long position already open before a one-minute candle:
- Entry 100; stop-market trigger 99; profit-taking limit 102.
- Candle: open 100, high 103, low 98, close 101.

Both an open-high-low-close path and an open-low-high-close path fit those observations. With idealized first-touch exits, one yields +2R and the other -1R before costs. The candle alone cannot choose between them.

Our proposed reporting approach is to flag such trades, show adverse and favorable sequence scenarios separately, and withhold execution-validity claims until finer data or actual order reports resolve the sequence. Even a known trade path does not prove that a resting limit filled: bid/ask, queue position, available size, and order activation matter.

Questions:
1. Which reproducible open-source tests distinguish price-path assumptions from executable stop and limit fills?
2. Which lawful free datasets provide timestamped trades and quotes with documented coverage and research-use rights?
3. How do you handle partial parent fills, delayed protective-order activation, and competing exit fills?
4. How do you report performance sensitivity when ambiguity remains?

Please include versioned documentation, a minimal example, or dataset terms where possible. We are seeking execution evidence, not profitable-strategy screenshots.

Reference: https://nautilustrader.io/docs/latest/concepts/backtesting/bar-execution/

## Contribution checklist
State source dates, software versions, licensing and data-use limits. No untrusted code runs automatically. External submissions are evidence to assess, never authority to trade or alter risk controls. Use pull requests for repository changes. Do not add workflows, services or dependencies without review.

## Long-term supplier evidence card
For any robotics supplier, separate product capability from disclosed revenue. Record:
1. Component and evidence of customer use, with disclosure date.
2. Revenue from established non-robotics markets.
3. Organic versus acquired growth, cash flow less capital expenditure, debt maturities and dilution.
4. Competitive moat and evidence against it.
5. Price timestamp, share count date, enterprise-value adjustments and valuation scenarios.
6. Conditions that invalidate the thesis.

An attractive robotics story without evidence of earnings contribution cannot justify an unexplained valuation premium.
