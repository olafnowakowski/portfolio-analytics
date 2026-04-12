# Spreadsheet Formula Errors Notes

## Overview

Spreadsheet errors are common in data analysis, especially when formulas reference missing, incorrect, or inconsistent data. Troubleshooting these errors is an important skill because it helps keep analysis accurate and reliable.

---

## Common Spreadsheet Errors

### 1. `#DIV/0!` Error

The **DIV error** happens when a formula tries to divide by:

- zero
- an empty cell

### Example
A percentage is calculated by dividing **Tasks Completed** by **Required Tasks**.  
If the required tasks cell contains `0` or is blank, the formula returns a `#DIV/0!` error.

### Fix
Use the `IFERROR()` function to replace the error with a clearer result, such as:

`Not applicable`

### Why this helps
It prevents confusing error messages and makes the spreadsheet easier to read.

---

### 2. `#ERROR!` Error

The **ERROR** message in Google Sheets means the formula cannot be interpreted correctly.  
This is also called a **parsing error**.

### Common cause
- missing comma
- missing parenthesis
- incorrect formula structure

### Example
A `SUM()` formula that should total two ranges causes an error because a comma is missing between the ranges.

### Fix
Add the missing delimiter, such as a comma, between the data ranges.

### Key idea
The spreadsheet must be able to clearly understand where one part of the formula ends and the next begins.

---

### 3. `#N/A` Error

The **N/A** error means the spreadsheet cannot find the data your formula is asking for.

### Common cause
This often happens with functions such as `VLOOKUP()`.

### Example
A lookup table contains `almonds`, but the formula searches for `almond`.

### Fix
Correct the lookup value so it matches the source data exactly.

### Key idea
`#N/A` usually means the value does not exist in the lookup table exactly as written.

---

### 4. `#NAME?` Error

The **NAME** error happens when the spreadsheet does not recognize the formula name.

### Common cause
- misspelled function name
- incorrect formula text

### Example
`VLOOKUP` is typed incorrectly with an extra letter.

### Fix
Correct the spelling of the function name.

### Key idea
Even a small typo in a function name can cause this error.

---

### 5. `#NUM!` Error

The **NUM** error means the formula cannot perform the calculation as written because the numbers or values do not make sense for that formula.

### Example
`DATEDIF()` is used to calculate the number of months between a start date and an end date, but the end date comes before the start date.

### Fix
- verify the data
- make sure the dates are in the correct order
- adjust the formula if needed

### Key idea
This error usually means the formula is valid, but the data given to it is not suitable for that calculation.

---

### 6. `#VALUE!` Error

The **VALUE** error indicates a problem with the formula or the type of data in the referenced cells.

### Common cause
- text appears where a number or date is expected
- incompatible data types are used in a formula

### Example
A person's name is entered into a cell where a date should be used in a `DATEDIF()` calculation.

### Fix
Replace the incorrect text with the correct value, such as a valid date.

### Key idea
This error often takes extra checking because the issue may not be obvious at first.

---

### 7. `#REF!` Error

The **REF** error happens when a formula refers to cells that no longer exist, often because they were deleted.

### Example
A formula adds values from cells `B2`, `B3`, and `B4`, but row 4 is deleted.

### Fix
- update the formula to reference the correct cells
- use a range-based function such as `SUM()` when possible

### Why `SUM()` can help
A formula using a range is often more flexible than one using several direct cell references.

---

## Helpful Functions Mentioned

### `IFERROR()`
Used to return a custom value instead of an error.

### Example use
Show `Not applicable` instead of `#DIV/0!`

---

### `SUM()`
Adds values together.

### Example use
Total tasks across a range of cells

---

### `VLOOKUP()`
Searches for a value in one column and returns related information from another column.

### Example use
Looking up nut prices from a master price list

---

### `DATEDIF()`
Calculates the difference between two dates.

### Example use
Finding the number of months between a project start date and end date

---

## Main Causes of Spreadsheet Errors

Spreadsheet errors often happen because of:

- dividing by zero or blank cells
- missing commas or delimiters
- typos in formulas
- lookup values that do not match exactly
- dates or numbers in the wrong order
- wrong data types, such as text instead of dates
- deleted referenced cells

---

## How to Troubleshoot Spreadsheet Errors

When you see an error:

1. Check the formula syntax carefully
2. Check for missing commas, parentheses, or symbols
3. Verify that referenced cells contain the correct type of data
4. Make sure lookup values match exactly
5. Confirm that referenced cells still exist
6. Use helper functions like `IFERROR()` when appropriate

---

## Key Takeaways

- Spreadsheet errors are normal and fixable
- Each error type points to a different kind of problem
- Common errors include:
  - `#DIV/0!`
  - `#ERROR!`
  - `#N/A`
  - `#NAME?`
  - `#NUM!`
  - `#VALUE!`
  - `#REF!`
- Troubleshooting formulas is an important data analyst skill
- Accurate formulas and clean source data are both necessary for reliable analysis

---

## Quick Summary Table

| Error | Meaning | Common Cause | Fix |
|---|---|---|---|
| `#DIV/0!` | Division by zero or blank cell | denominator is `0` or empty | use `IFERROR()` or correct the value |
| `#ERROR!` | Formula cannot be parsed | missing comma or bad syntax | fix the formula structure |
| `#N/A` | Data not found | lookup value does not match | correct the lookup term |
| `#NAME?` | Formula name not recognized | typo in function name | correct the spelling |
| `#NUM!` | Calculation cannot be performed | invalid number or date order | verify and correct the data |
| `#VALUE!` | Wrong data type in formula | text used where number/date is expected | replace with correct value |
| `#REF!` | Invalid cell reference | referenced cells were deleted | update the formula or use a range |

---

## Short Summary

Spreadsheet formula errors usually happen because of missing values, wrong data types, typos, or broken references. Learning what each error means makes it easier to troubleshoot problems quickly and keep data analysis accurate.
