# Tayseer Services

- **Course:** Data Visualization and Storytelling
- **Student:** Ghaida Al-Otyan
- **SDAIA Academy:** https://github.com/SDAIAAcademy

## Description
Average completion time for government services dropped a lot since 2021. This project checks if services really got faster, or if people just moved from branches to the Mobile App. It then shows where to spend SAR 40M.

## Audience, question, scope
- **Audience:** Director of Service Delivery / Branch Operations
- **Question:** Is the drop in completion time a real efficiency gain, or mostly people moving to the Mobile App? Should investment target branches?
- **Scope:** all 13 regions, 9 service categories and 4 channels, Jul 2021 to Jun 2026

## How the numbers are calculated
- **Completion time, CSAT, cost per transaction:** weighted by transactions, sum(value × transactions) / sum(transactions)
- **Complaints:** per 10,000 transactions
- **Digital adoption:** the same value repeats for all 4 channels, so duplicates are removed before taking the average
- **Channel mix effect:** 2025 channel times with 2021 channel shares
- **Extra branch hours:** branch time above Riyadh and Eastern Province for the same service, times transactions
- 2021 is Jul–Dec and 2026 is Jan–Jun

## Story
**Finding:** Most of the drop comes from people moving to the Mobile App, not from faster service. Branches are still slow, mainly in three regions.

**Evidence:**
- Average completion time fell from 25.9 min in 2021 to 14.7 min in Jan–Jun 2026.
- Branch time only fell from 40.2 min to 34.9 min over the same period.
- With the 2021 channel mix, 2025 would be 23.0 min instead of 15.8 min, so 71% of the drop is channel mix.
- Makkah, Jazan and Asir have 79% of the extra branch hours in 2025.

**Action:** Spend the SAR 40M on branch process improvement: Makkah SAR 27M, Jazan SAR 7M and Asir SAR 6M. Start with Justice & Notary and Business & Licensing. In these regions they take about 120 min per branch visit, compared with about 45 min in Riyadh. Keep moving simple services to digital.

## Limitation
This shows correlation, not cause. Simple services may have moved online first, leaving harder cases in branches. Some months have low volume, likely Ramadan. The data is synthetic and has no user-level detail.

## Chart choices
The line chart shows change over time, with Branch and the national line highlighted. The bar chart compares groups: 2021, 2025 with the old channel mix, and 2025. Both charts start at zero and use colorblind-friendly colors.

## AI note
I used Claude to help write the code. I checked these myself:
- I recomputed the weighted averages.
- I checked that digital adoption has one value per month, region and category before removing duplicates.
- I checked that no chart axis is cut.
