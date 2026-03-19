# Shock & Price — Executive Summary

**Project:** Geopolitical Crises and Oil Markets, 1993-2026
**Author:** Jessica Stubbs
**Last Updated:** March 18, 2026

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
| Brent peak | $95.74 on March 6, 2026 |
| Most vulnerable countries | South Korea, Japan, Pakistan, Taiwan, Singapore |
| Weeks for Brent to reach the pump | 1 week (r = 0.54 at lag 1) |
| Most expensive gas in real terms | 2008, not 2026 |

---

## What the Data Shows Right Now

As of March 11, 2026 prices have pulled back slightly from the $95.74 peak 
but remain well above pre-conflict levels. The quick resolution scenario is 
already ruled out by the data. Prices are tracking between prolonged 
disruption (~$100) and escalation (~$145). The new Supreme Leader has vowed 
to keep the Strait of Hormuz closed until the war ends.

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
- [Full Findings](FINDINGS.md)
- [GitHub Repository](https://github.com/rangywulf/shock_and_price)