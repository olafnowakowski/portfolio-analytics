# Spreadsheet Functions Notes

## Overview

Functions help make spreadsheet work faster and more efficient. They are closely related to formulas, but they are not exactly the same.

---

## Formula vs Function

### Formula
A **formula** is a set of instructions used to perform a calculation in a spreadsheet.

**Example:**  
`=(E2-D2)/D2`

### Function
A **function** is a preset command that automatically performs a specific process using spreadsheet data.

**Example:**  
`=SUM(B2:E2)`

### Main difference
- A **formula** is usually written by combining values, operators, and cell references.
- A **function** is a built-in tool that performs a specific task automatically.

---

## Why Functions Are Useful

Functions help analysts:

- save time
- reduce manual work
- perform calculations quickly
- work more efficiently with large datasets

Many function names describe what they do, which makes them easier to learn and remember.

---

## Example: `SUM`

The `SUM` function adds values together.

### Example
`=SUM(B2:E2)`

### How it works
- `SUM` is the function name
- `B2:E2` is the range of cells being added
- the colon `:` shows that all cells between `B2` and `E2` are included

### Result
This calculates total sales for the row.

---

## Example: `AVERAGE`

The `AVERAGE` function calculates the average of a set of values.

### Example
`=AVERAGE(B2:E2)`

### What it does
It adds the values in the selected range and divides by the number of cells in that range.

---

## Not Every Calculation Has a Function

Some calculations still need to be written as formulas.

### Example
To calculate percent change between June and July:

`=(E2-D2)/D2`

This is a formula, not a separate built-in function.

---

## Example: `MIN`

The `MIN` function finds the smallest value in a range.

### Example
`=MIN(B2:E4)`

### What it does
It returns the lowest sales value in the selected dataset.

### Why it is useful
It helps identify the lowest sales amount, which may be important for stakeholders.

---

## Example: `MAX`

The `MAX` function finds the largest value in a range.

### Example
`=MAX(B2:E4)`

### What it does
It returns the highest sales value in the selected dataset.

### Why it is useful
It helps identify the strongest performance in the data.

---

## Highlighting Important Data

Important values can be emphasized by changing the cell color.

### Example
After finding the minimum or maximum value:

- click the cell with that value
- choose the **Fill color** tool
- apply a color such as yellow

### Why this helps
Highlighting makes important data easier to spot.

---

## Common Function Error

Functions must follow the correct format.

### Example mistake
Forgetting the opening parenthesis after a function name:

`=MAX B2:E4`

### Correct version
`=MAX(B2:E4)`

### Key lesson
Always check the syntax of formulas and functions carefully.

---

## Key Functions Mentioned

| Function | Purpose | Example |
|---|---|---|
| `SUM` | Adds values together | `=SUM(B2:E2)` |
| `AVERAGE` | Finds the average value | `=AVERAGE(B2:E2)` |
| `MIN` | Finds the smallest value | `=MIN(B2:E4)` |
| `MAX` | Finds the largest value | `=MAX(B2:E4)` |

---

## Key Takeaways

- A **function** is a preset spreadsheet command
- A **formula** is a custom calculation written with operators and references
- Functions save time and improve efficiency
- Common functions include `SUM`, `AVERAGE`, `MIN`, and `MAX`
- Cell ranges use a colon, such as `B2:E2`
- The fill handle helps copy functions quickly
- Some calculations, like percent change, still require regular formulas
- Correct syntax is important to avoid errors

---

## Short Summary

Functions are built-in spreadsheet tools that automate common calculations like totals, averages, minimums, and maximums. They work similarly to formulas but are preset commands, which makes them faster and easier to use. Combined with tools like ranges and fill handles, functions help data analysts work more efficiently and organize insights more clearly.
