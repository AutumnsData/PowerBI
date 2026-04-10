# E-Commerce Sales Performance Dashboard

## Project Overview
This project builds an interactive dashboard to analyze e-commerce sales performance across multiple years. The goal was to turn raw sales data into clear, actionable insights for tracking revenue trends, comparing performance over time, spotting strong and weak product categories, and supporting decisions around inventory and regional focus.

I used the **Complete DAX Practice Dataset** from Kaggle (multi-year sales with customers, products, geographies, and dates). This let me practice realistic business scenarios similar to the sales trend work I've done with Shopify data and the category analysis from my earlier movie rental project.

The dashboard answers questions like:
- How are sales growing month-over-month and year-over-year?
- Which categories and regions are driving performance?
- What are the running totals and seasonal patterns?

I also rebuilt key visuals in Tableau to compare the two tools side-by-side.

## Key Features
- Star schema data model with a dedicated Date table
- Advanced DAX measures for time intelligence (YTD, YoY, MoM growth, running totals)
- Interactive slicers for year, month, category, and region
- KPI cards, trend lines, regional maps/treemaps, top product rankings, and drill-through pages
- Dynamic titles and what-if parameters for scenario testing
- Clean, professional layout with conditional formatting

## Tools & Technologies
- **Power BI Desktop** – Data modeling, DAX calculations, dashboard creation
- **Power Query** – Data cleaning and transformation
- **DAX** – Time intelligence, variables (VAR), CALCULATE, ranking, and dynamic measures
- **Tableau Desktop/Public** – Rebuilt select visuals for comparison (LODs, table calculations, parameters)
- GitHub – Version control with .pbip format for better tracking of changes

## Repository Structure
Ecommerce-Sales-Dashboard/
├── data/                  # Raw and cleaned files (small samples only)
├── screenshots/           # Dashboard page images
├── DAX_Measures.md        # Key DAX code with explanations
├── insights.md            # Business insights and recommendations
├── Ecommerce_Sales_Report.pbip   # Main Power BI project file
├── Tableau_Version/       # Packaged .twbx workbook + related files
└── README.md

## How to View the Dashboard
1. Download and open the `.pbip` file in **Power BI Desktop** (free).
2. Tableau version: [To Be Made]

## Sample Insights
(You'll fill this in once the dashboard is built – here's a template based on typical findings)

- Overall sales showed strong YoY growth in Q4, driven primarily by one high-performing category.
- Region X consistently lagged in MoM growth – opportunity to adjust marketing or inventory allocation.
- Top 5 products accounted for over 40% of total revenue; running totals highlight seasonal spikes.
- Recommendation: Increase stock in high-growth categories by X% ahead of peak seasons to avoid lost sales.

## What I Learned / Skills Demonstrated
- Building a proper star schema and marking a Date table for time intelligence
- Writing reusable, performant DAX measures using VAR and CALCULATE
- Creating dynamic, user-friendly dashboards with slicers, bookmarks, and drill-through
- Comparing Power BI (model-first approach) vs Tableau (visual-first with LODs)
- Documenting work clearly for technical and non-technical audiences

This project builds directly on my WGU coursework (movie rental automation in SQL, YouTube tags analysis in Tableau, data wrangling in Python) and my hands-on experience maintaining product listings and sales trends on Shopify.

## Future Improvements
- Add forecasting visuals
- Implement row-level security
- Connect to a live data source
- Expand with customer segmentation

## About Me
Autumn Bilbao – Data Analyst  
B.S. Data Management & Analysis, Western Governors University (Nov 2023)  
Experience in process automation, cross-functional collaboration, and turning data into decisions.

Feel free to reach out if you have questions or suggestions!

---

Last updated: April 2026
