# Week 2 Toolbox: Excel Calculations

## Main Idea

Week 2 focuses on performing calculations in Excel using formulas, functions, cell references, and worksheet navigation.

The toolbox includes:

- useful keyboard shortcuts
- key Excel terminology
- formula and function concepts
- relative and absolute references
- order of mathematical operations

---

# 1. Keyboard Shortcuts

Keyboard shortcuts help you work faster in Excel.

They are especially useful when writing formulas, moving between sheets, checking calculations, and correcting mistakes.

---

## Common Week 2 Shortcuts

| Shortcut | Windows | Mac | Purpose |
|---|---|---|---|
| Undo previous action | `CTRL + Z` | `CMD + Z` | Reverses the last action |
| Cycle cell reference types | `F4` or `fn + F4` | `CMD + T` | Switches between relative, absolute, and mixed references |
| Show formulas | `CTRL + ~` or `CTRL + \`` | Usually similar depending on keyboard | Displays formulas instead of results |
| Open Function Wizard / Formula Builder | `SHIFT + F3` | `CTRL + A` | Opens help for inserting functions |
| Go to previous sheet | `CTRL + PgUp` | `CMD + PgUp` | Moves to the worksheet on the left |
| Go to next sheet | `CTRL + PgDn` | `CMD + PgDn` | Moves to the worksheet on the right |

---

# 2. CTRL + Z: Undo

## Shortcut

```text
CTRL + Z
```

## Purpose

Undo reverses the previous action.

This is useful when you:

- type the wrong formula
- delete something by mistake
- apply the wrong formatting
- copy a formula incorrectly
- make an accidental change

## Important Note

Undo is one of the most useful shortcuts in Excel because mistakes are easy to make when working quickly.

---

# 3. F4: Cycle Through Cell Reference Types

## Shortcut

```text
F4
```

On some keyboards:

```text
fn + F4
```

On Mac:

```text
CMD + T
```

## Purpose

This shortcut cycles through the four types of cell references:

1. Relative reference
2. Absolute reference
3. Mixed reference with locked row
4. Mixed reference with locked column

---

## Example Cycle

If your formula contains:

```excel
=A1
```

Pressing `F4` cycles through:

```excel
=$A$1
=A$1
=$A1
=A1
```

---

## Reference Type Meaning

| Reference | Type | Meaning |
|---|---|---|
| `A1` | Relative | Column and row can change when copied |
| `$A$1` | Absolute | Column and row are locked |
| `A$1` | Mixed | Row is locked, column can change |
| `$A1` | Mixed | Column is locked, row can change |

---

# 4. CTRL + ~: Show Formulas

## Shortcut

```text
CTRL + ~
```

or:

```text
CTRL + `
```

## Purpose

This shortcut shows formulas in the worksheet instead of the formula results.

---

## Why This Is Useful

Show Formulas helps you:

- check formulas quickly
- find mistakes
- compare formulas across cells
- see whether formulas were copied correctly
- identify fixed references and relative references

---

## Example

Normally, a cell may show:

```text
150
```

But with Show Formulas turned on, it may show:

```excel
=SUM(A1:A5)
```

---

# 5. SHIFT + F3: Function Wizard

## Shortcut

```text
SHIFT + F3
```

On Mac, the equivalent may be:

```text
CTRL + A
```

## Purpose

This opens the Formula Builder or Function Wizard.

---

## Why This Is Useful

The Function Wizard helps you:

- search for functions
- understand function syntax
- enter arguments correctly
- avoid typing mistakes
- learn unfamiliar functions

---

# 6. CTRL + PgUp and CTRL + PgDn: Move Between Sheets

## Previous Sheet

```text
CTRL + PgUp
```

Mac:

```text
CMD + PgUp
```

## Next Sheet

```text
CTRL + PgDn
```

Mac:

```text
CMD + PgDn
```

## Purpose

These shortcuts move between worksheets in the same workbook.

---

## Why This Is Useful

Moving between sheets is useful when:

- formulas reference other worksheets
- data is split across multiple sheets
- you are building a summary sheet
- you need to compare yearly or monthly data

---

# 7. Excel Terminology

This section explains the key Excel terms from Week 2.

---

# 8. Formula

## Definition

A formula is entered into a cell to perform a calculation.

A formula always starts with an equal sign:

```excel
=
```

After you press Enter, Excel displays the result in the cell.

---

## Formula Example

```excel
=A1+B1
```

This formula adds the value in cell A1 to the value in cell B1.

---

## Important Lesson

The formula is stored in the cell, but the result is displayed.

You can see the formula by selecting the cell and looking at the formula bar.

---

# 9. Function

## Definition

A function is a built-in calculation in Excel.

It is like a small program that performs a specific task.

Functions are used inside formulas, so they also start with an equal sign.

---

## Function Example

```excel
=SUM(A1:A12)
```

This function adds all values from A1 through A12.

---

## Important Lesson

Functions are useful for more complex or repetitive calculations.

Instead of writing:

```excel
=A1+A2+A3+A4+A5+A6+A7+A8+A9+A10+A11+A12
```

You can write:

```excel
=SUM(A1:A12)
```

---

# 10. Formula vs Function

| Term | Meaning | Example |
|---|---|---|
| Formula | A calculation written by the user | `=A1+B1` |
| Function | A built-in Excel calculation used inside a formula | `=SUM(A1:A12)` |

---

## Simple Difference

A formula is the full calculation.

A function is a built-in tool that can be part of a formula.

---

# 11. Formula Bar

## Definition

The formula bar is located underneath the ribbon.

It shows the contents of the active cell.

---

## What the Formula Bar Does

The formula bar lets you:

- view formulas
- enter formulas
- edit cell contents
- see what is actually stored in a cell
- use helper tools for formulas and functions

---

# 12. Name Box

## Definition

The Name Box is the first edit line near the formula bar.

It shows the reference of the currently active cell.

---

## Example

If cell B4 is selected, the Name Box shows:

```text
B4
```

---

## Why the Name Box Is Useful

The Name Box helps you know exactly which cell is active.

This is useful when working with large spreadsheets.

---

# 13. Function Options in the Formula Bar

Once you type an equal sign into a cell, Excel may show frequently used functions.

These can appear near the formula bar or Name Box area.

A dropdown menu may offer additional function options.

---

# 14. Value

## Definition

A value is numeric data entered into a cell.

Values can be used in formulas and functions.

---

## Example Values

```text
10
25
350
0.06
1500
```

---

## Important Lesson

If data is formatted as a value type, Excel can use it in calculations.

---

# 15. Label

## Definition

A label is text entered into a cell.

Labels are not usually used directly in mathematical calculations.

---

## Example Labels

```text
Sales
Region
Manager
January
Product Name
```

---

# 16. Value vs Label

| Type | Meaning | Example | Used in calculations? |
|---|---|---|---|
| Value | Numeric data | `250` | Yes |
| Label | Text data | `Sales Total` | Usually no |

---

# 17. Range

## Definition

A range refers to two or more cells.

Ranges are used often in formulas and functions.

---

# 18. Adjacent Range

## Definition

An adjacent range is a group of cells that are next to each other.

---

## Example

```excel
A1:C2
```

This includes all cells from A1 through C2.

That means:

```text
A1, B1, C1, A2, B2, C2
```

---

## Colon Meaning

The colon `:` means “through to.”

So:

```excel
A1:C2
```

means A1 through C2.

---

# 19. Non-Adjacent Range

## Definition

A non-adjacent range includes cells or ranges that are not all next to each other.

---

## Example

```excel
A1:A2,C1:C2
```

This includes:

```text
A1, A2, C1, C2
```

---

## Comma Meaning

The comma separates different ranges.

So:

```excel
A1:A2,C1:C2
```

means include A1 through A2 and C1 through C2.

---

# 20. Relative Cell Reference

## Definition

A relative cell reference changes based on the direction in which it is copied.

---

## Example

```excel
=A2*B2
```

If copied down one row, Excel changes it to:

```excel
=A3*B3
```

If copied down again, Excel changes it to:

```excel
=A4*B4
```

---

## Why Relative References Are Useful

Relative references are useful when each row needs the same type of calculation using that row’s data.

---

## Example Scenario

If column A contains quantity and column B contains price, then column C can calculate total.

In C2:

```excel
=A2*B2
```

Copied down to C3:

```excel
=A3*B3
```

Copied down to C4:

```excel
=A4*B4
```

Excel updates the row numbers automatically.

---

# 21. Absolute Cell Reference

## Definition

An absolute cell reference does not change when copied.

It locks the cell reference.

---

## Example

```excel
=$A$1
```

The dollar signs lock both:

- the column A
- the row 1

---

## Why Absolute References Are Useful

Absolute references are useful when every copied formula needs to refer to the same fixed cell.

---

## Common Uses

Use absolute references for:

- tax rates
- commission rates
- discount rates
- exchange rates
- target values
- assumptions
- fixed input cells

---

# 22. “The Dollar Thingy”

An absolute reference is created by adding dollar signs to a cell reference.

Relative reference:

```excel
A1
```

Absolute reference:

```excel
$A$1
```

---

# 23. Shortcut for Absolute References

Instead of typing dollar signs manually, use:

```text
F4
```

This turns a selected cell reference into an absolute reference.

---

# 24. Mixed References

A mixed reference locks only part of the cell reference.

---

## Mixed Reference Examples

| Reference | Meaning |
|---|---|
| `$A1` | Column A is locked, row can change |
| `A$1` | Row 1 is locked, column can change |

---

## Important Note

Mixed references are useful in more advanced formulas.

For Week 2, the most important reference types are:

- relative references
- absolute references

---

# 25. Order of Basic Mathematical Operations

Excel follows the standard order of operations.

This means multiplication and division happen before addition and subtraction.

---

## Order

1. Parentheses
2. Multiplication and division
3. Addition and subtraction

---

# 26. Example Without Parentheses

```excel
=3+4*5
```

Excel calculates multiplication first.

So Excel reads it as:

```text
3 + (4 * 5)
```

The result is:

```text
23
```

Because:

```text
4 * 5 = 20
3 + 20 = 23
```

---

# 27. Example With Parentheses

```excel
=(3+4)*5
```

Excel calculates what is inside parentheses first.

So Excel reads it as:

```text
(3 + 4) * 5
```

The result is:

```text
35
```

Because:

```text
3 + 4 = 7
7 * 5 = 35
```

---

# 28. Why Parentheses Matter

Parentheses tell Excel which part of the formula to calculate first.

Use parentheses when you need to control the order of calculation.

---

# 29. Formula Comparison

| Formula | Excel Calculates | Result |
|---|---|---|
| `=3+4*5` | `3 + (4*5)` | `23` |
| `=(3+4)*5` | `(3+4) * 5` | `35` |

---

# 30. Week 2 Quick Reference

## Basic Operators

| Operator | Meaning |
|---|---|
| `+` | Add |
| `-` | Subtract |
| `*` | Multiply |
| `/` | Divide |
| `:` | Through to, used in ranges |
| `,` | Separates non-adjacent ranges |
| `$` | Locks part of a cell reference |

---

# 31. Key Examples

## Basic Formula

```excel
=A1+B1
```

Adds A1 and B1.

---

## SUM Function

```excel
=SUM(A1:A12)
```

Adds values from A1 through A12.

---

## Adjacent Range

```excel
A1:C2
```

Includes all cells from A1 through C2.

---

## Non-Adjacent Range

```excel
A1:A2,C1:C2
```

Includes A1 through A2 and C1 through C2.

---

## Relative Reference

```excel
=A2*B2
```

Changes when copied.

---

## Absolute Reference

```excel
=$A$1
```

Does not change when copied.

---

## Order of Operations Example

```excel
=(3+4)*5
```

Uses parentheses to calculate addition first.

---

# 32. Key Takeaways

- Excel formulas always start with `=`.
- A formula performs a calculation.
- A function is a built-in calculation used inside a formula.
- The formula bar shows or edits the contents of the active cell.
- The Name Box shows the active cell reference.
- Values are numeric data that can be used in calculations.
- Labels are text entries.
- A range is two or more cells.
- Adjacent ranges are connected cells.
- Non-adjacent ranges are separated by commas.
- Relative references change when copied.
- Absolute references stay fixed when copied.
- Use `F4` to quickly create absolute references.
- Excel follows order of operations.
- Multiplication and division happen before addition and subtraction.
- Parentheses control the order of calculations.

---

# Final Summary

The Week 2 toolbox introduces the essential shortcuts, terminology, and calculation rules needed for working with formulas and functions in Excel. Formulas are calculations that begin with an equal sign, while functions are built-in tools such as `SUM` that perform common calculations. The formula bar helps users view and edit formulas, and the Name Box shows the active cell reference. Values are numeric data used in calculations, while labels are text. Ranges can be adjacent, such as `A1:C2`, or non-adjacent, such as `A1:A2,C1:C2`. Relative references change when copied, while absolute references, such as `$A$1`, stay fixed. The `F4` shortcut helps cycle through reference types. Excel also follows the standard order of operations, so multiplication and division happen before addition and subtraction unless parentheses are used.
