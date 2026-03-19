# Shock & Price
### How Geopolitical Crises Move Global Oil Markets

A data analysis and visualization project tracking oil price responses to 
major geopolitical shocks from 1993 to 2026, with a focus on the ongoing 
US-Israel conflict with Iran and the first-ever closure of the Strait of Hormuz.

## Live Dashboards
- [Dashboard 1: The History](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/History)
- [Dashboard 2: Iran 2026](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/Iran2026#1)

## Key Findings
- The 2026 US-Israel war on Iran produced the fastest oil price spike in 
  30 years of data, peaking in just 4 days
- The previous record was the Ukraine invasion at 12 days
- Brent crude peaked at $95.74 on Day 4 before pulling back
- Scenario A (quick resolution) is already falsified — prices never retreated
- Asia-Pacific countries face the highest vulnerability to a prolonged 
  Strait of Hormuz disruption
- Brent crude price changes take approximately one week to show up at the 
  US pump, confirmed by lag correlation analysis
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

## Tools
Python (pandas, matplotlib, numpy) | Tableau Public