# 💚 Excel_Interactive__SalesScope_Dashboard

## 📌 Project Overview

This project presents an interactive **Microsoft Excel sales and profitability dashboard** for analyzing business performance across customer segments, product categories, sub-categories, cities, and years. It transforms a structured retail sales dataset into an executive reporting view that summarizes sales, profit, year-over-year (YoY) growth, quarterly sales trends, and geographic performance.

The dashboard is designed to help users compare the latest year's performance with the previous year, identify high-performing and declining product sub-categories and cities, monitor quarterly sales patterns, and explore the leading states by all-time sales. Its visual design uses a teal-and-green color palette, KPI cards, interactive slicers, comparison tables, and complementary charts.

> **Dashboard Preview:**
> <img width="1630" height="879" alt="Excel_Interactive__SalesScope_Dashboard  " src="https://github.com/user-attachments/assets/08e6e1ba-703d-4d7d-b4ce-73775929101d" />
> *The dashboard screenshot features six KPI cards, segment and category slicers, sub-category and city comparison tables, a quarterly sales and average-sales-per-unit combination chart, and a top-ten states-by-sales column chart.*

---

## 🗂️ Workbook Architecture

The workbook, `Excel_Interactive__SalesScope_Dashboard.xlsx`, is organized into three worksheets:

1. **Sales_Data** – The source dataset containing order and shipping details, customer information, geography, product details, sales, quantity, discount, and profit.
2. **Analysis** – The supporting calculation and summary layer. It contains PivotTables and supporting formulas for yearly sales and profit, YoY growth, product sub-category and city comparisons, quarterly sales and quantity, and state-level sales.
3. **Sales_Dashboard** – The presentation layer containing KPI cards, comparison tables, interactive slicers, and charts.

---

## 🔄 Data Structure & Preparation

The `Sales_Data` worksheet contains **9,994 sales records** and 21 source fields. The records cover **2014 through 2017** and describe retail orders in the United States.

The dataset includes the following business fields:

- **Row ID:** Unique row identifier.
- **Order ID:** Order identifier.
- **Order Date:** Date the order was placed.
- **Ship Date:** Date the order was shipped.
- **Ship Mode:** Shipping method used for the order.
- **Customer ID:** Customer identifier.
- **Customer Name:** Customer name.
- **Segment:** Consumer, Corporate, or Home Office.
- **Country:** Country associated with the order.
- **City:** City associated with the order.
- **State:** State associated with the order.
- **Postal Code:** Postal code associated with the order.
- **Region:** Sales region.
- **Product ID:** Product identifier.
- **Category:** Furniture, Office Supplies, or Technology.
- **Sub-Category:** Product sub-category, such as Phones, Chairs, Storage, Binders, and Tables.
- **Product Name:** Product description.
- **Sales:** Sales amount for the order line.
- **Quantity:** Number of units sold.
- **Discount:** Discount applied to the order line.
- **Profit:** Profit recorded for the order line.

The source data is formatted as an Excel Table named `tbl_Sales_Data`, providing a structured data source for the workbook's analysis.

**Dataset note:** The workbook contains 9,994 transaction records, with 21 columns in the source table.

### Overall Dataset Metrics

The following figures summarize the full 2014–2017 dataset, rather than only the two years highlighted in the dashboard KPI cards.

| Metric | Total |
|---|---:|
| **Sales** | **$2,297,200.86** |
| **Profit** | **$286,397.02** |
| **Quantity Sold** | **37,873** |


---

## 📊 Key Metrics & Executive KPIs

The dashboard presents six headline indicators comparing **2017 (Latest Year)** with **2016 (Last Year)**.

| KPI | 2017 | 2016 | YoY Growth |
|---|---:|---:|---:|
| **Sales** | **$733,215.26** | **$609,205.60** | **20.4%** |
| **Profit** | **$93,439.27** | **$81,795.17** | **14.2%** |

### Sales Performance

- **Latest Year Sales:** $733,215.26 in 2017.
- **Last Year Sales:** $609,205.60 in 2016.
- **Sales Growth vs PY:** Sales increased by approximately **20.4%** compared with 2016.

### Profit Performance

- **Latest Year Profit:** $93,439.27 in 2017.
- **Last Year Profit:** $81,795.17 in 2016.
- **Profit Growth vs PY:** Profit increased by approximately **14.2%** compared with 2016.

Sales growth exceeded profit growth during 2017, making the relationship between revenue growth and profitability an important area to monitor.

### Sales by Sub-Category

The dashboard compares sales for each product sub-category in 2017 and 2016, together with its YoY growth rate.

The displayed comparison includes:

- Phones
- Chairs
- Storage
- Binders
- Tables
- Copiers
- Accessories
- Machines
- Appliances
- Furnishings

The total shown in the comparison table is **$642,486.40 for 2017** versus **$533,512.49 for 2016**, representing approximately **20.4% growth**.

### Sales by City

The city comparison table presents 2017 and 2016 sales with YoY growth for:

- New York City
- Los Angeles
- Seattle
- Philadelphia
- San Francisco
- Detroit
- Houston
- Chicago
- Columbus
- Lafayette

The displayed city-table total is **$266,183.68 for 2017** versus **$339,408.45 for 2016**, representing approximately **27.5% decline** based on the values shown in the workbook.

### Quarterly Sales & Price Trend

The combination chart compares quarterly sales across 2014, 2015, 2016, and 2017. Sales are displayed as columns, while the line represents the calculated **average sales per unit** (`Sales / Quantity`).

The chart makes it possible to compare seasonal patterns and changes in sales activity across the four-year period.

### States With Highest All-Time Sales

The column chart ranks the ten states with the highest total sales across the dataset.

The leading states shown are:

1. **California:** approximately $458K
2. **New York:** approximately $311K
3. **Texas:** approximately $170K
4. **Washington:** approximately $139K
5. **Pennsylvania:** approximately $117K
6. **Florida:** approximately $89K
7. **Illinois:** approximately $80K
8. **Ohio:** approximately $78K
9. **Michigan:** approximately $76K
10. **Virginia:** approximately $71K

California and New York lead the state-level sales ranking in the supplied dataset.

---

## 🖥️ Dashboard Features & User Experience

- **Executive KPI Cards:** Six cards display Sales Latest Year, Sales Last Year, Sales Growth vs PY, Profit Latest Year, Profit Last Year, and Profit Growth vs PY.
- **Segment Slicers:** Interactive filters for Consumer, Corporate, and Home Office.
- **Category Slicers:** Interactive filters for Furniture, Office Supplies, and Technology.
- **Shipping Mode Slicers:** Filters for First Class, Same Day, Second Class, and Standard Class.
- **Sub-Category Comparison Tables:** Compare 2017 and 2016 sales by product sub-category, including YoY growth.
- **City Comparison Tables:** Compare 2017 and 2016 sales by city, including YoY growth.
- **Quarterly Sales & Price Trend:** A combination chart visualizes quarterly sales and average sales per unit from 2014 to 2017.
- **Top States by Sales:** A column chart ranks the ten states with the highest all-time sales.
- **Selective Slicer Connections:** Slicers are connected to specific PivotTables and dashboard sections, allowing different parts of the dashboard to be filtered independently.
- **Conditional Growth Indicators:** Green upward indicators and red downward indicators distinguish positive and negative YoY changes.
- **Consistent Visual Identity:** Teal KPI cards, light-teal slicers, a central brand mark, and consistent chart formatting create a cohesive dashboard.

---

## 🛠️ Tools & Excel Features Used

- **Microsoft Excel:** Data organization, calculations, analysis, and dashboard development.
- **Excel Tables:** Structured the source data as `tbl_Sales_Data`.
- **PivotTables:** Aggregated sales and profit by year, sub-category, city, quarter, and state.
- **Slicers:** Added interactive filtering for customer segment, product category, and shipping mode.
- **PivotTable Report Connections:** Controlled which PivotTables respond to each slicer.
- **GETPIVOTDATA:** Retrieved values from PivotTables for supporting calculations.
- **Excel Formulas:** Calculated YoY growth and prepared dashboard-ready values.
- **Year-over-Year Analysis:** Compared current-year values with previous-year values using growth-rate calculations.
- **Calculated Measures:** Derived average sales per unit using `Sales / Quantity`.
- **Combination Chart:** Combined quarterly sales columns with an average-sales-per-unit line.
- **Column Chart:** Visualized the ten states with the highest all-time sales.
- **Conditional Formatting & Custom Number Formats:** Used visual indicators and number formatting to distinguish positive and negative growth.
- **Shapes & Text Boxes:** Built the KPI cards and dashboard layout.
- **Linked Shape Values:** Connected KPI card displays to worksheet cell values.
- **Dashboard Design & Formatting:** Applied a consistent color palette, alignment, spacing, and visual hierarchy.

---

## ⚙️ How to Use

1. Download `Excel_Interactive__SalesScope_Dashboard.xlsx`.
2. Open the workbook in desktop **Microsoft Excel** for the intended dashboard and interactive filtering experience.
3. Navigate to the **Sales_Dashboard** worksheet to view the executive dashboard.
4. Use the **Segment** slicers to filter by Consumer, Corporate, or Home Office.
5. Use the **Category** slicers to filter by Furniture, Office Supplies, or Technology.
6. Use the **Ship Mode** slicers to filter by First Class, Same Day, Second Class, or Standard Class.
7. Review the KPI cards to compare 2017 sales and profit with 2016.
8. Explore the sub-category and city tables to identify changes in sales and YoY growth.
9. Review the quarterly sales trend and the top states by all-time sales.
10. Navigate to **Analysis** to inspect the supporting PivotTables and calculations, or to **Sales_Data** to review the original transaction records.

*Note: Slicers are connected selectively to the workbook's PivotTables. Different slicers therefore affect their assigned dashboard sections rather than necessarily filtering every element at once.*

---

## 🎓 Learning Resource

This project was developed by following the Skillnator YouTube tutorial:

[Watch the Excel Interactive Dashboard Tutorial](https://www.youtube.com/watch?v=eaSg0mu6nLM)

The tutorial served as the learning resource for building the dashboard and applying interactive Excel dashboard techniques.

---

## 📁 Project Files

| File | Description |
|---|---|
| `Excel_Interactive__SalesScope_Dashboard.xlsx` | Excel workbook containing the source data, analysis, and interactive dashboard. |
| `README.md` | Project documentation. |
| `dashboard-preview.png` | Screenshot of the completed dashboard. |

---

*Built with Microsoft Excel | PivotTables | Slicers | GETPIVOTDATA | Excel Formulas | Data Visualization*
