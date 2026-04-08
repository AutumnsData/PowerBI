# DAX Measures - E-Commerce Sales Dashboard

This file contains all the key DAX measures used in the project, with explanations of what each one does and why it was created. Understanding these measures demonstrates core skills in time intelligence, filter context, and dynamic calculations.

## Basic Aggregations

### Total revenue across all sales:
- Simple aggregation used as the foundation for almost every other measure.
```dax
Total Sales = SUM(FactSales[SalesAmount])
```

### Total number of units sold:
- Useful for volume analysis alongside revenue.
```dax
Total Quantity = SUM(FactSales[Quantity])
```

### Average revenue per order:
- Helps understand typical order size and customer behavior.
```dax
Avg Order Value = 
    DIVIDE([Total Sales], DISTINCTCOUNT(FactSales[OrderID]))
```

### Year-to-Date sales total:
 - Resets every January 1st. Critical for tracking annual performance.
```dax
YTD Sales = TOTALYTD([Total Sales], DimDate[Date])
```


