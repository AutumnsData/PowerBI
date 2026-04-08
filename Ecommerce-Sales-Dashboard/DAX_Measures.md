# DAX Measures - E-Commerce Sales Dashboard

This file contains all the key DAX measures used in the project, with explanations of what each one does and why it was created. Understanding these measures demonstrates core skills in time intelligence, filter context, and dynamic calculations.

## Basic Aggregations

### Total revenue across all sales:
```dax
Total Sales = SUM(FactSales[SalesAmount])
```
- Simple aggregation used as the foundation for almost every other measure.

### Total number of units sold:
```dax
Total Quantity = SUM(FactSales[Quantity])
```
- Useful for volume analysis alongside revenue.

### Average revenue per order:
```dax
Avg Order Value = 
    DIVIDE([Total Sales], DISTINCTCOUNT(FactSales[OrderID]))
```
- Helps understand typical order size and customer behavior.

### Year-to-Date sales total:
```dax
YTD Sales = TOTALYTD([Total Sales], DimDate[Date])
```
 - Resets every January 1st. Critical for tracking annual performance.

