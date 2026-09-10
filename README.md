
# Swiggy Website Traffic & Conversion Analysis (Tableau)

A Tableau dashboard analyzing website traffic behavior, conversion funnels, and device/source performance for Swiggy, built on a 10,000-row synthetic visitor dataset with 15 tracked attributes per session.

## 📁 Repository Structure

```
├── data/
│   └── swiggy_web_traffic.csv        # Raw session-level dataset
└── README.md                         # include a tableau dashboard public link
```

## 🔍 Project Overview

This dashboard explores how visitors interact with Swiggy's website — where they come from, how they navigate, and where they drop off — to surface actionable insights for improving conversion rates and reducing bounce.

The dataset tracks, per session: date, traffic source, visitor type (new vs. returning), device type, browser, operating system, country, landing/exit pages, campaign, page views, session count, bounce status, average session duration, and conversion status.

## 📊 Dashboard Views

The workbook includes 13 worksheets combined into a single interactive story, covering:

- KPI Summary — Sessions, Bounce Rate, Conversion Rate at a glance
- Conversion Analysis — By campaign, by traffic source, and trend over time
- Bounce & Device Performance — Bounce rate and conversion broken down by device type
- Device × OS Heatmap — Cross-tabulated performance across device/OS combinations
- Funnel Analysis — Landing page → exit page flow, and drop-off breakdown by funnel stage
- Retention — New vs. returning visitor mix
- Session Behavior — Average session duration and page views by source

## 🛠️ Key Fix Applied

The conversion rate metric was corrected from a flawed `SUM([Sessions])` denominator (which inflated session counts) to `COUNT([Number of Records])`, yielding an accurate overall conversion rate of **41.17%**.

## 🔗 Live Dashboard

[View the interactive dashboard on Tableau Public](https://public.tableau.com/app/profile/vraj.parekh5755/viz/milestone5swiggy/Story1)

## 🛠️ Tools Used

- **Tableau** — dashboard design and interactive visualization
- **Excel/CSV** — source dataset
