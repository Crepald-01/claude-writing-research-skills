---
name: data-cleaning
description: Clean and standardize messy CSV or spreadsheet data by fixing headers, types, duplicates, inconsistent labels, and missing values, and reporting every change made. Use when the user has a tabular file that is inconsistent or hard to analyze.
---

# Data cleaning

## Process
1. **Inspect**: row and column counts, header row position, data types per column, unique values in categorical columns, count of blanks.
2. **Structure**: remove title rows and footers, promote the real header, drop fully empty rows and columns.
3. **Standardize**:
   - Trim whitespace and normalize case in categories ("NY", "ny ", "New York" → one value).
   - Convert dates to ISO format (YYYY-MM-DD). Flag ambiguous dates like 03/04/2026 rather than guessing.
   - Convert numbers stored as text. Strip currency symbols and thousands separators, keep a note of the currency.
4. **Deduplicate**: identify exact duplicates and near-duplicates (same key fields). Show them before removing.
5. **Handle missing values**: leave blanks as blanks unless the user asks to fill them. Never impute silently.
6. **Flag anomalies**: outliers, negative values where unexpected, impossible dates, mismatched totals.

## Output
- Cleaned file (CSV or XLSX, matching the input format unless asked otherwise).
- A change log: column | issue | action | rows affected.
- A list of anomalies the user should check manually.

## Rules
- Keep the original file untouched. Write the cleaned version as a new file.
- Do not delete rows without listing them first, unless the user has approved deletion.
- Report counts before and after every major step.
