---
layout: default
title: Excel Dashboard - Retail Sales
---

# Retail Sales Performance Dashboard 
[Github Link](https://github.com/adhgn/Superstore_Excel_Dashboard)
## Project Overview
This project transforms raw e-commerce data from a "Superstore" into a functional business intelligence tool. The dashboard provides actionable insights into sales trends, and regional performance to help stakeholders make data-driven decisions.

## Dashboard Preview
![Sales Dashboard](https://raw.githubusercontent.com/adhgn/Superstore_Excel_Dashboard/93f1bd2028a032130611776210fb89821938a7cf/dashboard_image.png)

## Data Transformation
A significant portion of this project involved cleaning and modeling the data using Power Query (M).

**Key Challenge & Solution:**
- **Date Standardization:** The source data used a dd/mm/yyyy format, which conflicted with my system's locale. I implemented a Change Type with Locale transformation using the en-GB culture to ensure 100% accuracy in time-series analysis.

```
// Handling the date-locale mismatch for reliable analysis
= Table.TransformColumnTypes(#"Promoted Headers",{
    {"Order Date", type date, "en-GB"}, 
    {"Ship Date", type date, "en-GB"},
    {"Sales", type number},
    {"Postal Code", type text}
})
```

## Key Features
- **Dynamic Interactivity:** Integrated Slicers for Region, Category, and Segment, allowing for real-time data filtering.

- **Time-Series Analysis:** A yearly sales trend chart.

- **Geographical Mapping:** A choropleth map visualizing sales density across the United States.

- **KPI Scorecard:** Top-level metrics for Total Sales and Growth

## Tools Used
- **Microsoft Excel:** PivotTables, PivotCharts, and Advanced Formulas.

- **Power Query:** ETL (Extract, Transform, Load) process.

- **Markdown:** For project documentation.

## Data Source 
[Kaggle](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting)
