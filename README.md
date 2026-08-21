# Regional Sales Performance Dashboard — Northfield Outdoor Co. (Sample Project)

A self-directed portfolio project demonstrating end-to-end BI reporting: from raw
transactional data to a decision-ready interactive dashboard.

> **Note:** Northfield Outdoor Co. is a fictional UK outdoor retailer created for this
> project. All data is synthetically generated to reflect realistic seasonal retail
> patterns. No real client or company data is used.

## Objective

Simulate a common client request: *"We have raw sales data across regions and product
lines — help us see what's actually happening."* The project covers the full pipeline
a client would expect from a database/data engineering contractor:

1. **Data modeling** — structured a 12-month transactional dataset (`data/sales_data.csv`)
   across 5 UK regions × 6 product categories × 12 months (360 rows)
2. **Aggregation & transformation** — rolled the raw transactions up into KPI-ready
   summaries: monthly revenue/order trends, regional splits, category rankings, and
   average order value (`data/summary.json`)
3. **Reporting layer** — built an interactive dashboard (`dashboard.html`) presenting
   the KPIs a stakeholder would actually ask for: total revenue, order volume, AOV
   trend, quarter-over-quarter growth, and category/region breakdowns

## Stack

- Source data: CSV (designed to mirror a SQL Server extract)
- Transformation: Python (stand-in for T-SQL aggregation / SSIS transform logic)
- Reporting: HTML + Chart.js (stand-in for Power BI report layer — built this way so
  it's viewable directly in any browser without a Power BI license)

## What this demonstrates

- Comfort taking a raw dataset through cleaning, modeling, and aggregation
- Choosing the right KPIs for a retail sales use case (not just charting everything)
- Building a report that's readable at a glance — KPI cards up top, trend and
  breakdown charts below, consistent visual hierarchy throughout

## Files

- `dashboard.html` — open directly in any browser to view the interactive report
- `data/sales_data.csv` — the underlying raw (synthetic) transactional data
- `data/summary.json` — the aggregated data powering the dashboard's charts
