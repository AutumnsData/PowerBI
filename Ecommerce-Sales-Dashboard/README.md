# E-Commerce Sales Performance Dashboard

**Power BI Dashboard** – Built to analyze multi-year sales data and support data-driven decisions around performance tracking, target setting, inventory planning, and regional focus.

### Project Overview
This interactive dashboard explores sales trends across categories, products, time periods, and regions using a realistic e-commerce dataset. It demonstrates end-to-end skills in data modeling, DAX calculations, interactivity, and business storytelling.

The dashboard helps answer key business questions such as:
- Which categories and products are driving revenue?
- How are sales accumulating over time, and what happens if we need to hit higher targets?
- Which regions/countries are performing best?
- Where should we focus inventory or marketing efforts?

### Key Features
- **Executive Overview**: KPI cards, category donut, and monthly trend with What-If target adjustment
- **Time Analysis**: Yearly matrix with conditional formatting + running total area chart vs adjusted target
- **Product Deep Dive**: Top 10 SubCategories by sales + Quantity vs Sales scatter with tooltips
- **Regional Performance**: Filled map colored by Total Sales + supporting treemap by country and region

### Tools & Technologies
- **Power BI Desktop** – Star schema modeling, DAX time intelligence, conditional formatting, What-If parameters, report page tooltips
- **Power Query** – Data cleaning and transformation
- **DAX** – Running totals, YTD, MoM %, YoY %, dynamic adjusted targets
- **GitHub** – Full process documentation with screenshots

### Repository Structure
Ecommerce-Sales-Dashboard/
├── data/                     # Sample data files
├── screenshots/              # Process and final visuals
├── DAX_Measures.md           # Key DAX measures with explanations
├── insights.md               # Business insights from the dashboard
├── Ecommerce-Sales-Dashboard-2.pbix   # Main Power BI file
└── README.md

### How to View
1. Open the `.pbix` file in Power BI Desktop (free).
2. Use the slicers and What-If parameter to explore interactivity.
3. All pages are fully connected via filters and cross-highlighting.

### Key Insights
(You'll add 3–5 real insights here once you review the final dashboard — examples below)
- Strong mid-year sales peaks suggest seasonal inventory planning opportunities.
- Electronics and Furniture consistently drive the highest revenue.
- Running totals show clear annual resets with strong recovery in Q3/Q4 of 2024.
- Certain regions show significantly higher sales concentration — potential focus areas for expansion.

### What I Learned
- Built a proper star schema with a marked Date table to enable reliable time intelligence.
- Used What-If parameters and running totals to create dynamic “what-if” target scenarios.
- Applied conditional formatting and Top N filters to make insights scannable.
- Balanced interactivity with clean design across four connected pages.

### Future Improvements
- Add forecasting visuals
- Implement row-level security
- Connect to a live data source
- Expand with customer segmentation analysis

### About Me
Autumn Bilbao  
B.S. Data Management & Analysis – Western Governors University (2023)  
Passionate about turning raw data into actionable business insights.

---

Last updated: April 2026
