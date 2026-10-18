# Andes Retail Commercial Performance Analysis

Power BI dashboard project focused on commercial performance, revenue behavior, profitability, customer segments, product categories, geographic performance, and executive business interpretation for Andes Retail Group during 2024-2025.

This project is part of my professional data analytics portfolio and is positioned as a Business Intelligence / Marketing Data Analytics case study.

## Project Overview

This project analyzes the commercial performance of Andes Retail Group using a transactional Excel dataset and a Power BI dashboard.

The goal was to transform raw commercial data into an executive dashboard that helps monitor revenue, profit, margin, units sold, orders, customers, product categories, countries, regions, and customer segments.

The final dashboard includes two main views:

1. **Executive Overview**
2. **Detailed Analysis**

The project follows a complete business intelligence workflow:

```text
Excel dataset -> Power Query -> Power BI -> KPI modeling -> dashboard design -> business insights -> recommendations
```

## Business Context

Andes Retail Group operates across Colombia, Chile, and Peru, selling products across four main categories:

- Electronics
- Clothing
- Sports
- Home

The business needed a clear way to evaluate commercial performance during 2024 and 2025, identify where revenue and profit were concentrated, and detect opportunities by customer segment, product category, country, and region.

## Business Questions

This analysis addresses the following questions:

- How did total revenue evolve between 2024 and 2025?
- Which countries and regions generated the most revenue?
- Which product categories contributed most to profit?
- Which customer segments generated the highest commercial value?
- Where could Andes Retail Group focus future commercial actions?

## Dataset Used

The analysis uses a transactional Excel dataset containing commercial order data for 2024 and 2025.

Main fields include:

- Order ID
- Order date
- Season
- Customer ID
- Customer segment
- Region
- Country
- Product category
- Units sold
- Unit price
- Revenue
- Cost

The dataset was prepared in Power Query before building the dashboard in Power BI.

## Analytical Workflow

This project follows an **Excel → Power Query → Power BI → business insights** workflow.

### 1. Data exploration and preparation

- Imported the 2024–2025 transactional Excel dataset into Power BI Desktop.
- Reviewed the commercial fields and adjusted data types in Power Query: order date as date, units sold as whole number, unit price/revenue/cost as decimal numbers, and geographic/customer/product attributes as text.
- Created a conditional field, `Nivel_Venta`, to classify orders as **Venta Alta** for revenue greater than or equal to 1,000 and **Venta Baja** otherwise.
- Reviewed data consistency before using the fields in business indicators and visualizations.

### 2. Commercial KPIs

- Built and interpreted the reported indicators: total revenue, total profit, profit margin, units sold, total orders, and unique customers.
- Compared revenue and profitability by year, country, region, product category, and customer segment.

### 3. Power BI reporting

- Designed **Executive Overview** for rapid interpretation through KPI cards, annual revenue, category and country comparisons, and interactive filters.
- Designed **Detailed Analysis** to explore revenue and profit by customer segment, profit by product category, revenue by region, and combinations in the summary table.

### 4. Executive communication

- Applied the **SCQA** framework (Situation, Complication, Question, Answer) to the overview and detailed narratives.
- Turned descriptive business patterns into commercial recommendations and a concise executive update.

## Validated Commercial Results

The figures below were recalculated from the [source Excel dataset](datasets/andes-retail-group-2024-2025-dataset.xlsx) committed to this repository. The dataset contains **5,000 orders**, with all twelve original fields populated, unique order IDs, and order revenue matching units sold × unit price. Both 2024 and 2025 contain observations from **January through December**.

This is a **source-data reconciliation**, not a claim that every DAX measure or Power BI interaction has been independently retested. The dataset does not specify a currency, so all monetary values below are reported in the **original dataset units**.

| KPI | Verified total, 2024–2025 |
|---|---:|
| Total revenue | 5,531,994.00 |
| Total cost | 3,590,244.67 |
| Total profit (revenue − cost) | 1,941,749.33 |
| Profit margin (profit / revenue) | 35.10% |
| Units sold | 57,601 |
| Orders (unique order IDs) | 5,000 |
| Unique customers (distinct customer IDs) | 3,821 |
| Average order value (AOV) | 1,106.40 |

### Full-year performance: 2024 vs. 2025

| Metric | 2024 | 2025 | Year-over-year change |
|---|---:|---:|---:|
| Revenue | 2,863,384 | 2,668,610 | **−6.80%** |
| Total profit | 1,005,811.62 | 935,937.71 | **−6.95%** |
| Profit margin | 35.13% | 35.07% | **−0.06 percentage points** |
| Orders | 2,550 | 2,450 | **−3.92%** |
| Average order value | 1,122.90 | 1,089.23 | **−3.00%** |
| Units sold | 29,426 | 28,175 | **−4.25%** |

The two annual periods are comparable full calendar years. The dashboard rounds total units and unique customers to **58K** and **4K**; the exact values are shown above.

### Revenue bridge: fewer orders and lower average order value

Since **revenue = number of orders × average order value**, the **194,774** drop between the years can be decomposed arithmetically:

| Component | Revenue effect |
|---|---:|
| 2024 revenue | 2,863,384 |
| Change attributable mathematically to 100 fewer orders, holding 2024 AOV constant | −112,290 |
| Change attributable mathematically to lower AOV across 2025 orders | −82,484 |
| **2025 revenue** | **2,668,610** |

This breakdown allocates approximately **57.7% of the observed difference to the order-count component** and **42.3% to the AOV component** under this decomposition order. It is an accounting identity, **not evidence of the underlying causes** (such as pricing, competition, demand, or marketing effectiveness).

### Where the commercial differences appeared

| Dimension | Group | Revenue 2024 | Revenue 2025 | Change | YoY |
|---|---|---:|---:|---:|---:|
| Customer segment | Premium | 1,397,174 | 1,201,043 | **−196,131** | **−14.04%** |
| Customer segment | Economic | 241,396 | 255,612 | +14,216 | +5.89% |
| Product category | Electronics | 746,412 | 662,244 | **−84,168** | **−11.28%** |
| Product category | Home | 670,273 | 692,570 | +22,297 | +3.33% |
| Region | South | 950,120 | 834,693 | **−115,427** | **−12.15%** |
| Region | North | 942,109 | 948,057 | +5,948 | +0.63% |
| Country | Peru | 1,138,222 | 1,020,356 | **−117,866** | **−10.36%** |

The table highlights selected contrasts, not every group. **Do not add changes from different dimensions**: the same order can contribute simultaneously to a customer segment, a product category, a region, and a country. Group-level changes within a single dimension can be reconciled to the overall revenue movement.



## Key Metrics

The dashboard tracks the following key performance indicators:

| Metric | Result |
|---|---:|
| Total Revenue | 5.53M |
| Total Profit | 1.94M |
| Profit Margin | 35.10% |
| Units Sold | 58K |
| Total Orders | 5K |
| Unique Customers | 4K |

These metrics provide an executive view of the business performance and support deeper analysis by segment, category, country, and region.

## Power BI Dashboard

### Executive Overview

The executive view summarizes the main business indicators: total revenue, total profit, profit margin, units sold, total orders, and unique customers. It also shows annual revenue evolution, revenue by product category, revenue by country, and interactive filters for country, category, and customer segment.

<p align="center">
  <img src="images/1_overview-ejecutivo.png" alt="Andes Retail executive overview dashboard" width="900">
</p>

### Detailed Analysis

The detailed view explores revenue and profit by customer segment, profit by product category, revenue by region, and a summary table by country, region, product category, and customer segment. This page supports deeper commercial diagnosis and opportunity detection.

<p align="center">
  <img src="images/2_analisis-detallado.png" alt="Andes Retail detailed analysis dashboard" width="900">
</p>

## Key Findings

The source-data reconciliation strengthens the original Power BI dashboard findings with specific comparisons:

1. **Revenue fell 6.80% while profit margin stayed close to 35%.**  
   Revenue declined by **194,774**, and absolute profit declined by **69,873.91** (−6.95%). The relatively stable margin does **not** mean absolute profit was unchanged.

2. **Both order count and average order value weakened.**  
   Orders fell from **2,550 to 2,450** (−3.92%), while AOV dropped from **1,122.90 to 1,089.23** (−3.00%). Under an order-count-first arithmetic bridge, those components correspond to approximately **112,290** and **82,484** of the revenue reduction, respectively. The bridge is descriptive, not causal.

3. **Premium is the priority segment to investigate, not automatically the segment to discount.**  
   Premium generated the highest 2024–2025 revenue (**2,598,217**) and profit (**914,605.16**), but its annual revenue dropped by **196,131** (−14.04%). Premium orders decreased from **795 to 724**, and average order value decreased from approximately **1,757.45 to 1,658.90**. The segment's decline exceeded the overall net reduction because other segments partially offset it. This does not establish churn or customer lifetime value.

4. **Geographic results diverged rather than moving uniformly.**  
   The **South** region lost **115,427** in revenue (−12.15%), whereas **North** gained **5,948** (+0.63%). At the country level, **Peru** declined **117,866** (−10.36%). Region and country are overlapping analytical dimensions, so their declines should not be added together.

5. **Category leaders in total profit were not immune to falling sales.**  
   **Sports** generated the highest total 2024–2025 profit (**505,253.12**) and **Electronics** followed (**496,738.15**). However, Electronics revenue fell **84,168** (−11.28%) year over year, while Home increased **22,297** (+3.33%). Category margins were close to 35%, so absolute profit contribution should not be confused with a substantially higher profit-margin rate.

6. **The detailed report makes the next diagnosis possible.**  
   The country, region, category, and segment filters help locate combinations worth investigating. The current dataset does not include marketing-channel spend or campaign exposure, so it cannot independently explain the revenue decline or prove which marketing intervention will work.



## Business Recommendations

The next actions below are **hypotheses and measurement plans**, not guaranteed business outcomes:

1. **Diagnose the decline through orders and average order value.**  
   Track monthly orders, revenue, AOV, profit, and margin, then compare 2024 and 2025 by segment and product category. **Success measure:** identify which combinations account for the largest absolute decline and preserve profit margin during corrective actions.

2. **Investigate the Premium segment before designing loyalty or upselling campaigns.**  
   Its **−196,131** revenue change is the clearest segment-level priority. Examine the fall in Premium order count and AOV by category, country, and region before deciding whether the appropriate response is product assortment, customer contact, or a controlled promotional test. **Success measures:** Premium orders, AOV, revenue, and profit. The data alone does not establish a retention problem.

3. **Target the South region and Peru for separate diagnostic reviews.**  
   South had a **−12.15%** regional revenue change and Peru a **−10.36%** country-level change; these are **different slices of the same dataset**, not additive losses. Use cross-filters to identify specific intersections with declining orders or AOV. **Success measures:** revenue, orders, AOV, and margin in each relevant slice.

4. **Review Electronics against the growth seen in Home.**  
   Electronics revenue decreased **11.28%** while Home increased **3.33%**. Compare changes in category order count, order value, and profit before prioritizing inventory or communication. **Success measure:** category profit and revenue improvement without eroding margins. Any marketing-campaign effectiveness claim would require additional campaign data.

5. **Protect profitability while testing commercial interventions.**  
   The overall margin remained around **35%** despite lower revenue. Avoid assuming that aggressive discounting is warranted: evaluate incremental revenue **and incremental profit**, using controlled pilots where feasible. **Success measure:** sustained order/AOV recovery with acceptable profit margin.



## Tools and Skills

- **Microsoft Excel:** source transactional data and commercial field interpretation.
- **Power Query:** importing data, defining appropriate data types, reviewing consistency, and creating the `Nivel_Venta` conditional classification.
- **Power BI Desktop:** commercial KPIs, report layout, comparative charts, table summaries, slicers, and interactive executive reporting.
- **Commercial and Marketing Analytics:** interpreting revenue, profit, margin, sales volume, customer segments, product-category performance, and geographic differences.
- **Business Storytelling (SCQA):** framing business questions, explaining commercial findings, and translating them into recommendations.

## Professional Value

This project demonstrates my ability to transform commercial data into a clear and usable executive report. The combination of Power Query preparation, business KPIs, interactive Power BI views, and actionable interpretation is relevant to **Data Analyst, Marketing Data Analyst, Commercial Analyst, and Business Intelligence Analyst** roles.

## Personal Voice and Learning

My background in marketing shaped the way I approached this case: I did not want to show sales figures without connecting them to commercial decisions. The executive view answers *what happened*; the detailed view helps explore *where* revenue and profit are concentrated.

One important lesson was to separate **a visible pattern from its underlying cause**. The dashboard indicates lower revenue in 2025 than in 2024, but that alone cannot establish whether demand, pricing, product mix, seasonality, or marketing execution caused the change. Those remain hypotheses to test before committing resources.

This work strengthened my ability to combine **data preparation, KPI interpretation, visual communication, and commercial reasoning** in a format a stakeholder can understand quickly.

## Repository Structure

```text
andes-retail-commercial-performance-analysis/
├── dashboard/
│   └── andes-retail-commercial-performance-powerbi-dashboard.pbix
├── datasets/
│   └── andes-retail-group-2024-2025-dataset.xlsx
├── images/
│   ├── 1_overview-ejecutivo.png
│   └── 2_analisis-detallado.png
├── andes-retail-commercial-performance-project-notebook.ipynb
└── README.md
```

## File Guide

- `dashboard/andes-retail-commercial-performance-powerbi-dashboard.pbix`  
  Power BI dashboard file with the Executive Overview and Detailed Analysis pages.

- `datasets/andes-retail-group-2024-2025-dataset.xlsx`  
  Source Excel dataset used for the commercial performance analysis.

- `images/1_overview-ejecutivo.png`  
  Screenshot of the Executive Overview page displayed directly in this README.

- `images/2_analisis-detallado.png`  
  Screenshot of the Detailed Analysis page displayed directly in this README.

- `andes-retail-commercial-performance-project-notebook.ipynb`  
  Project notebook documenting the dashboard development, SCQA narrative, evaluator feedback, and business interpretation. It is a Markdown-oriented academic document, not a Python analysis pipeline.

- `README.md`  
  Portfolio documentation with business context, workflow, findings, recommendations, and dashboard previews.

## Reproducibility Note

The source Excel dataset and the Power BI `.pbix` are included in this repository. Download them and open the report in **Power BI Desktop** to explore the interactive dashboard. If the original Excel source path is unavailable on another computer, update it in **Power Query / Data source settings** before refreshing.

The `.ipynb` documents the original project and its SCQA storytelling. It is primarily a narrative notebook, **not an executable Python pipeline**. The two PNGs embedded above are static dashboard previews for recruiters and do not replace the interactive `.pbix`.

Results are reported in the original dataset's units; no specific currency is asserted unless confirmed by the source.

## Project Status

The original dashboard was completed and reviewed during the academic project. On `portfolio-polish`, the source Excel figures, annual comparison, and principal commercial findings have been cross-checked for portfolio documentation. The published Power BI report remains the original project; the `main` branch will only be updated after final approval.
