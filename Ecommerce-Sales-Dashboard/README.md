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
- As shown by the graphs on the Product Deep Dive page, the key categories include Clothing and Acessories. The top performers under clothing include jackets and pants. On average, the order value for jackets was about $1.01k, while the average order value for pants was about $780. The top performers under Accessories include headsets at an average order value of $816 and keyboards with an average order value of $693.

- How are sales accumulating over time, and what happens if we need to hit higher targets?
- The graph on the Time Analysis page shows how running total sales build up month by month. The total starts over at zero every January, which tells me the business measures performance on a calendar-year basis rather than a rolling 12-month window.
If the business wants to aim for 50% higher sales, I can slide the Target Multiplier to 1.5. When I do that, the blue area shows actual running total sales, the purple area shows the adjusted target, and the orange line shows the cumulative gap between them.
For example, in May 2024 the tooltip shows we are already about $2.12 million behind the 1.5x stretch target for the year so far. At that point we had only reached 67% of where we needed to be. This means the business would need significantly stronger sales in the remaining months of 2024 to still hit the full-year stretch goal.

- Which regions/countries are performing best? Where should we focus inventory or marketing efforts?
- According to the graphs and map on the Regional Performance tab, the regions and countries that perform the best include South & Central India, North & South Saudi Arabia, and South & North UK. This indicates that there the business's products may be popular in these regions, while also showing that there may be room to grow in Germany, North America, Egypt, and France. As such, it may be advisable to improve marketing in the regions where there is room to grow, while inventory could likely be expanded in areas where the business's products are already popular.


### About Me
Autumn Bilbao  
B.S. Data Management & Analysis – Western Governors University (2023)  
Passionate about turning raw data into actionable business insights.

---

Last updated: April 2026
