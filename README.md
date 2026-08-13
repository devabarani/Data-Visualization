# Global Superstore Power BI Dashboard

## 📊 Project Overview

This project presents an interactive **Power BI dashboard** built using
the **Global Superstore** dataset. The dashboard focuses on sales,
profit, quantity, customers, regions, products, discounts, shipping
modes, and shipping costs.

The project demonstrates how Power BI can be used to transform raw
business data into meaningful visual insights for sales and business
analysis.

## 🎯 Objectives

-   Analyze sales and profit across categories and sub-categories.
-   Identify the top-performing products and states based on sales.
-   Compare quantity and profit across sub-categories.
-   Analyze sales by region and market.
-   Understand profit performance by category and region.
-   Compare sales and quantity across customer segments.
-   Study the relationship between discount and profit.
-   Analyze sales based on different shipping modes.
-   Compare shipping costs across regions and shipping modes.

## 🗂️ Dataset

**Dataset:** Global Superstore

**File:** `Global_Superstore(CSV).csv`

The dataset contains **1,000 records and 24 columns**.

### Main Columns

  Column           Description
  ---------------- -------------------------------------
  Order ID         Unique order identifier
  Order Date       Date on which the order was placed
  Ship Date        Date on which the order was shipped
  Ship Mode        Shipping method
  Customer ID      Unique customer identifier
  Customer Name    Customer name
  Segment          Customer segment
  City             Customer city
  State            Customer state
  Country          Customer country
  Region           Geographic region
  Market           Market classification
  Category         Product category
  Sub-Category     Product sub-category
  Product Name     Product name
  Sales            Sales amount
  Quantity         Quantity of products sold
  Discount         Discount applied
  Profit           Profit generated
  Shipping Cost    Cost of shipping
  Order Priority   Order priority

## 🛠️ Tools Used

-   **Power BI Desktop**
-   **Power Query** for data loading and preparation
-   **DAX** for measures
-   **CSV** dataset
-   **GitHub** for project documentation and version control

## 📈 Dashboard Visualizations

The dashboard contains the following 10 visualizations:

  ------------------------------------------------------------------------
                           No. Analysis              Visualization
  ---------------------------- --------------------- ---------------------
                             1 Sales and Profit by   Matrix / Clustered
                               Category and          Bar Chart
                               Sub-Category          

                             2 Top 10 Products based Bar Chart
                               on Sales              

                             3 Quantity and Profit   Combo Chart
                               by Sub-Category       

                             4 Sales by Region and   Stacked Column Chart
                               Market                

                             5 Profit by Category    Matrix / Heatmap
                               and Region            

                             6 Sales and Quantity by Combo Chart
                               Customer Segment      

                             7 Top 10 States based   Bar Chart
                               on Sales              

                             8 Relationship between  Scatter Chart
                               Discount and Profit   

                             9 Sales by Category for Stacked Bar Chart
                               Each Ship Mode        

                            10 Shipping Cost by      Clustered Column
                               Region and Ship Mode  Chart
  ------------------------------------------------------------------------

## 🧮 DAX Measures

The following measures can be created in Power BI:

``` dax
Total Sales = SUM('Global Superstore'[Sales])

Total Profit = SUM('Global Superstore'[Profit])

Total Quantity = SUM('Global Superstore'[Quantity])

Total Shipping Cost = SUM('Global Superstore'[Shipping Cost])
```

> Replace `'Global Superstore'` with the actual table name displayed in
> Power BI if it is different.

## 🔧 Data Preparation

The basic Power BI workflow used in this project is:

1.  Open **Power BI Desktop**.
2.  Select **Get Data → Text/CSV**.
3.  Import `Global_Superstore(CSV).csv`.
4.  Check data types in Power Query.
5.  Verify fields such as Sales, Profit, Quantity, Discount, and
    Shipping Cost are numeric.
6.  Verify Order Date and Ship Date are date fields.
7.  Apply required transformations.
8.  Load the data into the Power BI model.
9.  Create DAX measures.
10. Build the 10 required visualizations.
11. Format the dashboard and add slicers/interactions.
12. Save the Power BI report as a `.pbix` file.

## 📊 Visualization Details

### 1. Sales and Profit by Category and Sub-Category

-   **Rows / Axis:** Category, Sub-Category
-   **Values:** Total Sales, Total Profit
-   **Visual:** Matrix or clustered bar chart

### 2. Top 10 Products Based on Sales

-   **Axis:** Product Name
-   **Value:** Total Sales
-   Apply a **Top N = 10** filter.

### 3. Quantity and Profit by Sub-Category

-   **Axis:** Sub-Category
-   **Column Value:** Total Quantity
-   **Line Value:** Total Profit
-   **Visual:** Line and clustered column chart

### 4. Sales by Region and Market

-   **Axis:** Region
-   **Value:** Total Sales
-   **Legend:** Market
-   **Visual:** Stacked column chart

### 5. Profit by Category and Region

-   **Rows:** Category
-   **Columns:** Region
-   **Values:** Total Profit
-   **Visual:** Matrix
-   Conditional formatting can be used to create a heatmap effect.

### 6. Sales and Quantity by Customer Segment

-   **Axis:** Segment
-   **Column Value:** Total Sales
-   **Line Value:** Total Quantity
-   **Visual:** Combo chart

### 7. Top 10 States Based on Sales

-   **Axis:** State
-   **Value:** Total Sales
-   Apply a **Top N = 10** filter.

### 8. Relationship Between Discount and Profit

-   **X-axis:** Discount
-   **Y-axis:** Profit
-   **Size:** Sales
-   **Details:** Product Name or Sub-Category
-   **Visual:** Scatter chart

### 9. Sales by Category for Each Ship Mode

-   **Axis:** Category
-   **Value:** Total Sales
-   **Legend:** Ship Mode
-   **Visual:** Stacked bar chart

### 10. Shipping Cost by Region and Ship Mode

-   **Axis:** Region
-   **Value:** Total Shipping Cost
-   **Legend:** Ship Mode
-   **Visual:** Clustered column chart

## 📁 Suggested GitHub Repository Structure

``` text
Global-Superstore-PowerBI/
│
├── README.md
├── Global_Superstore(CSV).csv
├── Global_Superstore_Dashboard.pbix
└── screenshots/
    ├── dashboard.png
    ├── top-products.png
    ├── profit-analysis.png
    └── shipping-analysis.png
```

## 💡 Key Business Questions

This dashboard helps answer questions such as:

-   Which categories and sub-categories generate the most sales?
-   Which products are the top 10 by sales?
-   Which regions and markets contribute the most revenue?
-   Which categories generate the highest profit?
-   Which customer segment has the highest sales?
-   Which states are the strongest sales performers?
-   Does discount have an impact on profit?
-   Which shipping modes generate the highest sales?
-   Which regions have the highest shipping costs?

## 🚀 Future Improvements

-   Add interactive slicers for **Year, Region, Market, Category,
    Segment, and Ship Mode**.
-   Add KPI cards for **Total Sales, Total Profit, Total Quantity, and
    Total Shipping Cost**.
-   Add time-series analysis of sales and profit.
-   Add drill-through pages for product and customer analysis.
-   Add tooltips for detailed business insights.
-   Publish the report to **Power BI Service** for sharing and
    collaboration.

## 👨‍💻 Project

**Project Title:** Global Superstore Sales Analysis using Power BI

**Domain:** Data Analytics / Business Intelligence

**Tool:** Microsoft Power BI

**Dataset:** Global Superstore

------------------------------------------------------------------------

⭐ If you find this project useful, consider giving the repository a
star!
