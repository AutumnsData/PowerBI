# E-Commerce Sales Performance Dashboard

**Power BI Dashboard** – Built to analyze multi-year sales data and support data-driven decisions around performance tracking, target setting, inventory planning, and regional focus.

### Project Overview
This interactive dashboard explores sales trends across categories, products, time periods, and regions using a realistic e-commerce dataset. It demonstrates end-to-end skills in data modeling, DAX calculations, interactivity, and business storytelling.

The dashboard helps answer key business questions such as:
- Which categories and products are driving revenue?
- How are sales accumulating over time, and what happens if we need to hit higher targets?
- Which regions/countries are performing best?
- Where should we focus inventory or marketing efforts?

### Tools & Technologies
- **Power BI Desktop** – Star schema modeling, DAX time intelligence, conditional formatting, What-If parameters, report page tooltips
- **Power Query** – Data cleaning and transformation
- **DAX** – Running totals, YTD, MoM %, YoY %, dynamic adjusted targets
- **GitHub** – Full process documentation with screenshots

# Interactive Power BI Dashboard

Analyzing multi-year sales data to track performance, set targets, optimize inventory, and identify regional opportunities.

### Dashboard Pages

#### 1. Executive Overview
KPI cards, category breakdown donut, and monthly trend with What-If target adjustment.

![Executive Overview](https://github.com/AutumnsData/PowerBI/blob/d6207c0f6f0bdae0572439639d9d1b636bc0f7ab/Ecommerce-Sales-Dashboard/screenshots/Executive%20Overview%20page_Target%20Multiplier%201.5.jpg)

#### 2. Time Analysis
Yearly performance matrix with conditional formatting + running total vs adjusted target chart.

![Time Analysis](https://github.com/AutumnsData/PowerBI/blob/389439faced3977bdb7b9d680d13f706fb04fb83/Ecommerce-Sales-Dashboard/screenshots/Running%20Total%20Sales%20vs%20Adjusted%20Target%20at%20multiplier%201.5%20(50%25%20stretch%20target).jpg)

#### 3. Product Deep Dive
Top 10 SubCategories by Total Sales and Quantity vs Sales scatter with interactive tooltips.

![Product Deep Dive](https://github.com/AutumnsData/PowerBI/blob/1fa5a5039fe15b9272aab8307fb6afb4a634d42d/Ecommerce-Sales-Dashboard/screenshots/Product%20Deep%20Dive.jpg)

#### 4. Regional Performance
Filled map showing Total Sales by country + supporting treemap by country and region.

![Regional Performance](https://github.com/AutumnsData/PowerBI/blob/78ee763d37d61812e2d245c801c6db6d73655fc7/Ecommerce-Sales-Dashboard/screenshots/Regional%20Performance%20Map%20-%20Germany.jpg)

### Additional Screenshots
- [Running Total at multiplier 1.0](https://github.com/AutumnsData/PowerBI/blob/d6207c0f6f0bdae0572439639d9d1b636bc0f7ab/Ecommerce-Sales-Dashboard/screenshots/Executive%20Overview%20page_Target%20Multiplier%201.jpg)
- [Running Total at multiplier 1.5](https://github.com/AutumnsData/PowerBI/blob/d6207c0f6f0bdae0572439639d9d1b636bc0f7ab/Ecommerce-Sales-Dashboard/screenshots/Executive%20Overview%20page_Target%20Multiplier%201.5.jpg)
- [Regional Performance Map - France](https://github.com/AutumnsData/PowerBI/blob/d6207c0f6f0bdae0572439639d9d1b636bc0f7ab/Ecommerce-Sales-Dashboard/screenshots/Regional%20Performance%20Map%20-%20France.jpg)

### Key Features & Skills Demonstrated
- Star schema data modeling with marked Date table
- Advanced DAX (running totals, YTD, MoM %, YoY %, What-If parameters)
- Conditional formatting, Top N filtering, and cross-visual interactions
- Geographic analysis using Filled Map and Treemap
- Interactive tooltips and slicers

### Repository Structure
- `data/` – Sample data files
- `screenshots/` – Process and final visuals
- `DAX_Measures.md` – Key DAX measures with explanations
- `insights.md` – Business insights from the dashboard
- `Ecommerce-Sales-Dashboard-2.pbix` – Main Power BI file

### How to View
1. Open the `.pbix` file in Power BI Desktop (free).
2. Use the slicers and What-If parameter to explore interactivity.
3. All pages are fully connected via filters and cross-highlighting.

### Key Insights
- On the Product Deep Dive page, there are two main visuals. The bar chart on the left shows the top 10 selling subcategories by total value of sales. The scatter plot on the right shows Sales by Category, in relation to the total quantity of items sold on the X axis and total value of category's sales on the Y axis. The size of each bubble denotes the average order value per category - the higher the average order value, the larger the bubble. As shown by the scatter plot, the clothing and accessories categories are high on the Y axis, indicating that the products sold under these categories produced the highest total value in sales out of all categories. The Kitchen category is far to the right on the X axis, indicating that this category sold the highest quantity of products. The Kitchen category being lower on the Y axis than the clothing and accessories categories despite selling the highest number of products indicates that a much larger number of products would have to be sold under the Kitchen category in order to reach the same amount of value in sales as the clothing and accessories categories. When clicking on a category bubble, the bar chart updates to only show subcategories of the selected category. After selecting the clothing category, we find that the Jackets and Pants categories produced the highest total sales in this category. Under the Accessories category, we find that headphones and keyboards returned the highest total sales in value. After selecting the Kitchen category, it is found that utensils surpassed appliances by $1.8m in total sales value. Viewing the Total Value of Sales per category and total quantity of items sold per category allows the business to quickly determine how to focus their inventory efforts, as the business will want to keep their highest selling products in value and quantity in stock.

  
- How are sales accumulating over time, and what happens if we need to hit higher targets?
- The graph on the Time Analysis page shows how running total sales build up month by month. The total starts over at zero every January, which tells me the business measures performance on a calendar-year basis rather than a rolling 12-month window.
If the business wants to aim for 50% higher sales, I can slide the Target Multiplier to 1.5. When I do that, the blue area shows actual running total sales, the purple area shows the adjusted target, and the orange line shows the cumulative gap between them.
For example, in May 2024 the tooltip shows we are already about $2.12 million behind the 1.5x stretch target for the year so far. At that point we had only reached 67% of where we needed to be. This means the business would need significantly stronger sales in the remaining months of 2024 to still hit the full-year stretch goal.

- Which regions/countries are performing best? Where should we focus inventory or marketing efforts?
- The Regional Performance map shows countries with the highest sales performance in purple, while the countries with the lowest sales performance are in light blue. When hovering over these countries, the tooltip shows the sales performance in each region. As such, it can be seen that the regions with the highest sales performance include South & Central India, North & South Saudia Arabia, and the South & North UK. It may be beneficial to focus inventory efforts in these areas.
- The regions with the fewest sales include Germany, North America, Egypt,and France. As such, it may be advisable to improve marketing in these regions so that sales can be expanded.


### About Me
Autumn Bilbao  
B.S. Data Management & Analysis – Western Governors University (2023)  
Passionate about turning raw data into actionable business insights.

---

Last updated: April 2026
