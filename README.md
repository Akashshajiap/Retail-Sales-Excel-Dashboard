# 📊 Executive Sales & Profit Insights Dashboard

An interactive Excel dashboard that transforms 8,680 raw sales transactions (2023–2026) into a single-page executive view of sales, profit, and discount performance — built with PivotTables, PivotCharts, and slicers on top of a clean transactional dataset.

**File:** `Executive_Sales_&_Profit_Insights_Dashboard.xlsx`
**Sheets:** `Data` (raw transactions) → `pivot` (PivotTable engine) → `dashboard` (executive view)

---

## 1. Executive Summary

This workbook analyzes **8,680 orders** across the Consumer, Corporate, and Home Office segments to answer one question for leadership: *where is the business making money, and where is it leaking margin?*

Headline numbers from the dashboard:

| KPI | Value |
|---|---|
| Total Sales | **$8,972,527.06** |
| Total Profit | **$1,299,796.52** |
| Total Orders | **8,683** |
| Total Quantity Sold | **48,043** |
| Average Discount | **13.7%** |
| Profit Margin | **14.5%** |

Technology and Furniture drive the most revenue, the Consumer segment is the single largest profit contributor, and steep discounting is strongly associated with eroded — and often negative — profit on individual orders.

---

## 2. Business Problem

Sales data was sitting in a flat, transaction-level table with no way for stakeholders to quickly answer everyday business questions:

- Which **segments, categories, and regions** actually generate the most sales and profit?
- Are certain **discount levels quietly destroying profit** on otherwise healthy sales?
- Which **sub-categories** are the top revenue drivers, and which underperform?
- How do **sales and profit trend month-to-month**, and is the trend improving or declining?
- **850 of 8,680 orders (~9.8%)** closed at a net loss — where are they concentrated, and why?

Leadership needed a **single, at-a-glance dashboard** — not a raw data dump — to spot these patterns and act on them without running manual queries every time.

---

## 3. Methodology / Skills

**Data preparation**
- Structured raw order-level data (`Order ID`, `Order Date`, `Year`, `Month`, `Day`, `Segment`, `Category`, `Sub-Category`, `Region`, `Sales`, `Profit`, `Quantity`, `Discount`) into a clean Excel Table for reliable PivotTable refresh.

**Analysis engine**
- Built a multi-dimensional **PivotTable** (`pivot` sheet) summarizing Sales, Profit, Quantity, and Discount across Segment, Category, Sub-Category, Region, and Month.
- Derived KPI calculations: Total Sales, Total Profit, Total Orders, Total Quantity, Average Discount, and Profit Margin (Profit ÷ Sales).

**Visualization**
- Designed 6 linked **PivotCharts** on the `dashboard` sheet:
  - Doughnut chart — Sales by Segment
  - Line chart — Sales & Profit Trend (by month)
  - Clustered bar chart — Profit vs. Discount
  - Horizontal bar chart — Sales by Category
  - Column chart — Sales by Region
  - 3D pie chart — Top 5 Sub-Categories by Sales
- Applied a consistent brand color palette (purple/orange/violet accents) and KPI card layout for an executive-ready, print-friendly single view.

**Tools:** Microsoft Excel — PivotTables, PivotCharts, Slicers, formula-driven KPIs.

---

## 4. Results & Business Recommendations

**Category & Region performance**
- **Technology** ($4.58M sales) and **Furniture** ($3.71M sales) together account for ~93% of revenue, while **Office Supplies** contributes far less ($675K) despite high order volume — recommend evaluating Office Supplies pricing/bundling to lift its margin contribution.
- Sales are evenly spread across regions (**East $2.32M**, **South $2.25M**, **West $2.23M**, **Central $2.17M**) — no single region is underperforming, so growth investment can follow demand rather than fixing a laggard.

**Segment profitability**
- **Consumer** is the top segment on both sales ($4.70M) and profit ($680K), followed by **Corporate** ($2.67M / $392K) and **Home Office** ($1.61M / $228K) — recommend prioritizing retention/loyalty programs for Consumer accounts, the largest profit engine.

**Discounting is the biggest controllable risk**
- Discount and profit show a **strong negative correlation (-0.44)**. Average profit per order collapses as discount increases:
  - 0–10% discount → **$199.68** avg. profit/order
  - 10–20% discount → **$117.65**
  - 20–30% discount → **$65.17**
  - 30%+ discount → **$14.55**
- **850 orders (9.8%) closed at a net loss**, concentrated at the high-discount end.
- **Recommendation:** Cap discretionary discounts near 20%, and require approval above that threshold — the data shows margin erosion accelerates sharply past this point.

**Product mix**
- **Copiers, Computers, Accessories, Phones,** and **Furnishings** are the top 5 sub-categories by sales — recommend protecting inventory/marketing spend here while auditing discount practices specifically within these high-volume lines.

---

## 5. Features / Highlights

- ✅ **Single-page executive dashboard** — all KPIs and charts visible without scrolling
- ✅ **6 interactive PivotCharts** covering segment, trend, discount impact, category, region, and sub-category views
- ✅ **6 headline KPI cards** — Total Sales, Total Profit, Total Orders, Total Qty Sold, Avg Discount, Profit Margin
- ✅ **Fully dynamic** — refreshing the underlying PivotTable updates every chart and KPI instantly
- ✅ **8,680-row transactional dataset** spanning 4 years (2023–2026) as the analytical foundation
- ✅ **Consistent, presentation-ready design** with a branded color palette suitable for stakeholder reporting


- <img width="1767" height="750" alt="Screenshot 2026-07-02 113332" src="https://github.com/user-attachments/assets/41c88e2d-3ed0-46e7-b727-98f48c7fcc61" />
