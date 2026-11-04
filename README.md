# Sales Analytics Dashboard | Microsoft Excel

An interactive retail sales analytics dashboard built in Microsoft Excel to track revenue KPIs, analyze customer segments, and evaluate multi-channel sales performance across 300,000+ transaction records.

---

## Project Overview

In retail sales, large volumes of transactional data often obscure high-level trends, customer behavior, and operational bottlenecks. The objective of this project was to transform raw, multi-attribute retail data into a dynamic, decision-ready analytics dashboard.

By cleaning and structuring over 300,000 records, I built an interactive executive dashboard in Microsoft Excel that allows business stakeholders to monitor financial KPIs, examine monthly revenue trends, evaluate product category and brand performance, and inspect customer purchasing patterns across geographic regions.

---

## Dataset

- **Total Records:** 302,010 rows
- **Total Attributes:** 30 columns
- **Key Fields:**
  - **Transaction & Customer:** `Transaction_ID`, `Customer_ID`, `Name`, `Email`, `Phone`, `Address`, `City`, `State`, `Zipcode`, `Country`, `Age`, `Gender`, `Income`, `Customer_Segment`
  - **Order Details:** `Date`, `Year`, `Month`, `Time`, `Shipping_Method`, `Payment_Method`, `Order_Status`
  - **Product & Financials:** `Product_Category`, `Product_Brand`, `Product_Type`, `products`, `Total_Purchases`, `Amount`, `Total_Amount`, `Ratings`, `Feedback`

---

## Tools & Skills Used

- **Microsoft Excel**
  - **Lookup & Reference Functions:** `XLOOKUP`, `VLOOKUP`, `INDEX-MATCH` for data mapping, validation, and table consolidation
  - **Data Summarization & Modeling:** Pivot Tables, custom date grouping, calculated metrics
  - **Data Visualization & KPI Reporting:** Pivot Charts (Line, Column, Doughnut charts), custom dynamic KPI cards
  - **Interactivity:** Multi-criteria Slicers (Country, Gender, Year, Shipping Method) and worksheet navigation controls

---

## Data Cleaning Steps

1. **Handling Missing & Inconsistent Values:** Identified and handled blank or unrecorded entries across demographic and geographic attributes by standardizing them (e.g., categorized missing entries as "Unknown") to maintain reporting consistency without dropping transaction volume.
2. **Date & Time Formatting:** Structured raw timestamps into dedicated `Date`, `Year`, and `Month` fields to support chronological aggregations and seasonal trend analysis.
3. **Data Mapping with Lookup Functions:** Utilized `XLOOKUP`, `VLOOKUP`, and `INDEX-MATCH` to cross-reference customer profiles, map brand categories, and join transactional details across data sheets.
4. **Data Type Normalization:** Converted and formatted financial fields (`Amount`, `Total_Amount`), quantities (`Total_Purchases`), and ratings into consistent numerical and currency formats to enable accurate aggregation in Pivot Tables.
5. **Deduplication & Quality Control:** Audited all 302,010 rows to remove duplicates and verify data integrity before building analytical data models.

---

## Dashboard Preview

### Executive Sales Performance Dashboard

![Sales Performance Dashboard](./screenshots/dashboard_overview.png)

- **What It Shows:** An executive overview of retail sales performance consolidating high-level business metrics, temporal patterns, product categories, brand contributions, regional sales, payment preferences, and customer segments in a single interface.
- **KPIs Displayed:**
  - **Total Revenue:** $402.5M
  - **Total Orders:** 294,462
  - **Avg Rating:** 3.2 / 5.0
  - **Avg Orders:** 5.36
- **Charts & Visualizations:**
  - **Monthly Revenue Trend (Line Chart):** Tracks monthly sales performance throughout the year, highlighting peaks in April ($55.1M) and January ($49.6M).
  - **Revenue by Product Category (Column Chart):** Compares total revenue across product lines: Electronics ($95.0M), Grocery ($89.0M), Clothing ($73.0M), Books ($72.7M), and Home Decor ($72.4M).
  - **Top 10 Revenue by Product Brand (Column Chart):** Identifies leading brands, led by Pepsi ($40.5M), Samsung ($24.8M), Sony ($24.5M), Nike ($24.4M), Zara ($24.4M), and Coca-Cola ($24.4M).
  - **Top 10 Revenue by State (Column Chart):** Displays top-performing regions, led by England (61,694), Berlin (51,451), New South Wales (43,959), and Ontario (43,946).
  - **Payment Method Analysis (Doughnut Chart):** Breaks down revenue share across payment methods: Credit Card (30%), Debit Card (26%), Cash (24%), and PayPal (20%).
  - **Order Status Analysis (Doughnut Chart):** Analyzes fulfillment progress: Delivered (43%), Shipped (22%), Processing (19%), and Pending (16%).
  - **Revenue by Customer Segment (Doughnut Chart):** Segments revenue contribution: Regular customers (49%), New customers (30%), and Premium customers (21%).
- **Interactive Slicers & Filtering:**
  - Four interactive slicers allow filtering across all charts and KPI cards simultaneously:
    - **Shipping:** `Express`, `Same-Day`, `Standard`, `Unknown`
    - **Year:** `2023`, `2024`, `Unknown`
    - **Gender:** `Female`, `Male`, `Unknown`
    - **Country:** `Australia`, `Canada`, `Germany`, `UK`, `USA`, `Unknown`
  - Visual buttons on the left facilitate direct navigation between `DASHBOARD`, `SUMMARY`, and `DATA` sheets.

> **[TODO: Add additional close-up screenshots (e.g., `./screenshots/pivot_charts.png`, `./screenshots/slicers.png`) if standalone detail views are desired.]**

---

## Key Insights

- **Top Product Category:** **Electronics** generated the highest total revenue at **$95.0M**, followed closely by **Grocery** at **$89.0M**.
- **Preferred Payment Method:** **Credit Card** is the most popular payment method, driving **30%** of total sales, followed by Debit Card (**26%**) and Cash (**24%**).
- **Leading Regional Markets:** **England** (61,694) and **Berlin** (51,451) generated the highest regional volume.
- **Primary Customer Segment:** **Regular** customers accounted for the largest revenue share at **49%**, followed by New (**30%**) and Premium (**21%**).

---
