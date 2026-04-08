# DAX Measures - E-Commerce Sales Dashboard

This file contains all the key DAX measures used in the project, with explanations of what each one does and why it was created. Understanding these measures demonstrates core skills in time intelligence, filter context, and dynamic calculations.

## Basic Aggregations

```dax
Total Sales = SUM(FactSales[SalesAmount])```

```dax
Total Quantity = SUM(FactSales[Quantity])```

```dax
Avg Order Value = 
    DIVIDE([Total Sales], DISTINCTCOUNT(FactSales[OrderID]))```

```dax
YTD Sales = TOTALYTD([Total Sales], DimDate[Date])```
