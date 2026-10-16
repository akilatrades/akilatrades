# Akila Juan

**Quantitative research analyst · trading, probability and pricing models · Houston, TX**

I'm a research analyst with a real passion for trading and for figuring out what the numbers are actually saying: probabilities, expected value, and how often things really happen compared with what the price implies. I spent my career so far in professional research and analytics, and I trade futures on a funded account under strict risk limits. Most of my own time now goes into building and testing pricing models for sports and prediction markets, and projects on physical commodity markets: how crude is priced, stored, shipped, hedged and reconciled.

The way I work is the same in every project here: ask one clear question, build the simplest model that can answer it, test it only on data it has never seen, and report the result honestly, even when the answer is "there's no edge."

## What I'm working on now

**[Sports market maker](https://github.com/akilatrades/sports-market-maker):** a market-making strategy for Kalshi's sports markets, built from my NBA and NFL player-prop models and a season of tests whose rules were written down before the data was downloaded. The models know things the price doesn't (NBA: t = 13.8 alongside the price), but buying their picks at the ask lost 0.9¢ a contract after the spread and fee, and so did weather and parlays. What paid was the other side of the book: resting "no" orders against retail "yes" buyers made 1.65¢ a contract with no model, and 2.9¢ (t = 6.1) with the model used only to skip orders it rates as losers, consistent across both halves of the season and every price level. A scan of 274 Kalshi series found the same pattern in NFL props and a few other markets, and its opposite in game-winner markets. Nine paper ledgers run live through 2026-27 with their pass criteria fixed in advance; nothing is traded with money until they pass.

## Projects

### Sports pricing and probability

| Project | The question | What I found |
|---|---|---|
| [Sports market maker](https://github.com/akilatrades/sports-market-maker) | Where is the edge in Kalshi's sports markets, and for whom? | Not in forecasting: model picks lost 0.9¢/contract at the ask. In liquidity provision: resting "no" orders made 2.9¢/contract (t = 6.1) with the model as a filter; scan of 274 series; nine live paper ledgers |
| [NBA prop model](https://github.com/akilatrades/sports-market-maker/blob/main/docs/nba-model.md) | Can a model price NBA player props well? | Calibrated within half a point on a holdout season. Its repository became the project above (renamed); the model lives there as `markets/nba` |
| [NFL prop model](https://github.com/akilatrades/sports-market-maker/blob/main/docs/nfl-model.md) | Can a transparent model price NFL player props well? | Calibrated within ~1 point over 125,803 walk-forward predictions. Merged into the project above as `markets/nfl`; the original repository, [nfl-parlay-model](https://github.com/akilatrades/nfl-parlay-model), is archived |
| [Same-game parlay pricing](https://github.com/akilatrades/nfl-sgp-correlation) | How wrong is a parlay priced as if its legs were independent? | A QB's yards over and his top receiver's yards over hit together 1.33x as often as independence implies (fair +265, not +385); the correction held on seasons it hadn't seen |
| [NFL projection analysis](https://github.com/akilatrades/nfl-dfs-projection-analysis) | How do my weekly projections hold up against real results? | Monte Carlo lineup simulations, with pre-game inputs saved and reviewed against the results |

### Trading, risk and statistics

| Project | The question | What I found |
|---|---|---|
| [Risk forecast backtest](https://github.com/akilatrades/energy-commodity-var-engine) | Do daily 99% risk forecasts for a refiner's hedge book hold up? | Volatility scaling cut misses from 2.16% to 1.43% over 1,894 forecasts and passed the coverage test, but failed the independence test; I report both |
| [Refining margin signal test](https://github.com/akilatrades/energy-commodity-var-engine/tree/main/projects/refining-margin) | Does the 3-2-1 crack spread mean-revert day to day? | No usable edge (51.7% hit rate, p = 0.68); contract rolls and a one-day look-ahead error would each have faked one |
| [WTI producer hedge simulator](https://github.com/akilatrades/wti-producer-hedge-simulator) | How much revenue risk does a hedge remove, and what's left? | A full futures hedge cut revenue-surprise variance by about 96%; compares swaps and collars priced with Black-76 |

### Physical commodity markets

| Project | The question | What I found |
|---|---|---|
| [Physical crude book](https://github.com/akilatrades/commodity-decision-intelligence/tree/main/projects/physical-crude-book) | Can SQL handle a desk's month-end on a synthetic crude book? | Deal pricing, delivery checks, invoice reconciliation, positions and P&L; caught every planted error |
| [Crude export arb](https://github.com/akilatrades/wti-producer-hedge-simulator/tree/main/projects/crude-export-arb) | When does Brent pay for shipping Cushing crude to Europe? | Open in 44 of 129 months under base costs |
| [Crude storage carry](https://github.com/akilatrades/wti-producer-hedge-simulator/tree/main/projects/crude-storage-carry) | When does contango pay for storage? | Only 12 of 59 contango months covered the assumed carrying costs; also built in SQL |
| [Petchem feedstock and PE margins](https://github.com/akilatrades/commodity-decision-intelligence/tree/main/projects/petchem-feedstock) | What does a feedstock hedge actually protect? | It can work exactly as designed while the polyethylene margin still falls |

## Professional experience

- **Research Analyst, Phillip Townsend Associates (2025–2026).** Benchmarked the operating and cost performance of polyolefins plants against industry peer groups. Validated and reconciled large client datasets and presented findings to client teams.
- **Proprietary futures trader (2024–present).** Trade crude oil and gold futures on a funded account under hard daily loss and drawdown limits. I've also traded event contracts on Kalshi.
- **Data scientist, freelance and academic (2021–2024).** Regression and classification models, SQL data pipelines and Power BI and Tableau dashboards.
- **B.S. Computer Information Systems, Data Science,** University of Houston–Victoria.

## Tools

Python (pandas, NumPy, SciPy, scikit-learn), SQL (SQLite, PostgreSQL, MySQL), Excel, Power BI, Tableau, Git, pytest and GitHub Actions. Methods I use most: walk-forward testing, calibration (Brier score, log loss), Monte Carlo simulation, bootstrap intervals and regression.

## What I'm looking for

Junior quant trading, trading analyst and quantitative research roles, especially in sports and prediction markets. I'm also interested in physical commodity trading roles, and I build projects for that side of the market too: the physical crude book, export arb, storage carry and petchem work above. I'm based in Houston. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/akila-juan-a9622a203/).

Public portfolio work uses public or clearly synthetic data; it doesn't include any employer or client information. Outside work, I train and compete in Muay Thai.

## AI use

I used AI tools to help write code and documentation and to review my work. I reviewed the analytical assumptions, methods and results and remain responsible for the claims made in these projects.
