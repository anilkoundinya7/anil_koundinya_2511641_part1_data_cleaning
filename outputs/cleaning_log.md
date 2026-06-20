# Cleaning Log

## Missing Values

- Filled missing values in `region` with "Unknown".
- Filled missing values in `ship_mode` with "Unknown".
- Replaced missing `discount` values with 0 in `cleaned_discount`.

## Duplicate Records

- Found 17 duplicate Order IDs.
- Duplicate records were flagged for review.
- No records were deleted.

## Discount Validation

- Found 17 negative discount values.
- Found 0 discounts above 1.
- Converted percentage values (70%, 85%) to decimal format.
- Invalid discounts were flagged.

## Date Validation

- Missing order_date: 0
- Missing ship_date: 0
- Found 97 records where ship_date was earlier than order_date.
- Invalid shipping records were flagged.

## Order & Payment Validation

- Cancelled Orders: 147
- Returned Orders: 165
- Failed Payments: 70
- Refunded Payments: 73

Action:
- Excluded cancelled, failed and refunded transactions from completed sales summaries.

## Sales & Profit Validation

- Sales mismatches found: 96
- Profit mismatches found: 98

Action:
- Mismatches were flagged for business review.

## Final Data Quality Summary

- Total Records: 932
- Clean Records: 823
- Invalid Records: 109
- Warning Records: 0

No rows were deleted. Invalid records were flagged for review.
