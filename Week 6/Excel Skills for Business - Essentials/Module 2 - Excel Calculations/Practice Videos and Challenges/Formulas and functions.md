# Excel Week 2 Detailed Notes: Performing Calculations

## Main Idea

Week 2 focuses on learning how Excel performs calculations.

The key skills are:

- using formulas
- using functions
- understanding relative cell references
- understanding absolute cell references
- copying calculations with the fill handle
- performing calculations across worksheets

The most important habit is to use cell references instead of typing fixed values directly into formulas.

This allows Excel to update answers automatically when the original data changes.

---

# 1. Basic Formulas in Excel

A formula is a calculation you create in Excel.

Every formula starts with an equals sign:

```excel
=
```

This tells Excel that you want it to calculate something.

---

## Basic Formula Steps

1. Click the cell where you want the answer.
2. Type `=`.
3. Click or type the first cell reference.
4. Add an operator.
5. Click or type the second cell reference.
6. Press Enter.

Example:

```excel
=B3+B4
```

This means: add the value in B3 to the value in B4.

---

# 2. Why Cell References Matter

You could type a formula like this:

```excel
=20+10
```

This gives the correct answer, but it is not the best method.

A better formula is:

```excel
=B3+B4
```

This is better because if the value in B3 or B4 changes, Excel automatically updates the answer.

This is one of the main strengths of Excel.

---

# 3. Basic Formula Operators

Excel uses different symbols for different calculations.

| Operation | Excel Symbol | Example |
|---|---|---|
| Addition | `+` | `=B3+B4` |
| Subtraction | `-` | `=B3-B4` |
| Multiplication | `*` | `=B3*B4` |
| Division | `/` | `=B3/B4` |

---

## Important Notes

For multiplication, Excel uses an asterisk:

```excel
*
```

For division, Excel uses a forward slash:

```excel
/
```

---

# 4. Formulas in a Business Context

Formulas are useful because they can solve real workplace problems.

In the shipping data example, the spreadsheet had more than 1,000 records.

Instead of typing calculations manually for every row, formulas and the fill handle were used to complete the calculations quickly.

---

# 5. Profit Margin Formula

Profit margin is calculated by subtracting cost price from retail price.

Formula logic:

```excel
=Retail Price - Cost Price
```

Example structure:

```excel
=N4-M4
```

This calculates how much profit is made before considering other costs.

---

# 6. Subtotal Formula

Subtotal is the amount the customer pays before discount and shipping.

Formula logic:

```excel
=Retail Price * Order Quantity
```

Example structure:

```excel
=N4*R4
```

This multiplies the retail price by the number of items ordered.

---

# 7. Discount Formula

A discount is calculated as a percentage of the subtotal.

Formula logic:

```excel
=Subtotal * Discount %
```

Example structure:

```excel
=S4*T4
```

If the discount is 6%, Excel treats it as:

```excel
0.06
```

So 6% is not the same as 6.

It means 6 divided by 100.

---

# 8. Order Total Formula

Order total is calculated by taking the subtotal, subtracting the discount, and adding the shipping cost.

Formula logic:

```excel
=Subtotal - Discount + Shipping Cost
```

Example structure:

```excel
=S4-U4+V4
```

This is a slightly longer formula, but it still uses the same basic operators.

---

# 9. Fill Handle

The fill handle is the small square at the bottom-right corner of the selected cell.

It lets you copy formulas down or across a spreadsheet.

---

## Why the Fill Handle Matters

If you have more than 1,000 rows, you do not want to type the same formula again and again.

Instead:

1. Create the formula once.
2. Select the cell with the formula.
3. Use the fill handle.
4. Excel copies the formula to the remaining rows.

---

## Ways to Use the Fill Handle

You can:

- drag the fill handle down
- double-click the fill handle to copy the formula down a column

Double-clicking is useful when Excel can detect the data range beside the formula.

---

# 10. Functions

A function is a built-in Excel calculation.

Functions are useful when formulas would be too long or repetitive.

Example of a long formula:

```excel
=B4+C4+D4+E4
```

The same calculation with a function:

```excel
=SUM(B4:E4)
```

Both add the same values, but the function is cleaner and easier to manage.

---

# 11. SUM Function

The SUM function adds values together.

Example:

```excel
=SUM(B4:E4)
```

This means: add all values from B4 through E4.

---

## Parts of the SUM Function

```excel
=SUM(B4:E4)
```

| Part | Meaning |
|---|---|
| `=` | Starts the calculation |
| `SUM` | Tells Excel to add values |
| `(` | Opens the function |
| `B4:E4` | The range of cells to add |
| `)` | Closes the function |

---

# 12. The Colon in a Function

The colon `:` is a range operator.

It means “from this cell through that cell.”

Example:

```excel
B4:E4
```

This means:

```text
B4, C4, D4, and E4
```

---

# 13. AutoSum

AutoSum is a shortcut that inserts the SUM function automatically.

It is usually found on the Home tab of the ribbon.

---

## How AutoSum Works

Excel tries to guess which cells should be added.

Its basic logic is:

1. Look above the selected cell.
2. If there are at least two numbers above, add them.
3. If not, look to the left.
4. If there are numbers to the left, add them.
5. If Excel chooses the wrong range, manually select the correct cells.

---

## Important AutoSum Note

AutoSum is fast, but you should always check the selected range before pressing Enter.

Excel is helpful, but it does not always choose the correct cells.

---

# 14. AVERAGE Function

The AVERAGE function calculates the average of a range.

Example:

```excel
=AVERAGE(B4:E4)
```

This returns the average value across the selected cells.

---

## Ways to Insert AVERAGE

You can insert AVERAGE by:

- typing it manually
- using Insert Function
- using the AutoSum dropdown

The Insert Function button is the small `fx` button near the formula bar.

It opens a dialog box where you can search for a function.

---

# 15. MAX Function

The MAX function returns the largest value in a range.

Example:

```excel
=MAX(B4:E4)
```

This is useful when you want to find the highest value.

Examples:

- highest quarter
- highest sale
- highest score
- highest price
- highest total

---

# 16. MIN Function

The MIN function returns the smallest value in a range.

Example:

```excel
=MIN(B4:E4)
```

This is useful when you want to find the lowest value.

Examples:

- lowest quarter
- lowest sale
- lowest score
- lowest price
- lowest total

---

# 17. Key Functions Summary

| Function | Purpose | Example |
|---|---|---|
| `SUM` | Adds values | `=SUM(B4:E4)` |
| `AVERAGE` | Finds the average | `=AVERAGE(B4:E4)` |
| `MAX` | Finds the largest value | `=MAX(B4:E4)` |
| `MIN` | Finds the smallest value | `=MIN(B4:E4)` |

These are some of the most important beginner Excel functions.

---

# 18. Copying Functions With the Fill Handle

Functions can be copied using the fill handle, just like formulas.

Example:

```excel
=AVERAGE(B4:E4)
```

If this calculates the average for one sales manager, you can use the fill handle to copy it down for the other sales managers.

---

## Fill Handle Warning

When you use the fill handle, Excel copies both:

- the calculation
- the formatting

If copied formatting causes a problem, use Fill Options and choose:

```text
Fill Without Formatting
```

This keeps the formula but avoids changing the formatting.

---

# 19. Relative Cell References

A relative cell reference changes when a formula is copied.

Example:

```excel
=F4*J1
```

If copied down one row, Excel may change it to:

```excel
=F5*J2
```

This happens because Excel thinks in relative positions.

It understands the formula based on where the referenced cells are located in relation to the formula cell.

---

# 20. Why Relative References Are Useful

Relative references are usually helpful.

They let you create one formula and copy it down through many rows.

Example:

```excel
=B4+C4
```

When copied down, it becomes:

```excel
=B5+C5
=B6+C6
=B7+C7
```

This is useful when each row needs its own calculation.

---

# 21. When Relative References Cause Problems

Relative references can cause problems when one part of the formula should stay fixed.

Example:

A commission calculation multiplies each account manager’s total sales by the same 5% commission rate.

If the commission rate is stored in J1, every formula should use J1.

But if you copy this formula down:

```excel
=F4*J1
```

Excel may change it to:

```excel
=F5*J2
```

That is wrong because the commission rate should stay in J1.

---

# 22. Absolute Cell References

An absolute cell reference locks a cell reference so it does not change when copied.

Example:

```excel
=F4*$J$1
```

The dollar signs lock the column and row.

---

## Reference Types

| Reference | Meaning |
|---|---|
| `J1` | Relative reference |
| `$J$1` | Absolute reference |
| `$J1` | Mixed reference: column locked |
| `J$1` | Mixed reference: row locked |

For now, the most important one is:

```excel
$J$1
```

This locks both the column and the row.

---

# 23. F4 Shortcut for Absolute References

You can add dollar signs quickly by using the F4 key.

---

## Steps

1. Start writing the formula.
2. Click the cell you want to lock.
3. Press F4.
4. Excel adds the dollar signs automatically.

Example before pressing F4:

```excel
=F4*J1
```

Example after pressing F4 on J1:

```excel
=F4*$J$1
```

---

## Important F4 Warning

If you press F4 more than once, Excel cycles through different reference types.

These include absolute and mixed references.

Make sure the reference has both dollar signs if you want the whole cell locked.

Correct:

```excel
$J$1
```

---

# 24. When to Use Absolute References

Use an absolute reference when one cell should stay fixed while formulas are copied.

Common examples:

- commission rate
- tax rate
- discount rate
- exchange rate
- target value
- fixed assumption
- lookup value outside the main data table

---

## Commission Example

If J1 contains a 5% commission rate:

```excel
=F4*$J$1
```

When copied down:

- F4 becomes F5, F6, F7, etc.
- J1 stays fixed

---

# 25. Calculations Across Sheets

Excel formulas can use values from different worksheets.

This is useful when data is separated by:

- year
- department
- product
- region
- category

Example scenario:

A summary sheet needs to pull sales totals from:

- Sales 2015
- Sales 2016

---

# 26. Why Copying and Pasting Values Is Risky

Copying and pasting values from one sheet to another can cause problems.

If the original value changes, the pasted value does not update.

This can make the workbook inaccurate.

Example:

If the 2015 sales total changes, but the summary sheet contains an old pasted value, the summary is wrong.

---

# 27. Linking to Another Worksheet

To pull a value from another worksheet:

1. Click the cell where you want the answer.
2. Type `=`.
3. Click the worksheet tab that contains the value.
4. Click the cell with the value.
5. Press Enter.

Example:

```excel
='Sales 2015'!F18
```

This means: pull the value from cell F18 on the Sales 2015 worksheet.

---

# 28. Important Rule for Cross-Sheet Formulas

When creating a formula across sheets, do not click back into the summary sheet before pressing Enter.

Press Enter when the formula is complete.

Clicking back into another worksheet during the formula can break the calculation because Excel may think you are selecting another cell as part of the formula.

---

# 29. Combining Values Across Sheets

You can add values from different worksheets.

Example:

```excel
='Sales 2015'!G4+'Sales 2016'!G4
```

This adds the value from cell G4 on the Sales 2015 sheet to the value from cell G4 on the Sales 2016 sheet.

This is useful when building summaries that combine multiple years or categories.

---

# 30. AutoSum Across a Summary Table

AutoSum can also be used in summary sheets.

If several yearly totals are listed in a row, you can select the cells where totals should go and click AutoSum.

This quickly creates summary totals without typing each formula manually.

---

# 31. Simple Formulas vs Functions

Use a simple formula when the calculation is short and direct.

Examples:

```excel
=B3+B4
=N4-M4
=S4-U4+V4
=F4*$J$1
```

Use a function when Excel already has a built-in calculation for the task.

Examples:

```excel
=SUM(B4:E4)
=AVERAGE(B4:E4)
=MAX(B4:E4)
=MIN(B4:E4)
```

---

## Quick Rule

If you are doing a simple one-step calculation, use a formula.

If you are summarizing a range of values, use a function.

---

# 32. Common Mistakes to Avoid

## Mistake 1: Typing fixed numbers directly into formulas

Avoid:

```excel
=20+10
```

Better:

```excel
=B3+B4
```

This lets Excel update automatically when values change.

---

## Mistake 2: Trusting AutoSum without checking the range

AutoSum is helpful, but it can select the wrong cells.

Always check the highlighted range before pressing Enter.

---

## Mistake 3: Forgetting absolute references

If a formula uses one fixed value, lock it.

Use:

```excel
$J$1
```

instead of:

```excel
J1
```

---

## Mistake 4: Copying formulas between sheets incorrectly

Do not copy formulas from one sheet to another unless you understand how the references will behave.

It is safer to build a link formula directly.

---

## Mistake 5: Copying formatting accidentally

The fill handle copies formatting too.

Use Fill Without Formatting if the copied formatting causes problems.

---

# 33. Mini Glossary

| Term | Meaning |
|---|---|
| Formula | A calculation written by the user |
| Function | A built-in Excel calculation |
| Operator | A symbol used in a formula, such as `+`, `-`, `*`, or `/` |
| Cell reference | A cell address used in a formula, such as B4 |
| Range | A group of cells, such as B4:E4 |
| Fill handle | The small square used to copy formulas or values |
| Relative reference | A cell reference that changes when copied |
| Absolute reference | A cell reference that stays fixed when copied |
| Mixed reference | A reference where only the row or column is locked |
| AutoSum | A tool that quickly inserts the SUM function |

---

# 34. Key Formulas and Functions to Remember

Adds two cells:

```excel
=B3+B4
```

Subtracts one cell from another:

```excel
=B3-B4
```

Multiplies two cells:

```excel
=B3*B4
```

Divides one cell by another:

```excel
=B3/B4
```

Adds a range:

```excel
=SUM(B4:E4)
```

Finds the average of a range:

```excel
=AVERAGE(B4:E4)
```

Finds the highest value in a range:

```excel
=MAX(B4:E4)
```

Finds the lowest value in a range:

```excel
=MIN(B4:E4)
```

Multiplies F4 by a fixed value in J1:

```excel
=F4*$J$1
```

Pulls a value from another worksheet:

```excel
='Sales 2015'!F18
```

Adds values from two worksheets:

```excel
='Sales 2015'!G4+'Sales 2016'!G4
```

---

# 35. Big Lesson

Excel calculations are powerful because they can update automatically.

To make this work well:

- use cell references
- copy formulas with the fill handle
- use functions for ranges
- check AutoSum selections
- lock fixed cells with absolute references
- link across sheets instead of copying static values

---

# Final Summary

Week 2 focuses on performing calculations in Excel. Formulas are used for simple calculations such as addition, subtraction, multiplication, and division. Functions are built-in calculations, such as SUM, AVERAGE, MAX, and MIN, that make it easier to summarize ranges of data. The fill handle helps copy formulas and functions quickly across rows, which is especially useful in large datasets. Relative references adjust when copied, while absolute references lock a cell so it stays fixed. This is important when every row needs to use the same value, such as a commission rate. Excel can also calculate across worksheets by linking directly to cells in other sheets, which is safer than copying and pasting values. The main lesson is that Excel works best when calculations are built with references and functions that update automatically.
