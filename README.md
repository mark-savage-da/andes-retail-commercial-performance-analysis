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

Some of the main findings from the dashboard include:

1. **Revenue decreased between 2024 and 2025.**  
   The annual revenue trend shows a decline, which suggests the need to monitor commercial performance and review growth opportunities.

2. **The Premium segment generated the highest business value.**  
   Premium customers contributed the most to both revenue and profit, followed by the Standard segment.

3. **The Economic segment had a lower contribution.**  
   This segment may require a differentiated commercial strategy depending on the company's goals for acquisition, retention, or profitability.

4. **Sports and Electronics showed strong profit performance.**  
   These categories stood out as relevant contributors to profitability.

5. **Regional performance was relatively balanced, with the North region leading revenue.**  
   North generated the highest revenue, while Center and South remained close, suggesting that regional performance should continue to be monitored.

6. **The detailed summary table supports more specific opportunity detection.**  
   Combining country, region, product category, and customer segment helps identify more precise commercial patterns.

## Business Recommendations

Based on the analysis, Andes Retail Group could consider the following actions:

1. **Monitor the revenue decline between 2024 and 2025.**  
   The company should review whether the decrease is linked to demand, seasonality, product mix, pricing, campaign performance, or regional execution.

2. **Prioritize commercial actions for the Premium segment.**  
   Since Premium customers generate the highest revenue and profit, this segment should be considered for retention, loyalty, and upselling strategies.

3. **Strengthen high-performing categories such as Sports and Electronics.**  
   These categories can be used as strategic levers for campaigns, inventory planning, and commercial focus.

4. **Use regional monitoring to adjust sales and marketing efforts.**  
   Regional differences can help guide localized campaigns and commercial resource allocation.

5. **Review the Economic segment separately.**  
   Its lower contribution does not necessarily mean it should be ignored, but it may require different pricing, messaging, or product strategies.

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

The original dashboard was completed and reviewed during the academic project. The `portfolio-polish` branch contains portfolio-documentation improvements under final review. The `main` branch remains unchanged until approval.
