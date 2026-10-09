---
name: spreadsheet-formulas
description: Write, explain, and debug Excel and Google Sheets formulas from a plain-language description or a broken formula. Use when the user needs a formula, wants an existing one explained, or gets an error such as #N/A, #REF!, or #VALUE!.
---

# Spreadsheet formulas

## Writing a formula
1. Ask for or infer: the app (Excel or Google Sheets), the column layout, and the exact result wanted. If the layout is unknown, state the assumed layout (e.g. "assuming data in A2:A500").
2. Prefer functions available in both apps when the app is unknown: SUMIFS, COUNTIFS, INDEX/MATCH, IF, IFERROR, TEXT, DATE.
3. Use XLOOKUP only if the user confirms they have it. Otherwise use INDEX/MATCH or VLOOKUP with exact match (FALSE / 0).
4. Give the formula in a code block, then a plain-English explanation of each part, then one example input and expected output.

## Debugging a formula
Work through the error type:
- **#N/A**: lookup value not found. Check for trailing spaces, number vs text mismatch, or missing exact-match argument.
- **#REF!**: a referenced cell or range was deleted.
- **#VALUE!**: wrong data type in an operation (text in arithmetic, a range where a single value is expected).
- **#DIV/0!**: divisor is zero or blank. Wrap with IFERROR or check the denominator.
- **Wrong result without an error**: check absolute vs relative references ($A$1 vs A1), and whether ranges include header rows.

Ask for the formula, the cell it sits in, and a sample of the referenced data if the cause is not clear.

## Rules
- Use whole-column references sparingly; bounded ranges are faster and safer.
- Explain the fix, not just the new formula, so the user can adapt it.
- Do not claim a formula has been tested if it has not been run against the user's data.
