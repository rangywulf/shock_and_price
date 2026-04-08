# Shock & Price — Executive Summary

**Project:** Geopolitical Crises and Oil Markets, 1993-2026
**Author:** Jessica Stubbs
**Last Updated:** April 8, 2026

---

## What This Project Does

Tracks how oil prices respond to major geopolitical shocks using 30 years 
of daily Brent crude data. Built during the active 2026 US-Israel conflict 
with Iran, the project applies event study methodology to compare 8 crises, 
model forward scenarios, and map which countries face the greatest exposure.

---

## The Short Version

Not all geopolitical shocks move oil markets the same way. Speed matters 
more than magnitude, supply disruption matters more than military action, 
and a shock that closes a critical shipping lane is a completely different 
category from one that leaves supply routes open.

The 2026 Iran conflict is the fastest price spike in 30 years of data. 
It is also the first crisis in the dataset to involve an actual closure 
of the Strait of Hormuz, through which 20% of global oil and LNG flows daily.

---

## Key Numbers

| | |
|---|---|
| Events analyzed | 8 geopolitical shocks, 1993-2026 |
| Fastest spike | Iran 2026, peak in 4 days |
| Previous record | Ukraine 2022, peak in 12 days |
| Brent peak | $128/barrel on April 2, 2026 |
| Ceasefire drop | $92.21 on April 7, 2026 (-15% in one session) |
| US retail gas (week of Apr 6) | $4.12/gallon |
| Most vulnerable countries | South Korea, Japan, Pakistan, Taiwan, Singapore |
| Weeks for Brent to reach the pump | 1 week (r = 0.54 at lag 1) |
| Most expensive gas in real terms | 2008, not 2026 |

---

## What the Data Shows Right Now

On April 7, 2026, Iran agreed to a ceasefire and safe passage through the 
Strait of Hormuz, roughly two hours before Trump's 8pm ET deadline. Brent 
dropped more than 15% to $92.21 on the news, the largest single-session 
relief drop of the conflict.

The full arc is now visible: prices spiked to nearly $128/barrel on April 2, 
six weeks of sustained disruption between $95 and $128, then a sharp drop 
on ceasefire news. US retail gas crossed $4.00/gallon on March 31 and 
reached $4.12 by April 6. In real terms, it still hasn't matched the 2008 
peak.

Whether prices stabilize or drift back up depends on how quickly Hormuz 
traffic actually resumes. The dashboard will reflect the April 7 drop in 
next week's data update.

---

## Tools and Methods

- **Python** — pandas, numpy, matplotlib across 5 Jupyter notebooks
- **Tableau Public** — two interactive dashboards
- **Data sources** — EIA, World Bank, FRED, Investing.com
- **Methodology** — event study framework, exponential decay scenario 
  modeling, composite vulnerability scoring, lag correlation analysis

---

## Links

- [Dashboard 1: The History](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/History)
- [Dashboard 2: Iran 2026](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/Iran2026#1)
- [Dashboard 3: At the Pump](https://public.tableau.com/views/ShockOilPrices/AtthePump)
- [Full Findings](FINDINGS.md)
- [GitHub Repository](https://github.com/rangywulf/shock_and_price)
- [Your Gas Bill Is a War Report](https://medium.com/@jxdata/your-gas-bill-is-a-war-report-e4db8988af9b) — Medium article covering 30 years of oil price data, the per-president analysis, and the Brent-to-pump lag finding