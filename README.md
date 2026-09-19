# finance-council

[Leer en español](README.es.md)

A skill for Claude Code that turns Claude into a council of ten senior specialists. You describe a business, an idea or a plan, and it goes through every discipline and comes back with a full report. It is built to disagree with you when the numbers do not hold up.

## The ten disciplines

Finance, accounting, management, commerce, economics, actuarial science, audit, statistics, treasury and risk management.

Each one gives its own reading. When two of them clash (say, commerce wants a lower price and accounting says the margin no longer covers fixed costs), the report says so instead of averaging them out.

## What you get

If you pitch a business or an idea, all ten disciplines take part and the report has seven parts:

1. Summary of the idea and the assumptions taken
2. One block per discipline, each ending in Alert, Watch or OK
3. Tensions between disciplines
4. Key numbers: break-even, capital needed, months of cash, three scenarios
5. Top 5 risks with mitigation
6. Verdict: go, go with conditions, or not yet
7. What is left to verify and next steps

For a narrow question (check a calculation, size a position, settle a price) it only calls the 2 or 3 disciplines that matter.

It asks for real numbers before giving a serious opinion. If you make it continue without them, every assumption is marked as one.

## Install

Copy the folder into your skills directory.

```bash
git clone https://github.com/Warriors1996/finance-council.git
cp -r finance-council ~/.claude/skills/finance-council
```

For the Spanish version, copy the `es` folder as its own skill:

```bash
cp -r finance-council/es ~/.claude/skills/finance-council-es
```

On Windows, the skills folder is `C:\Users\<you>\.claude\skills`.

## Use

Just describe the idea. Something like:

> I want to open a small roastery that sells coffee by subscription. What do you think?

Or ask for a single lens:

> Check the position sizing of my trading bot, I have a backtest with 40 trades.

## Limits

This is an analysis framework, not financial advice. It does not tell you to buy or sell a specific asset, and it does not replace an accountant or a lawyer for tax or legal filings. If it lacks data, it says so instead of inventing figures.

## License

MIT. See [LICENSE](LICENSE).
