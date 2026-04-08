# Shock & Price
### How Geopolitical Crises Move Global Oil Markets

A data analysis and visualization project tracking oil price responses to 
major geopolitical shocks from 1993 to 2026, with a focus on the ongoing 
US-Israel conflict with Iran and the first-ever closure of the Strait of Hormuz.

## Live Dashboards
- [Dashboard 1: The History](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/History)
- [Dashboard 2: Iran 2026](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/Iran2026#1)
- [Dashboard 3: At the Pump](https://public.tableau.com/views/ShockOilPrices/AtthePump)

## Published Analysis
- [Your Gas Bill Is a War Report](https://medium.com/@jxdata/your-gas-bill-is-a-war-report-e4db8988af9b) — Medium article covering 30 years of oil price data, the per-president analysis, and the Brent-to-pump lag finding

## Key Findings
- The 2026 US-Israel war on Iran produced the fastest oil price spike in 
  30 years of data, peaking in just 4 days
- The previous record was the Ukraine invasion at 12 days
- Brent crude peaked at nearly $128/barrel on April 2, 2026, before a 
  ceasefire on April 7 triggered a 15% single-session drop to $92.21
- US retail gas crossed $4.00/gallon on March 31 and reached $4.12 by 
  April 6 — the first time above $4 since 2022
- Asia-Pacific countries face the highest vulnerability to a prolonged 
  Strait of Hormuz disruption
- Brent crude price changes take approximately one week to show up at the 
  US pump, confirmed by lag correlation analysis (strongest correlation at 
  1-week lag, r = 0.544)
- Gas price spikes since 1993 consistently trace back to wars, sanctions, 
  and supply shocks rather than domestic policy or presidential terms
- In inflation-adjusted terms, the 2008 financial crisis peak remains the 
  most expensive gas in 30 years of data — not 2026

## Data Sources
- Brent and WTI spot prices: US Energy Information Administration (EIA)
- US retail gasoline prices: EIA
- TTF Natural Gas futures: Investing.com
- Country inflation data: World Bank
- US Consumer Price Index: FRED (Federal Reserve Bank of St. Louis)

## Project Structure
- `notebooks/` — five notebooks covering data cleaning, event study, 
  scenario modeling, correlation analysis, and US gas price analysis
- `data/` — raw CSV files from EIA, World Bank, FRED and Investing.com
- `outputs/` — processed CSVs and charts feeding the Tableau dashboards

## Notebooks
- `01_load_and_clean.ipynb` — data ingestion and merging across all sources
- `02_event_study.ipynb` — normalized price analysis across 8 geopolitical shocks
- `03_iran_2026.ipynb` — scenario modeling and live price tracking
- `04_correlation.ipynb` — oil price to country inflation correlation analysis
- `05_us_gas_prices.ipynb` — US retail gasoline: nominal vs inflation-adjusted, 
  per-president analysis, and lag correlation with Brent crude

## Methodology
Oil price responses are measured using an event study approach, normalizing 
prices to 100 at the event date and tracking percentage changes over a 90 day 
window. Scenario projections are calibrated from historical events rather than 
assumed speeds. Country vulnerability scores are composite indices of oil 
exposure, LNG exposure and pipeline alternatives. Inflation adjustment uses 
monthly CPI from FRED with February 2026 as the base period.

Data reflects EIA prices through April 6, 2026. Ceasefire announced April 7. 
Dashboard will reflect post-ceasefire prices in next week's update.

## Tools
Python (pandas, matplotlib, numpy) | Tableau Public