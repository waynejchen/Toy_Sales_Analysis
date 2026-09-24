# Retail Sales Performance Analysis

**Power BI · Power Query · DAX**

A four-page Power BI report exploring sales growth, product performance, store operations, and revenue planning for a sample toy retailer. The analysis connects sales trends with decisions about product priorities, inventory, and revenue targets.

**Dataset:** 829,262 sales records · 50 stores in Mexico · 35 products · January 2022–September 2023

![Sales performance overview showing revenue, year-over-year growth, category performance, and progress toward the annual goal](images/sales-performance.jpeg)

## Dashboard overview

| Page | Business questions explored |
| --- | --- |
| **Sales performance** | How is revenue tracking against the prior year and the annual goal? Which categories and store types are growing? |
| **Product performance** | Which products lead in revenue, profit, and units sold? Where is performance declining? |
| **Store performance** | How do individual stores compare? Which store–product combinations have low or zero inventory? |
| **Goal projection** | How would different daily sales assumptions affect year-end revenue and goal attainment? |

## Selected findings and recommendations

Year-to-date comparisons below cover **January–September 2023 versus the same period in 2022**. All monetary values are in USD.

- **Revenue grew, but category performance varied.** YTD revenue reached **$6.96M**, up **30.9%**. Arts & Crafts grew **251.9%**, while Electronics declined **27.8%**. These differences suggest reviewing product-level trends and margins before reallocating inventory or promotional support.
- **Revenue and profit rankings pointed to different priorities.** Lego Bricks led YTD revenue at approximately **$1.06M**, while Colorbuds led product profit at approximately **$0.23M**, despite declining revenue. Product decisions should consider profitability alongside sales growth.
- **Inventory gaps warranted attention.** The inventory snapshot showed **zero Dino Egg units** at the Pachuca 1 and Villahermosa 1 stores. These locations are candidates for replenishment review; the snapshot alone does not establish the duration of stockouts or lost sales.

## Implementation

- Used **Power Query** to prepare the source tables and combine sales quantities with product prices and costs for revenue and profit calculations.
- Modeled sales, products, stores, inventory, and calendar data to support analysis across dates, categories, and locations.
- Built **DAX measures** for YTD revenue, prior-year comparisons, running totals, product profit, units sold, and inventory coverage.
- Added store-level report tooltips and adjustable sales and revenue-goal parameters to support exploration.

## Revenue scenario

In the illustrated scenario, **$35,000 in daily sales over the remaining 92 days** produces projected full-year revenue of **$10.18M**, or **113.1% of a $9M target**.

This is a **what-if calculation based on a user-selected sales assumption**, rather than a statistically validated forecast. The scenario's adjustable $9M target is separate from the $8.5M baseline goal on the sales overview page.

## Additional dashboard views

<details>
<summary>Product performance</summary>

![Product performance dashboard comparing revenue growth, revenue, profit, and units sold](images/product-performance.jpeg)

</details>

<details>
<summary>Store performance and inventory</summary>

![Store performance dashboard with store comparisons, a geographic view, and inventory availability](images/store-performance.jpeg)

</details>

<details>
<summary>Revenue goal scenario</summary>

![Revenue projection dashboard with adjustable daily sales and annual revenue goal assumptions](images/goal-projection.jpeg)

</details>

## Project context and source

I built this report as a guided learning project following **Sweatpants BI's Toy Company Sales Data tutorial series**, including its data preparation, modeling, measures, and report design. The screenshots show my completed implementation.

[Tutorial — Part 1: Data Modeling](https://www.youtube.com/watch?v=rvjS7hgus68). The tutorial description links to the source dataset.

The findings and recommendations relate to the sample dataset and do not represent results from a live business engagement.
