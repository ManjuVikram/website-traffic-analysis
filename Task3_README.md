# Website Traffic Analysis — Alfido Tech

**Task 3 of 3 — Alfido Tech Data Analytics Internship Program**

## Overview
Analysis of 226,230 website traffic events (pageviews, previews, clicks) recorded across music smart-link pages over one week (Aug 19–25, 2021), covering 211 countries and 3,822 links, to understand traffic trend, the conversion funnel, geographic patterns, and top-performing content, with actionable recommendations for Alfido Tech.

**Dataset:** Music smart-link traffic events — `traffic.csv`. Each row is a single traffic event (a pageview, preview, or click) on a music smart-link page, with the visitor's country/city and the artist/track/album/link being viewed.

## Files in this repo
| File | Description |
|---|---|
| `Website_Traffic_Analysis.ipynb` | Full Jupyter notebook — data cleaning, feature engineering, trend/funnel/geographic/content analysis (executed, all outputs included) |
| `Website_Traffic_Analysis_Report.pdf` | Detailed 8-page analytical report — methodology, findings, and recommendations |
| `Task3_Submission_Summary.pdf` | 1-page submission summary — executive summary, key findings, top recommendations, key charts, and notebook screenshots |

## Approach
1. **Data cleaning** — verified that ~46% "duplicate" rows are real repeat traffic (no user ID in the data), not a data quality issue; handled missing values and the "Unknown" city category.
2. **Feature engineering** — extracted weekday from date; built helper functions for chart formatting.
3. **Trend analysis** — daily traffic volume by event type across the one-week window.
4. **Funnel analysis** — pageview → preview/click conversion rates.
5. **Geographic analysis** — traffic volume and click-through rate by country and city.
6. **Content analysis** — top artists, tracks, and links by traffic volume and conversion quality.

## Key Findings
- Total traffic declined 13.9% across the one-week window, with pageviews and clicks falling in lockstep.
- Overall click-through rate is a strong 39.2% of pageviews, but only 20.1% of visitors preview first — traffic appears largely referral-driven rather than discovery-driven.
- Traffic is geographically concentrated — **Saudi Arabia** and **India** together account for ~40% of all traffic; within Saudi Arabia, two cities (Jeddah, Riyadh) dominate.
- Click-through quality doesn't track with volume — Saudi Arabia has the most traffic but a below-average 32.9% CTR, while smaller markets like Pakistan (51.5%) convert far better.
- Traffic is highly concentrated in a single piece of content — one track ("Jalebi Baby") drives 18% of all traffic.

## Top 5 Recommendations
1. Investigate the cause of the 13.9% weekly traffic decline.
2. Prioritize high-CTR, currently-smaller markets (Pakistan, Ghana, Netherlands, Canada) for growth investment.
3. Diagnose why Saudi Arabia's CTR lags its traffic volume.
4. Reduce dependency on a single top track via cross-promotion.
5. Study and replicate what the highest-CTR top links do differently.

---
*Prepared as part of the Alfido Tech Data Analytics Internship Program.*
