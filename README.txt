
# Retail Data Cleaning and Preparation

## Project Overview
This project cleans a public online retail dataset
to prepare it for reliable data analysis.

## Dataset Source
UCI Machine Learning Repository:
https://archive.ics.uci.edu/dataset/352/online+retail

## Tools Used
- Python
- Pandas
- Excel file handling
- GitHub

## Data Quality Checks
- Missing values
- Duplicate records
- Incorrect data types
- Inconsistent text values
- Invalid quantities and prices

## Cleaning Steps
1. Inspected the raw dataset and data types.
2. Measured missing values and duplicate records.
3. Removed exact duplicate rows.
4. Trimmed whitespace in text columns.
5. Converted transaction dates and numeric columns.
6. Removed rows missing essential transaction fields.
7. Created a Revenue column using Quantity * UnitPrice.
8. Validated the output and exported the cleaned CSV.

## Results
- Original row count: [fill after running]
- Final row count: [fill after running]
- Duplicate rows removed: [fill after running]
- Remaining missing values: [document actual results]

## Notes
Negative quantities may represent returns.
Missing customer IDs are retained where possible.
Cleaning decisions depend on the intended analysis.

## Author
Swathi Palanivel
