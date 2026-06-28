
# Business Data Cleaning, Validation & Excel Reporting

## Project Overview

This project was completed as part of the Business Data Cleaning and Validation assignment. The objective was to transform a raw retail sales dataset into a clean, validated and analysis-ready dataset by applying business rules, handling data quality issues and preparing summary reports for management review.

---

## Dataset Information

**Source File:** raw_orders.xlsx

| Description | Value |
|------------|------:|
| Total Records | 932 |
| Total Columns | 21 |
| Final Records After Cleaning | 912 |

---

## Tools Used

- Google Colab
- Python
- Pandas
- NumPy
- OpenPyXL
- Microsoft Excel

---

## Data Cleaning Performed

The following cleaning activities were completed before analysis:

- Standardized all text fields
- Removed leading, trailing and multiple spaces
- Converted mixed date formats into DD/MM/YYYY
- Filled missing Region values with "Unknown"
- Filled missing Ship Mode values with "Unknown"
- Replaced missing Discount values with 0 where applicable
- Identified invalid discount values
- Calculated shipping delay for every order
- Removed exact duplicate records
- Flagged duplicate Order IDs for business review
- Created calculated sales, profit and profit margin columns
- Assigned data quality flags to every record

---

## Business Rules Applied

- Missing Region → Unknown
- Missing Ship Mode → Unknown
- Missing Discount → 0
- Negative Discount → Invalid
- Discount outside the accepted business range → Invalid
- Ship Date earlier than Order Date → Invalid Shipping
- Cancelled orders excluded from completed sales reporting
- Failed payment records excluded from completed sales reporting
- Returned orders analysed separately

---

## Deliverables

The repository contains:

- raw_orders.xlsx
- cleaned_orders.xlsx
- data_quality_report.xlsx
- pivot_summary.xlsx
- cleaning_log.md
- README.md
- Project screenshots

---

## Reports Created

### Data Quality Report

The report includes:

- Missing Value Summary
- Duplicate Summary
- Discount Validation
- Date Validation
- Order Status Summary
- Sales & Profit Validation
- Final Data Quality Summary

### Pivot Reports

- Sales & Profit by Region
- Sales & Profit by Category and Sub-category
- Order Count by Ship Mode
- Profit Margin by Customer Segment
- Cancelled / Returned / Failed Orders by Region
- Monthly Sales Trend

---

## Business Insights

The analysis highlighted several data quality issues that required correction before reporting. Missing Region and Ship Mode values were standardised, duplicate records were reviewed, invalid discounts were identified and shipping inconsistencies were flagged. After validation, the dataset became suitable for business reporting, dashboard development and further analytical work.

---

## Assumptions

- Missing Discount values were treated as zero.
- Missing Region and Ship Mode values were labelled as Unknown.
- Only exact duplicate records were removed.
- Duplicate Order IDs with conflicting information were retained for manual review.

---

## Limitations

The cleaning process was performed only on the supplied dataset and based on the available business rules. Any issues outside the provided data could not be validated.

---

## Repository Structure

part1_data_cleaning/

├── data/

├── outputs/

├── screenshots/

└── README.md

