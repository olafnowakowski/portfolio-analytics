# Spreadsheet Tools for Data Cleaning

## Main Idea

Data Analysts use spreadsheet tools to clean data faster and more accurately.

Common tools include:

- conditional formatting
- remove duplicates
- date formatting
- text strings and substrings
- split text to columns
- CONCATENATE

These tools help identify missing data, remove repeated records, standardize formats, separate combined data, and prepare datasets for analysis.

---

# 1. Why Spreadsheet Cleaning Tools Matter

Data can be cleaned manually, but spreadsheet tools make the process faster and more efficient.

Spreadsheet tools help analysts:

- find missing values
- highlight errors
- remove duplicates
- fix inconsistent formats
- separate text into different columns
- convert values into usable formats
- reduce manual work
- avoid cleaning mistakes

---

# 2. Conditional Formatting

## Definition

**Conditional formatting** is a spreadsheet tool that changes how cells appear when values meet specific conditions.

It can also help show when cells do not meet the conditions set by the analyst.

---

## Why Conditional Formatting Is Useful

Conditional formatting gives visual cues.

This is especially useful when working with large spreadsheets because it makes certain values stand out.

Analysts can use it to identify:

- blank cells
- missing data
- unusual values
- duplicate values
- values above or below a threshold
- data that does not follow expected rules

---

## Example: Highlighting Blank Cells

In the logistics association spreadsheet, conditional formatting is used to highlight blank cells.

This helps the analyst quickly see where information is missing.

## Basic Steps

1. Select the range you want to check.
2. Go to **Format**.
3. Choose **Conditional formatting**.
4. Set the rule to format cells if the cell is empty.
5. Choose a formatting style, such as a bright fill color.
6. Click **Done**.

The blank cells are then highlighted automatically.

---

# 3. Remove Duplicates

## Definition

**Remove duplicates** is a spreadsheet tool that automatically searches for and removes duplicate entries from a spreadsheet.

---

## Important Rule Before Removing Data

Before removing anything from a dataset, always make a copy of the original data.

This gives you a backup in case you accidentally remove something important.

---

## Why Duplicates Are a Problem

Duplicate records can lead to:

- inflated counts
- incorrect totals
- inaccurate summaries
- misleading analysis
- poor business decisions

---

## Basic Steps to Remove Duplicates

1. Make a copy of the dataset.
2. Go to **Data**.
3. Select **Remove duplicates**.
4. Choose **Data has header row** if the first row contains column names.
5. Select the columns or choose **All** to inspect the full spreadsheet.
6. Click **Remove duplicates**.

The spreadsheet finds and removes duplicate rows.

---

# 4. Standardizing Date Formats

Dates should be formatted consistently before analysis.

Inconsistent date formats can cause confusion when analyzing time-based information.

---

## Why Date Formatting Matters

Consistent date formatting is important when analyzing:

- when members joined
- when memberships were renewed
- how long someone has been a member
- trends over time
- expiration dates
- time between events

---

## Basic Steps to Format Dates

1. Select the date column.
2. Go to **Format**.
3. Select **Number**.
4. Choose **Date**.

This makes all dates in the selected column follow the same format.

---

# 5. Text String

## Definition

A **text string** is a group of characters inside a cell.

Text strings are usually made of letters, numbers, punctuation, or spaces.

---

## Example

```text
Maria Smith
```

or:

```text
Toronto, Ontario, Canada
```

---

## Text String Length

The **length** of a text string is the number of characters in it.

This can include:

- letters
- numbers
- spaces
- punctuation

---

# 6. Substring

## Definition

A **substring** is a smaller part of a text string.

---

## Example

Full text string:

```text
Maria Smith
```

Substring:

```text
Maria
```

Another substring:

```text
Smith
```

---

# 7. Split Text to Columns

## Definition

**Split** is a tool that divides a text string around a specified character and puts each piece into a separate cell.

The specified character used to separate the text is called a **delimiter**.

---

# 8. Delimiter

## Definition

A **delimiter** is the character that separates pieces of text in a cell.

Common delimiters include:

```text
comma
space
semicolon
dash
```

---

## Example

If certifications are listed like this:

```text
CPC, CLTD, CSCP
```

The comma is the delimiter.

After splitting, each certification can be placed into its own column.

---

# 9. When Split Text to Columns Is Useful

Split text to columns is useful when one cell contains more than one piece of information.

Examples:

- first and last name in one cell
- city, state, country, and zip code in one cell
- multiple certifications in one cell
- product codes stored together
- numbers stored as text

---

## Example: Splitting Certifications

A logistics association wants to analyze professional certifications earned by members.

The certifications are stored in one column and separated by commas.

The analyst can use **Split text to columns** to put each certification into a separate column.

---

## Basic Steps

1. Highlight the column.
2. Select **Data**.
3. Choose **Split text to columns**.
4. Confirm or select the delimiter.
5. The spreadsheet separates the text into columns.

Sometimes the spreadsheet detects the delimiter automatically.

Other times, the analyst must choose it manually.

---

# 10. Numbers Stored as Text

Sometimes values look like numbers but are actually stored as text.

This can happen when:

- copying and pasting data
- importing data from another system
- formatting is incorrect
- numbers contain hidden characters

---

## Why This Is a Problem

If a number is stored as text, the spreadsheet may not be able to use it in calculations.

For example, a formula may fail if it tries to multiply a product cost by a units-sold value that is stored as text.

---

## Example

A cosmetics company spreadsheet has an order value that looks like:

```text
707
```

But the spreadsheet treats it as text instead of a number.

Because of this, the calculation fails.

Using **Split text to columns** can sometimes resolve the issue by making the value usable as a number.

---

# 11. CONCATENATE

## Definition

**CONCATENATE** is a spreadsheet function that joins multiple text strings into one text string.

It does the opposite of splitting text.

---

## Example

If first name and last name are in separate cells, CONCATENATE can join them together.

Example logic:

```excel
=CONCATENATE(A2," ",B2)
```

This joins the value in A2, a space, and the value in B2.

---

# 12. Split vs CONCATENATE

| Tool | Purpose |
|---|---|
| Split text to columns | Separates one text string into multiple cells |
| CONCATENATE | Joins multiple text strings into one cell |

---

# 13. Common Spreadsheet Cleaning Tools

| Tool | Main Use |
|---|---|
| Conditional formatting | Highlights cells that meet or fail conditions |
| Remove duplicates | Finds and removes duplicate records |
| Date formatting | Makes date values consistent |
| Split text to columns | Separates combined text into separate columns |
| CONCATENATE | Combines multiple text strings into one |
| Text formatting tools | Fix text strings, substrings, and formatting issues |

---

# 14. Common Mistakes to Avoid

## Mistake 1: Removing duplicates without making a copy

Always back up your dataset before removing data.

## Mistake 2: Ignoring blank cells

Blank cells may indicate missing information that needs to be added or investigated.

## Mistake 3: Leaving dates in inconsistent formats

Inconsistent dates can make time-based analysis confusing or inaccurate.

## Mistake 4: Forgetting to check delimiters

If the wrong delimiter is selected, the text may split incorrectly.

## Mistake 5: Treating numbers stored as text like real numbers

Numbers stored as text may break calculations.

## Mistake 6: Confusing Split and CONCATENATE

Split separates text. CONCATENATE joins text.

---

# 15. Key Takeaways

- Spreadsheet tools make data cleaning faster and more accurate.
- Conditional formatting helps highlight missing or unusual data.
- Remove duplicates helps eliminate repeated records.
- Always make a copy before deleting or removing data.
- Date formatting makes dates consistent for analysis.
- A text string is a group of characters in a cell.
- A substring is a smaller part of a text string.
- Split text to columns separates text using a delimiter.
- A delimiter is the character that separates text values.
- Split text to columns can also help fix some numbers stored as text.
- CONCATENATE joins multiple text strings into one.
- Clean data helps improve data integrity and analysis quality.

---

# Final Summary

This lesson introduces common spreadsheet tools used for data cleaning. Conditional formatting helps highlight cells that meet certain conditions, such as blank cells. Remove duplicates automatically finds and removes repeated records, but analysts should always make a copy of the dataset first. Date formatting helps make dates consistent, which is important for time-based analysis. Text strings are groups of characters, and substrings are smaller parts of those strings. Split text to columns separates combined text into different cells using a delimiter, such as a comma. It can also help fix numbers stored as text. CONCATENATE does the opposite by joining multiple text strings into one. The main lesson is that spreadsheet cleaning tools save time, reduce errors, and help prepare datasets for reliable analysis.
