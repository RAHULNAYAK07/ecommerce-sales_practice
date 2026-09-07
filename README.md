# E-Commerce Sales Analysis (Excel)

An end-to-end sales performance analysis of a U.S.-based retail/e-commerce dataset (2011–2014), built entirely in Excel using Pivot Tables, Pivot Charts, and an interactive dashboard.

## 📊 Project Overview

This project analyzes **9,994 order line items** (5,009 unique orders) from a Superstore-style retail dataset to uncover sales, profit, and customer trends across regions, categories, and time. The workbook is structured as a 3-layer analysis: raw data → pivot-based calculations → interactive dashboard.

## 📁 Dataset

| Detail | Value |
|---|---|
| Rows | 9,994 order line items |
| Unique Orders | 5,009 |
| Date Range | Jan 2011 – Dec 2014 |
| Unique Customers | 793 |
| Unique Products | 1,862 |
| States Covered | 49 |
| Cities Covered | 531 |
| Segments | Consumer, Corporate, Home Office |
| Categories | Furniture, Office Supplies, Technology |
| Regions | South, West, Central, East |
| Ship Modes | Standard Class, Second Class, First Class, Same Day |

**Columns:** Row ID, Order ID, Year, Order Date, Ship Date, Ship Mode, Customer ID, Customer Name, Segment, Country, City, State, Postal Code, Region, Product ID, Category, Sub-Category, Product Name, Sales, Quantity, Discount, Profit.

## 🗂️ Workbook Structure

- **`Data`** — Raw, cleaned transactional dataset (9,994 rows × 22 columns); the single source of truth all pivots reference.
- **`charts`** — Pivot tables and pivot charts powering the analysis (monthly trends, category/sub-category breakdowns, state-wise sales, yearly summaries, etc.).
- **`dashboard`** — Consolidated interactive dashboard view combining key visuals and slicers for at-a-glance exploration.

## 🔑 Key Metrics (Overall)

| Metric | Value |
|---|---|
| Total Sales | **$2,297,200.86** |
| Total Profit | **$286,397.02** |
| Overall Profit Margin | **12.47%** |
| Average Discount | **15.6%** |
| Total Quantity Sold | 37,873 units |

## 📈 Analysis Included

- **Monthly Sales & Profit Trend** — Sales and profit aggregated by month (Jan–Dec), revealing strong Q4 seasonality (Sep, Nov, Dec are consistently the highest-performing months, with November peaking at ~$349K in sales).
- **Yearly Performance (2011–2014)** — Year-over-year growth in sales, profit, quantity, order count, and profit margin, showing consistent growth each year (Sales grew from ~$484K in 2011 to ~$734K in 2014).
- **Category & Sub-Category Breakdown** — Profit and sales share across Furniture, Office Supplies, and Technology, plus top-performing sub-categories (Phones, Chairs, Storage, Tables, Binders by sales volume).
- **State-Wise Sales Distribution** — Full 49-state sales breakdown, highlighting top markets (California, New York, and Texas lead in total sales).
- **Profit Margin Analysis** — Monthly profit margin trend, isolating months where high sales didn't translate to proportionally high profit (useful for spotting discount-driven margin erosion).
- **Interactive Dashboard** — A single-view dashboard combining the above visuals with slicers for dynamic filtering by year, region, category, or segment.

## 🧠 Key Insights

- **Technology** is the strongest category by profit contribution (~$145K), despite Office Supplies having a comparable sales share — indicating stronger margins in Technology.
- **Furniture** generates solid sales volume but the lowest profit contribution of the three categories, suggesting discounting or cost pressure is compressing margins in this category.
- Sales are **highly seasonal**, with Q4 (Sep–Dec) consistently outperforming the rest of the year — relevant for inventory planning and marketing spend timing.
- **California, New York, and Texas** are the top three states by sales, together contributing a disproportionate share of national revenue.
- Profit margin **fluctuates independently of sales volume** month to month — high-sales months don't always correspond to high-margin months, pointing to discounting as a key lever affecting profitability.

## 🛠️ Tools & Techniques Used

- Excel Pivot Tables & Pivot Charts
- Slicers for interactive filtering
- Aggregate formulas (SUM, COUNT) across Sales, Profit, Quantity, and Profit Margin
- Time-series analysis (monthly and yearly trends)
- Dashboard design for at-a-glance KPI reporting

## 🚀 How to Use

1. Clone/download the repository and open `Ecommerce_Sales_Analysis.xlsx` in Excel.
2. Go to the **`dashboard`** sheet for the consolidated interactive view.
3. Use the slicers to filter by Year, Region, Category, or Segment.
4. Explore the **`charts`** sheet to see the underlying pivot tables behind each visual.
5. The **`Data`** sheet contains the raw dataset if you want to build your own pivots or run further analysis (e.g., in Python/Power BI).

## 📌 Possible Next Steps

- Rebuild the same analysis in Power BI with DAX measures for more advanced KPIs (YoY growth %, running totals).
- Add customer segmentation (RFM analysis) using Customer ID and Order Date.
- Build a discount-vs-profit regression to quantify how discount level impacts margin by category.

---
*Feel free to explore, fork, and extend this analysis — contributions and suggestions are welcome!*
