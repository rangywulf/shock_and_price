# Shock & Price
### How Geopolitical Crises Move Global Oil Markets

A data analysis and visualization project tracking oil price responses to 
major geopolitical shocks from 1993 to 2026, with a focus on the ongoing 
US-Israel conflict with Iran and the first-ever closure of the Strait of Hormuz.

## Live Dashboard
[View on Tableau Public](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/Iran2026#1)

## Key Findings
- The 2026 US-Israel war on Iran produced the fastest oil price spike in 
  30 years of data, peaking in just 4 days
- The previous record was the Ukraine invasion at 12 days
- Brent crude peaked at $95.74 on Day 4 before pulling back to $94.35
- Scenario A (quick resolution) is already falsified — prices never retreated
- Asia-Pacific countries face the highest vulnerability to a prolonged 
  Strait of Hormuz disruption

## Data Sources
- Brent and WTI spot prices: US Energy Information Administration (EIA)
- US retail gasoline prices: EIA
- TTF Natural Gas futures: Investing.com
- Country inflation data: World Bank

## Project Structure
- notebooks/ — data cleaning, event study, scenario modeling, correlation analysis
- data/ — raw CSV files from EIA and World Bank
- outputs/ — processed CSVs feeding the Tableau dashboards

## Methodology
Oil price responses are measured using an event study approach, normalizing 
prices to 100 at the event date and tracking percentage changes over a 90 day 
window. Scenario projections are calibrated from historical events rather than 
assumed speeds. Country vulnerability scores are composite indices of oil 
exposure, LNG exposure and pipeline alternatives.

## Tools
Python (pandas, matplotlib, numpy) | Tableau Public