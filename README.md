# Online Retail Sales Analysis Dashboard

## Project Overview
This project analyzes an online retail dataset and presents the key sales findings in an interactive dashboard built with **Tableau Public**.

The project workflow includes:
1. Data cleaning using Python and Pandas.
2. Exploratory Data Analysis (EDA).
3. KPI and chart development in Tableau.
4. Interactive dashboard creation and publication.

## Tools Used
- Python
- Pandas
- Tableau Public
- CSV dataset
- GitHub

## Dataset
The project uses the UCI Online Retail dataset.

Original dataset columns include:
- InvoiceNo
- StockCode
- Description
- Quantity
- InvoiceDate
- UnitPrice
- CustomerID
- Country

The cleaned dataset also includes a calculated `Revenue` field.

## Data Preparation
The cleaning process includes:
- Checking and handling missing values.
- Checking duplicate records.
- Converting date and numeric columns to suitable data types.
- Reviewing cancelled invoices and returned quantities.
- Creating `Revenue = Quantity × UnitPrice`.

**Important:** Missing CustomerID values and return/cancellation records should be handled according to the analysis purpose. Do not remove them without documenting the reason.

## Dashboard KPIs
The dashboard is designed to include:
- Sales Revenue
- Total Orders
- Units Sold
- Unique Customers
- Average Order Value

## Dashboard Charts
The dashboard is designed to include:
- Monthly Sales Trend
- Top 10 Products by Revenue
- Revenue by Country
- Returns Analysis

## Interactivity
Add and test useful filters such as:
- Invoice Date
- Country
- Product Description

Confirm that each filter affects the intended charts and KPIs before publishing.

## Key Findings
Replace this section with **at least five findings calculated from your final Tableau workbook**.

1. [Add verified finding 1]
2. [Add verified finding 2]
3. [Add verified finding 3]
4. [Add verified finding 4]
5. [Add verified finding 5]

Do not publish example or estimated values. Use values verified from your own cleaned dataset and dashboard.

## Dashboard Screenshot
Save your actual Tableau dashboard screenshot in this repository using this exact filename:

`Online_Retail_Dashboard.png`

Then keep this image in the same folder as this README. GitHub will display it below:

![Online Retail Dashboard](Online_Retail_Dashboard.png)

If you use a different filename, update the image path above to match it exactly.

## Tableau Public Dashboard
Add your published Tableau Public workbook URL here:

[View Interactive Tableau Dashboard](ADD_YOUR_TABLEAU_PUBLIC_URL)

## Project Repository
This GitHub repository contains the project files and documentation.

## Files to Upload
Upload these project files to the repository:
- `README.md` (this file)
- `cleaned_retail_data.csv` or your cleaned dataset ZIP, if you choose to share the data
- `Online_Retail_Dashboard.png` (your actual dashboard screenshot)
- Tableau workbook file (`.twb` or `.twbx`), if available
- EDA notebook or Python script used for analysis
- Project report PDF, if available

Before uploading data, check the dataset's license and file size. If the cleaned CSV is too large, upload a compressed ZIP or provide the original dataset source instead.

## Final Publishing Checklist
- [ ] Confirm all KPI calculations.
- [ ] Confirm the date, country and product filters work.
- [ ] Check that return/cancellation logic is documented.
- [ ] Add at least five verified findings.
- [ ] Capture and upload the actual Tableau dashboard screenshot.
- [ ] Publish the workbook on Tableau Public.
- [ ] Replace the Tableau Public URL placeholder above.
- [ ] Check that the README image displays correctly on GitHub.
