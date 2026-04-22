# Spreadsheet Formulas Quick Reference

## What Is a Formula?

A **formula** is a set of instructions that performs a specific calculation using data in a spreadsheet.

### Why formulas matter

Formulas help data analysts:

- calculate values automatically
- reduce manual work
- improve accuracy
- analyze data more effectively

---

## Mathematical Operators

The main operators used in spreadsheet formulas are:

- **Addition:** `+`
- **Subtraction:** `-`
- **Multiplication:** `*`
- **Division:** `/`

### Example

`=A1+B1`

---

## Creating a Numbered Sequence

To auto-fill a sequence like `1, 2, 3, 4...`:

1. Enter the first two numbers in adjacent cells.
2. Highlight both cells.
3. Drag the fill handle to continue the sequence.

### Example

To fill numbers `1` through `100` in column A:

- enter `1` in `A1`
- enter `2` in `A2`
- highlight both cells
- drag the fill handle down to `A100`

This fills the numbers automatically in order.

---

## Relative References

A **relative reference** changes when a formula is copied to another cell.

### Example

`=A10`

If copied one cell to the right, it becomes:

`=B10`

### Why this happens

The reference changes based on the new location of the formula.

---

## Absolute References

An **absolute reference** uses dollar signs (`$`) to keep a row, a column, or both fixed.

### Example

`=$A$10`

This locks:

- column `A`
- row `10`

### Key rule

Absolute references do **not** change when copied to another cell.

---

## Mixed References

You can lock only one part of a reference.

### Example

`=$A10`

This locks the column, but not the row.

If copied downward, it becomes:

`=$A11`

Because the row is still relative.

---

## Switching Between Reference Types

You can use the **F4** key to switch between reference styles.

### Example

Highlight `A10` or `$A$10` in the formula bar and press `F4` to cycle through:

- `A10`
- `$A$10`
- `A$10`
- `$A10`

This is a quick way to change reference types without typing dollar signs manually.

---

## Data Range

When you click into a formula, spreadsheet tools often highlight the referenced cells in different colors.

### Why this helps

It makes it easier to see:

- which cells are being used
- which ranges belong to which part of the formula
- how the formula connects to the data

### Extra tip

In many spreadsheet tools, pressing **F2** or **Enter** while the formula cell is selected highlights the referenced range.

---

## Combining Formulas with Functions

A formula can include a **function** to perform more advanced calculations.

### Example: `COUNTIF()`

`=COUNTIF(A1:A16,"7")`

### What it does

This counts only the cells in the range `A1:A16` that contain the number `7`.

### Why this is useful

Combining formulas and functions lets you do more work with one command and apply specific conditions to calculations.

---

## Key Terms

### Formula

A spreadsheet instruction used to calculate a value.

### Function

A built-in spreadsheet command that performs a specific task.

### Operator

A symbol used in a formula, such as `+`, `-`, `*`, or `/`.

### Relative reference

A cell reference that changes when copied.

### Absolute reference

A cell reference that stays fixed when copied.

### Mixed reference

A reference where only the row or only the column is fixed.

### Fill handle

The small square or circle used to copy values, formulas, or sequences.

### Data range

A group of cells used in a formula.

---

## Quick Examples

| Task | Example |
|---|---|
| Add two cells | `=A2+A3` |
| Multiply values | `=B2*C2` |
| Absolute reference | `=$A$10` |
| Mixed reference | `=$A10` |
| Count cells equal to 7 | `=COUNTIF(A1:A16,"7")` |

---

## Key Takeaways

- Formulas always begin with `=`
- Operators are used for addition, subtraction, multiplication, and division
- Autocomplete helps reduce typing and errors
- Auto-fill saves time when copying values, formulas, or sequences
- Relative references change when copied
- Absolute references stay fixed when copied
- Mixed references lock only one part of a reference
- `F4` helps switch between reference types
- Colored ranges help show which cells are used in a formula
- Functions like `COUNTIF()` make formulas more powerful

---

## Short Summary

Spreadsheet formulas are essential for fast and accurate calculations. By using operators, fill handles, relative and absolute references, and functions like `COUNTIF()`, data analysts can automate work, reduce mistakes, and analyze data much more e
