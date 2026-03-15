# Retail-Analysis-on-Spreadsheet

## Data Cleaning

Raw data contained 633 rows across 12 stores and 52 weeks.
The following issues were identified and resolved:

| Issue | Method | Rows Affected | Action |
|---|---|---|---|
| Duplicate rows | COUNTIFS on unique key | 8 | Removed |
| Missing Traffic values | COUNTBLANK | 14 | Removed |
| Negative transactions/sales | COUNTIF <0 | 9 | Removed |
| Outlier sales value | Business logic filter <$1000 | 1 | Removed |
| Store name inconsistencies | UNIQUE function | 5 variants | TRIM + Find & Replace |
| Region typos | UNIQUE function | 3 variants | Find & Replace |
| Inconsistent date formats | COUNTIF wildcard | 22 rows | Find & Replace |

**Clean dataset: 602 rows**
