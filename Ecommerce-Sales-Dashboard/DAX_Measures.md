# DAX Measures - E-Commerce Sales Dashboard

This file contains all the key DAX measures used in the project, with explanations of what each one does and why it was created. Understanding these measures demonstrates core skills in time intelligence, filter context, and dynamic calculations.

## Basic Aggregations

```dax
Total Sales = SUM(FactSales[SalesAmount])
```

Calculates the total revenue across all sales. Simple aggregation used as the foundation for almost every other measure.

```dax
Total Quantity = SUM(FactSales[Quantity])
```

Total number of units sold. Useful for volume analysis alongside revenue.

```dax
Avg Order Value = 
    DIVIDE([Total Sales], DISTINCTCOUNT(FactSales[OrderID]))
```

Average revenue per order. Helps understand typical order size and customer behavior.

## Time Intelligence Measures
```dax
YTD Sales = TOTALYTD([Total Sales], DimDate[Date])
```

Year-to-Date sales total. Resets every January 1st. Critical for tracking annual performance.

```dax
MoM Sales Growth % = 
VAR CurrentMonth = [Total Sales]
VAR PriorMonth = CALCULATE([Total Sales], DATEADD(DimDate[Date], -1, MONTH))
RETURN
    DIVIDE(CurrentMonth - PriorMonth, PriorMonth)
```

Month-over-Month percentage growth. Uses VAR for readability and CALCULATE + DATEADD to shift the filter context.

```dax
YoY Sales Growth % = 
VAR CurrentYTD = [YTD Sales]
VAR PriorYTD = CALCULATE([YTD Sales], SAMEPERIODLASTYEAR(DimDate[Date]))
RETURN
    DIVIDE(CurrentYTD - PriorYTD, PriorYTD)
```

Year-over-Year growth on a YTD basis. Shows true annual performance comparison, accounting for seasonality.

```dax
Running Total Sales = 
    CALCULATE([Total Sales], DATESYTD(DimDate[Date]))
```

Cumulative sales from the start of the year up to the current date. Excellent for visualizing sales momentum throughout the year.

## What-If Scenario Measure
```dax
Adjusted Target Sales = 
VAR BaseSales = [Total Sales]
VAR Multiplier = [Target Multiplier Value]
RETURN
    BaseSales * Multiplier
```
Dynamically adjusts base sales based on the Target Multiplier What-If parameter. Allows stakeholders to simulate different performance scenarios (e.g., 110% or 80% of current sales). Demonstrates interactive "what-if" analysis for forecasting and target setting.

## Key Learnings & Design Decisions

- All time intelligence measures rely on a properly marked Date Table and a relationship based on a true Date data type column (not the integer DateKey).
- VAR statements are used heavily to improve readability and performance.
- Measures are designed to be reusable across multiple visuals and pages.
- The What-If parameter was added manually as a slicer to give full control over placement and formatting.

These measures form the analytical core of the dashboard. They enable both static reporting and dynamic scenario planning, directly supporting business decisions around inventory, regional performance, and growth targets.

Last updated: April 2026

