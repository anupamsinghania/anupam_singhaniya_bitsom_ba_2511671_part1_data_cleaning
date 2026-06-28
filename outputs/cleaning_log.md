
# Cleaning Log

## Project Objective

The purpose of this project was to improve the quality of the retail sales dataset before business analysis. The dataset was reviewed for missing values, inconsistent formatting, duplicate records, calculation issues and business rule violations.

---

## Data Quality Issues Identified

The following issues were identified during the assessment:

- Mixed date formats
- Missing Region values
- Missing Ship Mode values
- Missing Discount values
- Invalid Discount values
- Duplicate Order IDs
- Exact duplicate records
- Ship Date earlier than Order Date
- Inconsistent text formatting
- Sales and profit calculation differences

---

## Cleaning Activities Performed

The dataset was cleaned using the following approach:

1. Standardised text formatting across all business fields.
2. Removed leading, trailing and unnecessary spaces.
3. Converted all dates into DD/MM/YYYY format.
4. Filled missing Region values with "Unknown".
5. Filled missing Ship Mode values with "Unknown".
6. Replaced missing Discount values with zero where applicable.
7. Flagged invalid discount values.
8. Calculated Shipping Delay.
9. Removed exact duplicate records.
10. Flagged duplicate Order IDs for manual review.
11. Created calculated Sales, Profit and Profit Margin columns.
12. Assigned a Data Quality Flag to every record.

---

## Business Rules Applied

| Rule | Action Taken |
|------|--------------|
| Missing Region | Filled with Unknown |
| Missing Ship Mode | Filled with Unknown |
| Missing Discount | Replaced with 0 |
| Negative Discount | Flagged as Invalid |
| High Discount | Flagged as Invalid |
| Ship Date before Order Date | Flagged as Invalid Shipping |
| Cancelled Orders | Excluded from completed sales reporting |
| Failed Payments | Excluded from completed sales reporting |
| Returned Orders | Reported separately |

---

## Duplicate Handling

Exact duplicate records were removed from the cleaned dataset.

Duplicate Order IDs with different business information were retained and marked for further investigation instead of being deleted.

---

## Final Outcome

The final dataset is consistent, validated and suitable for reporting, dashboard creation and business analysis. All major quality issues identified during the assessment have been documented in the accompanying reports.

