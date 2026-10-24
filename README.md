
# Retail Data Cleaning and Preparation

## 1. Project Overview

This project focuses on cleaning and preparing a raw retail transaction dataset for data analysis. The goal is to improve data quality by identifying missing values, duplicate records, incorrect data types, and inconsistent values.

**Project Type:** Data Analytics — Data Cleaning  
**Tools:** Python, Pandas, Excel, GitHub

## 2. Dataset Source

The dataset is obtained from the UCI Machine Learning Repository.

**Dataset:** Online Retail

**Source:** https://archive.ics.uci.edu/dataset/352/online+retail

The dataset contains retail transaction information, including invoice numbers, product codes, product descriptions, quantities, invoice dates, unit prices, customer IDs, and countries.

## 3. Project Objectives

- Identify missing values in the dataset.
- Detect and remove duplicate records.
- Correct inappropriate data types.
- Standardize inconsistent text values.
- Review invalid or unusual quantities and prices.
- Prepare the dataset for further analysis and visualization.

## 4. Data Cleaning Process

### Missing Values
Checked missing values in each column and reviewed their impact on analysis. Missing customer IDs were retained where possible rather than automatically deleting those transactions.

### Duplicate Records
Identified and removed exact duplicate rows to reduce unnecessary repeated records.

### Data Type Correction
Converted the invoice date column into a datetime format and ensured quantity and unit price columns were numeric.

### Text Standardization
Removed unnecessary leading and trailing spaces from selected text columns.

### Data Validation
Reviewed unusual quantities and prices. Negative quantities may represent product returns, so they should not be removed without understanding their business meaning.

### Revenue Calculation
Created a revenue column using the following calculation:

Revenue = Quantity × Unit Price

## 5. Tools and Technologies

- **Python:** Used to perform data cleaning and validation.
- **Pandas:** Used for data manipulation and handling missing values and duplicates.
- **GitHub:** Used to store and document the project.

## 6. Project Files

- `compressed_data.csv.gz` — Compressed cleaned dataset for easier upload and sharing.
- `clean_data.py` — Python script used for data cleaning, if included in the repository.
- `README.md` — Project documentation.

## 7. Results and Validation

The cleaning process includes checks for missing values, duplicate records, data types, and unusual values.

- Original row count: To be confirmed.
- Final row count: To be confirmed.
- Duplicate records removed: To be confirmed.
- Remaining missing values: To be confirmed.

The final results should be updated after running the cleaning script and validating the exported dataset.

## 8. Conclusion

This project demonstrates the importance of data cleaning as an essential step in the data analytics workflow. By identifying data-quality issues and applying appropriate cleaning methods, the dataset can be prepared for more reliable analysis, reporting, and visualization.

## 9. Author

**Swathi Palanivel**

Aspiring Data Analyst

