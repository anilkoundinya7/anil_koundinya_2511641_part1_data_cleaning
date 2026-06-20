# Part 1: Business Data Cleaning, Validation & Excel Reporting

## Problem Summary

This project focuses on cleaning, validating, and preparing retail order data for business analysis. The raw dataset contained inconsistencies such as missing values, duplicate records, invalid discounts, date issues, and sales/profit calculation mismatches. The objective was to create a clean, analysis-ready dataset and generate summary reports for business review.

## Dataset Description

Dataset Used: Retail order-level sales data provided in the assignment.

Files Included:

* raw_orders.xlsx
* cleaned_orders.xlsx
* data_quality_report.xlsx
* pivot_summary.xlsx
* cleaning_log.md

## Tools Used

* Microsoft Excel
* Pivot Tables
* Excel Functions (TRIM, IF, YEAR, TEXT, etc.)

## Cleaning Steps Performed

* Standardized text fields.
* Cleaned and validated order dates and ship dates.
* Identified duplicate order IDs.
* Filled missing values.
* Validated discount values.
* Calculated shipping delays.
* Calculated sales and profit metrics.
* Created data quality flags.
* Extracted order month and order year.

## Business Rules Applied

* Missing region values were filled with "Unknown".
* Missing ship_mode values were filled with "Unknown".
* Missing discounts were treated as 0 when applicable.
* Negative discounts were flagged as invalid.
* Discounts above the allowed range were flagged.
* Orders with ship_date earlier than order_date were flagged.
* Cancelled and failed payment orders were excluded from completed sales summaries.
* Refunded orders were separately summarized.

## Data Quality Issues Found

* Duplicate Order IDs Found: 64
* Negative Discounts Found: 17
* Invalid Shipping Records: 97
* Sales Mismatches: 96
* Profit Mismatches: 98

## Pivot Reports Created

1. Sales and Profit by Region
2. Sales and Profit by Category and Sub-Category
3. Order Count by Ship Mode
4. Profit Margin by Customer Segment
5. Refunded/Cancelled/Failed Orders by Region
6. Monthly Sales Trend

## Key Business Insights

* South region generated the highest sales.
* Standard Class was the most frequently used shipping mode.
* Several records contained invalid shipping dates.
* Duplicate order IDs required manual review.
* Sales and profit mismatches were identified and flagged.

## Assumptions

* Missing region and ship_mode values were replaced with "Unknown".
* Percentage discounts (70%, 85%) were converted to decimal values.
* Duplicate records were flagged instead of deleted.

## Limitations

* Conflicting duplicate records were not removed automatically.
* Invalid records were flagged for review rather than deleted.

## Screenshots Included

* raw_data_preview.png
* cleaned_data_preview.png
* pivot_summary_1.png
* pivot_summary_2.png


