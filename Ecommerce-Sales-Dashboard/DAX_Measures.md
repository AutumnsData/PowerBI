# DAX Measures - E-Commerce Sales Dashboard

This file contains all the key DAX measures used in the project, with explanations of what each one does and why it was created. Understanding these measures demonstrates core skills in time intelligence, filter context, and dynamic calculations.

## Basic Aggregations

```dax
Total Sales = SUM(FactSales[SalesAmount])
```
Calculates the total revenue across all sales.
Simple aggregation used as the foundation for almost every other measure.

```dax
Total Quantity = SUM(FactSales[Quantity])
```
Total number of units sold.
Useful for volume analysis alongside revenue.

```dax
Avg Order Value = 
    DIVIDE([Total Sales], DISTINCTCOUNT(FactSales[OrderID]))
```
Average revenue per order.
Helps understand typical order size and customer behavior.

### Year-to-Date sales total:
```dax
YTD Sales = TOTALYTD([Total Sales], DimDate[Date])
```
 - Year-to-Date sales total.
 - Resets every January 1st. Critical for tracking annual performance.

