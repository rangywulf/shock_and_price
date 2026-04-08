# Key Findings
## Shock & Price: How Geopolitical Crises Move Global Oil Markets

## Live Dashboards
- [Dashboard 1: The History](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/History)
- [Dashboard 2: Iran 2026](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/Iran2026#1)
- [Dashboard 3: At the Pump](https://public.tableau.com/views/ShockOilPrices/AtthePump)

### The Central Question
When geopolitical crises hit, how fast and how far do oil prices spike, 
and does it last? Using 30 years of daily Brent crude data and 8 major 
events, this project finds that not all shocks are equal, and the 2026 
Iran conflict is unlike anything in the historical record.

---

### Finding 1: Speed Matters More Than Magnitude
The 2026 US-Israel war on Iran peaked in just 4 days, nearly 3x faster 
than the Ukraine invasion which was previously the fastest shock in the 
dataset at 12 days.

| Event | Peak % | Days to Peak |
|---|---|---|
| US-Israel war on Iran | 23.95% | 4 |
| Ukraine invasion | 31.48% | 12 |
| Libya civil war | 22.42% | 74 |
| Oil price crash | 52.91% | 87 |
| Iraq invasion | 3.46% | 83 |
| 9/11 attacks | 0.34% | 3 |

The right column tells the real story. Iraq and 9/11 barely moved markets 
because there was no supply disruption. A shock that closes a chokepoint 
is a different beast entirely.

[View the full 30 year timeline and Magnitude vs Speed chart on Dashboard 1](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/History)

---

### Finding 2: The Strait of Hormuz Changes Everything
Previous crises involved threats to supply. The 2026 conflict is the first 
time in history the Strait of Hormuz has effectively closed. Around 20% of 
global oil and LNG flows through this 21 mile wide channel daily. There is 
no alternative route for most of this volume.

---

### Finding 3: The Scenarios Played Out in Real Time
As of March 11, the Quick Resolution scenario was already falsified. Prices 
tracked between Prolonged Disruption and Escalation through mid-March, then 
broke decisively higher. Brent reached nearly $128/barrel on April 2, the 
highest daily price of the conflict, briefly touching the Escalation scenario 
ceiling before pulling back.

On April 7, Iran agreed to a ceasefire and safe passage through the Strait 
of Hormuz, roughly two hours before Trump's 8pm ET deadline. Brent dropped 
more than 15% to $92.21 on the news. The dashboard currently reflects data 
through April 6. The relief drop will appear in next week's update.

The full arc is now visible in the data: a rapid spike, six weeks of elevated 
prices between $95 and $128, and a sharp relief drop on ceasefire news. 
Whether prices stabilize here or drift back up depends on how quickly Hormuz 
traffic actually resumes.

[View the Iran 2026 Scenario Projections on Dashboard 2](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/Iran2026#1)

---

### Finding 4: Asia-Pacific Bears the Heaviest Burden
Countries are ranked by a composite vulnerability score measuring oil 
exposure, LNG exposure and availability of pipeline alternatives.

**Score 5 (most vulnerable):** South Korea, Japan, Pakistan, Taiwan, Singapore
All are entirely import dependent with no pipeline alternatives. South Korea 
confirmed only 9 days of LNG reserves remaining as of March 5.

**Score 4:** Thailand, Philippines
High oil dependency with no pipeline alternatives.

**Score 3:** China, India, Italy, Spain, Turkey
Meaningful exposure but partially buffered. China and India can pivot to 
Russian overland supply.

**Score -1 (least vulnerable):** USA, Canada, Russia, Saudi Arabia, Iraq
Major producers largely insulated from supply shortage. Note that US 
consumers still face pump price increases from global price contagion 
despite domestic production buffers.

[View the Country Vulnerability Map on Dashboard 2](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/Iran2026#1)

---

### Finding 5: Markets Price in Risk Before the Trigger
Looking at the 90 day pre-event window across all 8 events, prices were 
already moving in the 30 days before most events. This suggests markets 
price in geopolitical risk before the official trigger date, meaning the 
true cost of a crisis begins before the first headline.

[View the Event Overlay Chart on Dashboard 1](https://public.tableau.com/app/profile/jess.stubbs/viz/ShockOilPrices/History)

---

### Finding 6: Brent Price Changes Take One Week to Reach the Pump
Lag correlation analysis across 1,719 weekly observations shows that the 
correlation between Brent and US retail gasoline price changes jumps from 
0.21 at zero lag to 0.54 at a one-week lag, then drops off sharply. 

When oil prices spike, expect to feel it at the gas station the following 
week, not the same day.

---

### Finding 7: In Real Terms, 2008 Was Worse Than 2026
Adjusting US retail gasoline prices to February 2026 dollars, the 2008 
financial crisis peak of ~$4.11/gallon equals nearly $5.00 in today's money. 
The Iran 2026 spike has not yet approached that level in real purchasing 
power terms. When people say gas prices are at historic highs, the data 
says otherwise.

[View Gas Prices including inflation on Dashboard 3](https://public.tableau.com/views/ShockOilPrices/AtthePump)

---

### Methodology Note
Event study analysis normalizes prices to 100 at the event date, allowing 
direct comparison across different price environments. Scenario projections 
are calibrated from historical events rather than assumed speeds. Country 
vulnerability scores are composite indices and represent structural exposure, 
not short term price sensitivity. Inflation adjustment uses monthly CPI from 
FRED with February 2026 as the base period.

Data reflects EIA prices through April 6, 2026. This project was built 
during the active conflict period and represents a snapshot analysis 
rather than a live tracker.

Last updated: April 8, 2026.