# Akila Juan

My background includes research analysis of petrochemical industry data and polyolefins manufacturing benchmarking. My projects explore how commodity prices, physical exposure and hedging decisions affect a business’s margins and risk.

I use Python, SQL and Excel to make the assumptions visible and the results reproducible. Public portfolio work uses public or explicitly synthetic data; it does not include employer or client information.

## Projects

### Physical markets

- **[Physical crude book](https://github.com/akilatrades/commodity-decision-intelligence/tree/main/projects/physical-crude-book):** A desk's month-end work in SQL on a synthetic Permian-to-Houston book: CMA deal pricing, ticket-based delivery checks, invoice reconciliation, flat-price positions after swaps, and book P&L.
- **[Crude export arb](https://github.com/akilatrades/wti-producer-hedge-simulator/tree/main/projects/crude-export-arb):** When does Brent pay for piping Cushing crude to the Gulf Coast and shipping it to Europe? Open in 44 of 129 months under base costs, yet exports kept flowing; treating committed pipeline tariffs as sunk explains part of the gap.
- **[Crude-storage carry](https://github.com/akilatrades/wti-producer-hedge-simulator/tree/main/projects/crude-storage-carry):** When does contango pay for storage? In the historical monthly sample, 59 months had contango but only 12 covered the assumed carrying costs. The study is also written in SQL, with tests that check it against the Python model.

### Hedging, margins and risk

- **[WTI producer hedge simulator](https://github.com/akilatrades/wti-producer-hedge-simulator):** How much revenue risk does a futures hedge remove, and what remains when basis or production changes? A hedge ratio close to 1 is expected for Cushing-linked exposure; residual risk is the more useful question.
- **[Energy commodity VaR engine](https://github.com/akilatrades/energy-commodity-var-engine):** How do different risk models describe the same refiner hedge book, and where do their forecasts fail?
- **[Refining margin](https://github.com/akilatrades/energy-commodity-var-engine/tree/main/projects/refining-margin):** Does the 3-2-1 crack spread mean-revert day to day? A pre-specified rule finds no usable edge; month-start contract rolls and a one-day look-ahead error would each have suggested otherwise.
- **[Petchem feedstock and PE margins](https://github.com/akilatrades/commodity-decision-intelligence/tree/main/projects/petchem-feedstock):** Public historical ethane, propane and LDPE benchmarks, an explicit mass balance, and what a feedstock hedge leaves exposed.

### Sports pricing and forecasting

- **[NFL same-game parlay pricing](https://github.com/akilatrades/nfl-sgp-correlation):** How far off is a same-game parlay priced as if its legs were independent? Across 2012–2025, a QB's yards over and his WR1's yards over hit together 1.33x as often as independence implies; a correlation adjustment fit on 2012–2020 still priced 2021–2025 better.
- **[NFL projection analysis](https://github.com/akilatrades/nfl-dfs-projection-analysis):** Forecasting, uncertainty and reviewing predictions against outcomes.

**Currently building:** volatility-scaled risk forecasts and dated-contract reconciliation; extending the petchem model’s coproduct and basis assumptions.

Outside work, I train and compete in Muay Thai.

## AI use

I used AI tools to help write code and documentation and to review my work. I reviewed the analytical assumptions, methods and results and remain responsible for the claims made in these projects.
