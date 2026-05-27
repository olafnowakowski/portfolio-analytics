# Spreadsheet Functions for Data Cleaning

## Main Idea

Spreadsheet functions can make data cleaning faster, more accurate, and more efficient.

Functions help analysts check for errors, count values, measure text length, extract parts of text strings, combine text strings, and remove extra spaces.

Common data-cleaning functions include:

- `COUNTIF`
- `LEN`
- `LEFT`
- `RIGHT`
- `MID`
- `CONCATENATE`
- `TRIM`

---

# 1. What Is a Function?

A **function** is a set of instructions that performs a specific calculation using data in a spreadsheet.

Functions are useful because they automate tasks that would take much longer to do manually.

---

# 2. Syntax

**Syntax** is the required structure of a function.

It includes:

- the function name
- parentheses
- required inputs
- commas
- ranges or values

If the syntax is wrong, the function may not work correctly.

---

# 3. COUNTIF

## Definition

`COUNTIF` is a function that returns the number of cells that match a specified value or condition.

It counts how many times a value appears in a range of cells.

---

## COUNTIF Syntax

```excel
=COUNTIF(range,"condition")
```

---

## Example: Count Membership Dues Less Than $100

The lowest valid membership due is `$100`.

To check if any dues are less than `$100`, use:

```excel
=COUNTIF(I2:I72,"<100")
```

This checks cells `I2` through `I72` and counts how many values are less than `100`.

---

## Example: Count Membership Dues Greater Than $500

The highest valid membership due is `$500`.

To check if any dues are greater than `$500`, use:

```excel
=COUNTIF(I2:I72,">500")
```

This helps identify values that are unusually high, such as an extra zero entered by mistake.

---

## Why COUNTIF Is Useful

`COUNTIF` can help find:

- negative numbers
- values below the expected range
- values above the expected range
- repeated values
- values that match a specific condition

---

# 4. LEN

## Definition

`LEN` is a function that returns the length of a text string by counting the number of characters it contains.

Characters can include:

- letters
- numbers
- spaces
- punctuation

---

## LEN Syntax

```excel
=LEN(cell)
```

---

## Example: Check Member ID Length

If member IDs should be six digits long, use `LEN` to check whether each ID contains six characters.

```excel
=LEN(A2)
```

This counts the number of characters in cell `A2`.

---

## How to Use LEN for Data Cleaning

If every member ID should have six characters, any result that is not `6` may indicate an error.

You can combine `LEN` with conditional formatting to highlight values that are not equal to `6`.

---

# 5. Conditional Formatting With LEN

Conditional formatting can highlight cells when values meet or fail a condition.

## Example

If column B contains the length of each member ID, you can highlight cells where the value is not equal to `6`.

This helps identify IDs with too many or too few characters.

---

# 6. LEFT

## Definition

`LEFT` is a function that returns a set number of characters from the left side of a text string.

---

## LEFT Syntax

```excel
=LEFT(cell,number_of_characters)
```

---

## Example: Extract Numeric Product Code

Suppose a product code contains:

- a five-digit numeric code
- a four-character text identifier

To extract the first five characters from cell `A2`, use:

```excel
=LEFT(A2,5)
```

This returns only the five-digit numeric part of the product code.

---

# 7. RIGHT

## Definition

`RIGHT` is a function that returns a set number of characters from the right side of a text string.

---

## RIGHT Syntax

```excel
=RIGHT(cell,number_of_characters)
```

---

## Example: Extract Text Identifier

If a product code ends with a four-character text identifier, use:

```excel
=RIGHT(A2,4)
```

This returns only the four-character identifier from the right side of the product code.

---

# 8. Text String

## Definition

A **text string** is a group of characters inside a cell.

A text string can include:

- letters
- numbers
- symbols
- spaces

## Example

```text
12345ABCD
```

---

# 9. Substring

## Definition

A **substring** is a smaller part of a text string.

## Example

Full text string:

```text
12345ABCD
```

Substring from the left:

```text
12345
```

Substring from the right:

```text
ABCD
```

Functions like `LEFT`, `RIGHT`, and `MID` can extract substrings.

---

# 10. MID

## Definition

`MID` is a function that returns a segment from the middle of a text string.

---

## MID Syntax

```excel
=MID(cell,start_position,number_of_characters)
```

---

## Example: Extract State Abbreviation

Suppose a client code includes:

- first three letters of the city
- two-letter state abbreviation
- three-digit identifier

If the code is in cell `D2`, and the state abbreviation starts at the fourth character, use:

```excel
=MID(D2,4,2)
```

This starts at character `4` and extracts `2` characters.

---

## Why MID Is Useful

`MID` is useful when the needed information is located inside a text string, not at the beginning or end.

It can help extract:

- state abbreviations
- area codes
- product segments
- location codes
- middle parts of IDs

---

# 11. CONCATENATE

## Definition

`CONCATENATE` is a function that joins two or more text strings into one text string.

It does the opposite of splitting text apart.

---

## CONCATENATE Syntax

```excel
=CONCATENATE(text1,text2)
```

---

## Example: Rejoin Product Code Parts

If the numeric part of a product code is in `H2` and the text identifier is in `I2`, use:

```excel
=CONCATENATE(H2,I2)
```

This joins the two parts back into one complete product code.

---

## Example With a Space

If first name is in `A2` and last name is in `B2`, use:

```excel
=CONCATENATE(A2," ",B2)
```

This joins the first name, a space, and the last name.

---

# 12. TRIM

## Definition

`TRIM` is a function that removes leading, trailing, and repeated spaces in data.

---

## TRIM Syntax

```excel
=TRIM(cell)
```

---

## Example: Remove Extra Spaces From Client Names

If client names are in cell `C2`, use:

```excel
=TRIM(C2)
```

This removes extra spaces from the client name.

---

## Why TRIM Is Useful

Extra spaces can cause problems when:

- searching
- filtering
- sorting
- matching values
- using lookup functions

For example, a client name may not appear in search results if it contains hidden extra spaces.

---

# 13. Function Summary Table

| Function | Purpose | Example |
|---|---|---|
| `COUNTIF` | Counts cells that match a condition | `=COUNTIF(I2:I72,"<100")` |
| `LEN` | Counts characters in a text string | `=LEN(A2)` |
| `LEFT` | Extracts characters from the left | `=LEFT(A2,5)` |
| `RIGHT` | Extracts characters from the right | `=RIGHT(A2,4)` |
| `MID` | Extracts characters from the middle | `=MID(D2,4,2)` |
| `CONCATENATE` | Joins text strings together | `=CONCATENATE(H2,I2)` |
| `TRIM` | Removes extra spaces | `=TRIM(C2)` |

---

# 14. Split vs CONCATENATE

| Tool or Function | Purpose |
|---|---|
| Split text to columns | Separates one text string into multiple columns |
| `CONCATENATE` | Joins multiple text strings into one cell |

---

# 15. LEFT, RIGHT, and MID Comparison

| Function | Extracts From | Best Used When |
|---|---|---|
| `LEFT` | Beginning of a text string | Needed data is at the start |
| `RIGHT` | End of a text string | Needed data is at the end |
| `MID` | Middle of a text string | Needed data is inside the string |

---

# 16. Common Mistakes to Avoid

## Mistake 1: Using the wrong range

Always check that the function refers to the correct cell or range.

## Mistake 2: Forgetting quotation marks in COUNTIF conditions

Conditions like `<100` or `>500` should be placed inside quotation marks.

## Mistake 3: Miscounting characters

When using `LEFT`, `RIGHT`, or `MID`, count the characters carefully.

## Mistake 4: Ignoring spaces

Spaces count as characters in text strings and can affect function results.

## Mistake 5: Forgetting to drag formulas down

After writing a function for one row, apply it to the rest of the column if needed.

## Mistake 6: Using CONCATENATE without separators

If you want a space between values, include it in quotation marks.

Example:

```excel
=CONCATENATE(A2," ",B2)
```

---

# 17. Key Takeaways

- Functions help automate data cleaning tasks.
- `COUNTIF` counts cells that match a condition.
- `LEN` checks the length of text strings.
- Conditional formatting can highlight values that do not meet expected rules.
- `LEFT` extracts characters from the start of a text string.
- `RIGHT` extracts characters from the end of a text string.
- `MID` extracts characters from the middle of a text string.
- `CONCATENATE` joins multiple text strings into one.
- `TRIM` removes extra spaces from data.
- These functions help improve data integrity and make datasets easier to analyze.

---

# Final Summary

Spreadsheet functions can make data cleaning faster and more reliable. `COUNTIF` helps count cells that match a condition, such as membership dues below or above expected values. `LEN` checks the number of characters in a text string, which is useful for validating ID lengths. `LEFT`, `RIGHT`, and `MID` extract specific parts of text strings, such as product codes or state abbreviations. `CONCATENATE` joins separate text strings into one complete value, while `TRIM` removes extra spaces that can interfere with searching, sorting, and matching. The main lesson is that spreadsheet functions help analysts clean data efficiently and support stronger data integrity.
