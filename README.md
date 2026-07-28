<div align="center">

# 🏨 Revenue Insights in Hospitality
### Power BI Dashboard for AtliQ Grands

`Power BI` · `DAX` · `Power Query` · `Data Modeling`

📦 `hospitality-revenue-insights-powerbi`

![Dashboard Overview](hospitality%20domain%20project/images/1%29dashboard%20review.png)

</div>

## Overview

An end-to-end Power BI project analyzing revenue, occupancy, and booking behavior across AtliQ Grands' hotel portfolio — built on a star schema (`fact_bookings`, `fact_aggregated_bookings`, `dim_date`, `dim_hotels`, `dim_rooms`) with 25+ custom DAX measures (documented in [`metrics-list.xlsx`](hospitality%20domain%20project/metrics-list.xlsx)).

## 📊 Key Insights

| Insight | Detail |
|---|---|
| 💰 **No dynamic pricing** | ADR barely moves across 13 weeks even as occupancy swings 44–68% — RevPAR volatility is driven almost entirely by occupancy, not rate, signaling a flat pricing strategy |
| 📅 **No weekend premium** | Weekend ADR (₹12,725) is only ~₹43 above weekday (₹12,682) despite +6.8pp higher weekend occupancy — a clear miss on demand-based pricing |
| ⭐ **Rating drives occupancy** | The portfolio's lowest-occupancy property, AtliQ Grands Bangalore (44.3%), also holds one of its lowest ratings (2.3) — a pattern that repeats across other underperforming properties |
| 🌐 **Channel pricing is a trap** | Direct-channel rates track OTA rates closely rather than undercutting them — OTA bots detect and de-rank listings that price lower elsewhere, so promotions/perks are the safer lever than rate cuts |
| 🏙️ **Revenue ≠ efficiency** | Mumbai leads revenue (₹660.6M) but Delhi posts the highest occupancy (60.4%) and rating (3.8) |
| 🔄 **Cancellation leakage** | 24.8% of bookings cancel, capping Realisation % at 70.1% of total demand |

> 💡 These insights mirror the stakeholder review with a real hotel revenue manager during the project build — the analysis moves level-by-level (portfolio → city → property) using a Pareto-style "bottom 20%" approach to isolate where pricing strategy has the biggest revenue impact.

## 📸 Dashboard Preview

| Property & Room-Class Breakdown | KPI Trend Summary |
|---|---|
| ![Property metrics](hospitality%20domain%20project/images/2%29%20dashboard%20review.png) | ![KPI trend summary](hospitality%20domain%20project/images/3%29report%20review.png) |

|  Realisation % by Week (Weekday vs. Weekend)  | RevPAR by Week |
|---|---|
| ![Realisation trend](hospitality%20domain%20project/images/6%29%20Realisation%20%25%20by%20week.png) | ![RevPAR trend](hospitality%20domain%20project/images/5%29%20RevPar%20by%20week%20number.png) |

## 🗂️ Project Structure

<details>
<summary>Click to expand</summary>

```
hospitality domain project/
├── Revenue-Insights-in-the-Hospitality-Domain.pbix   # Final dashboard
├── stage1_power_query.pbix                       # Data cleaning
├── stage2_dax_measures.pbix                      # Measures & model
├── stage3_visual_creation_demo.pbix               # Visual build
├── metrics-list.xlsx
├── data/            → dim_date, dim_hotels, dim_rooms, fact_bookings, fact_aggregated_bookings
└── images/
    ├── 1)dashboard review.png
    ├── 2) dashboard review.png
    ├── 3)report review.png
    ├── 4) revenue trend by week.png
    ├── 5) RevPar by week number.png
    └── 6) Realisation % by week.png
```
</details>

## 🚀 Run It Yourself

```bash
git clone https://github.com/ShivamPatidar3/hospitality-revenue-insights-powerbi.git
```

1. Open `hospitality domain project/Revenue-Insights-in-the-Hospitality-Domain.pbix` in **Power BI Desktop**
2. Update data source paths to the `data/` folder if prompted
3. Refresh → explore via the date, hotel, room class & platform filters

---

<div align="center">

**[Shivam Patidar]** · [LinkedIn](https://www.linkedin.com/in/shivam-patidar-28a576245/)  

</div>
