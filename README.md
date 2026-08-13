# Superstore Sales Performance Dashboard

An interactive Power BI dashboard analyzing retail sales performance across
regions, categories, and time — built on the Sample Superstore dataset
(9,994 cleaned records, 2015–2018).

## Dashboard Preview

**KPI Cards:** Total Sales (2.30M) · Total Profit (286.40K) · Profit Margin % (12.47%)

**Visuals included:**
- Sales by Category (Technology, Furniture, Office Supplies)
- Profit by Region (Central, East, South, West)
- Sales Trend by Year (2015–2018)
- Sales by Sub-Category (Treemap breakdown)
- Interactive Slicers for Category and Region — filter the entire dashboard live

## Data Preparation

The raw dataset was cleaned in **Excel** before being imported into Power BI:
- Removed 806 blank rows and checked for duplicate records using Power Query
- Fixed data types (dates, postal codes) and trimmed whitespace across text columns
- Filled missing postal codes using verified reference data
- Built a pivot-style sales/profit summary using SUMIFS formulas
- Built a region lookup table using INDEX/MATCH (functionally equivalent to XLOOKUP)
- Final cleaned dataset: 9,994 rows, ready for analysis

## Tools Used

**Excel** — Power Query, Pivot Tables, SUMIFS, INDEX/MATCH
**Power BI Desktop** — DAX measures, interactive visuals, slicers, data modeling

## Key Insights

- **West region** generates significantly higher profit than Central despite
  comparable order volumes — worth investigating regional pricing or cost
  structures behind the gap
- **Sales grew steadily from 2015–2018**, with growth accelerating sharply
  after 2016 — nearly doubling by 2018
- **Technology** leads in total sales among the three categories, while
  **Phones and Chairs** are the top-performing sub-categories driving revenue
- Sub-category analysis reveals meaningful variation within categories that
  isn't visible at the top-level Category breakdown alone

## Files

- `Sample_Superstore_Raw.csv` — original raw dataset (10,800 rows, before cleaning)
- `Superstor_Cleaned.xlsx` — cleaned dataset (9,994 rows) with Excel-based
  analysis (Power Query steps, pivot summary, lookup table)
- `Sales Dashboard.pbix` — final interactive Power BI dashboard

## How to Use

1. Open `Sales Dashboard.pbix` in Power BI Desktop
2. Use the Category and Region slicers (top-right) to filter the dashboard
3. Hover over any chart element for detailed tooltips
