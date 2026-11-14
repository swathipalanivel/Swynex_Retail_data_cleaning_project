# Online Retail Sales Analysis Dashboard

## Project Overview
This project explores the UCI Online Retail transaction dataset and presents sales performance in an interactive Tableau Public dashboard. The aim is to make sales trends, product performance, country contribution, customer activity, and returns easier to understand.

> **Before publishing:** Replace every item marked `TODO` with values and screenshots from your own completed Tableau workbook. Do not publish estimated or unverified KPI values.

## Business Questions
- How does revenue change month by month?
- Which products generate the highest revenue?
- Which countries contribute most to revenue?
- How many orders and units are recorded?
- How many unique customers are represented?
- How does the quantity of returned items change over time?

## Tools Used
- Python / Pandas — data preparation (if used in your workflow)
- Tableau Public — interactive visualisation and dashboard
- CSV — cleaned data source

## Dataset
The project uses the Online Retail dataset, containing transaction-level records with fields such as `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, and `Country`.

## Data Preparation
The dataset was prepared for analysis. The project workflow includes checking missing values and duplicates, confirming data types, and creating a revenue measure from quantity and unit price.

**Sales Revenue calculation used in Tableau:**
```tableau
IF [Quantity] > 0
AND [UnitPrice] > 0
AND LEFT(STR([InvoiceNo]), 1) <> "C"
THEN [Revenue]
END
```
The `[Revenue]` field is calculated as:
```tableau
[Quantity] * [UnitPrice]
```
This measure focuses on positive-quantity, positive-price transactions and excludes invoice numbers beginning with `C`. Returns are analysed separately using negative quantities.

## Dashboard KPIs
- Total Sales Revenue — `SUM([Sales Revenue])`
- Total Orders — `COUNTD([InvoiceNo])`
- Units Sold — `SUM([Quantity])` (confirm whether the worksheet is filtered to sales-only transactions)
- Unique Customers — `COUNTD([CustomerID])`, excluding null CustomerID
- Average Order Value — `SUM([Sales Revenue]) / COUNTD([InvoiceNo])`

## Visualisations
1. Monthly Sales Trend — monthly revenue over time
2. Top 10 Products — products ranked by sales revenue
3. Revenue by Country — revenue contribution by country
4. Returns Analysis — returned quantity over time

## Interactivity
The dashboard is designed to include useful filters such as date and country. Add and test any additional filters you have implemented before describing them as available.

## Key Findings
Add at least three findings after checking your actual Tableau results:
1. TODO — highest-revenue month and its value.
2. TODO — leading country and its share/value.
3. TODO — top product by revenue.
4. TODO — notable pattern in returns.

## Dashboard Preview
TODO — Add a screenshot of your final Tableau dashboard here.

## How to View
- Open the published Tableau Public workbook: TODO — paste your Tableau Public URL.
- Or download the workbook from Tableau Public if you have enabled downloads.

## Author
Swathi Palanivel

## Notes
This is a portfolio learning project. KPI definitions and filters should be checked against the workbook before interpreting the results. In particular, verify whether Units Sold and Total Orders exclude returns/cancellations consistently.
