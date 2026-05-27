# Different Data Perspectives

## Main Idea

Data Analysts can look at data in different ways to clean it more efficiently.

Different perspectives can help analysts find duplicates, missing values, outliers, incorrect values, and important patterns.

Useful tools for changing the way you view data include:

- sorting
- filtering
- pivot tables
- VLOOKUP
- plotting data

---

# 1. Why Different Perspectives Matter

No two analytics projects are exactly the same.

Different projects require analysts to focus on different parts of the data.

Looking at data from different perspectives helps analysts:

- clean data faster
- identify errors more easily
- focus on relevant information
- find outliers
- compare records
- locate missing or incorrect values
- prepare better data for analysis

---

# 2. Sorting

## Definition

**Sorting** means arranging data into a meaningful order.

Data can be sorted:

- alphabetically
- numerically
- from smallest to largest
- from largest to smallest
- by date
- by category

---

## Sorting for Data Cleaning

Sorting is useful for cleaning because it can:

- make values easier to find
- bring duplicate entries closer together
- reveal unusual values
- organize messy data
- help compare similar records

---

## Example

If customer names are sorted alphabetically, duplicate names or spelling variations may appear near each other.

This makes them easier to identify and fix.

---

# 3. Filtering

## Definition

**Filtering** means showing only data that meets specific criteria while hiding the rest.

Filtering does not delete the hidden data. It only changes what is visible.

---

## Filtering for Data Cleaning

Filtering helps analysts focus on a specific part of the dataset.

You might filter for:

- values above a certain number
- values below a certain number
- blank cells
- specific categories
- even or odd values
- records from a certain date range
- outliers or suspicious values

---

## Why Filtering Is Useful

Filtering separates the data you need from the rest of the dataset.

This makes data cleaning faster and more focused.

---

# 4. Pivot Tables

## Definition

A **pivot table** is a data summarization tool used in data processing.

Pivot tables can:

- sort data
- reorganize data
- group data
- count data
- total data
- average data

---

## Pivot Tables for Data Cleaning

In data cleaning, pivot tables give analysts a quick, clutter-free view of the data.

They help analysts focus only on the parts of the dataset that matter for the current project.

---

## Example: Most Profitable Products

A cosmetics company wants to focus only on products that earned at least:

```text
$10,000
```

A pivot table can sort total profits in descending order so the most profitable products appear at the top.

This helps the analyst quickly identify which products are relevant to the project.

---

# 5. VLOOKUP

## Definition

**VLOOKUP** stands for **vertical lookup**.

It is a function that searches for a specific value in a column and returns a corresponding piece of information from the same row.

---

## Why VLOOKUP Is Useful

In real analytics work, all the data needed for a project is rarely stored in one place.

Analysts often need to search across:

- multiple sheets
- different tables
- different databases
- separate datasets

VLOOKUP helps connect related information from different places.

---

## VLOOKUP Syntax

```excel
=VLOOKUP(lookup_value, table_array, column_index, FALSE)
```

---

## VLOOKUP Parts

| Part | Meaning |
|---|---|
| `lookup_value` | The value you want to search for |
| `table_array` | The range where the function should search |
| `column_index` | The column number in the range that contains the value to return |
| `FALSE` | Finds an exact match |

---

## Exact Match

Using `FALSE` tells VLOOKUP to search for an exact match.

This is useful when looking up specific values such as:

- product codes
- member IDs
- customer IDs
- order numbers

---

## Example

A pivot table shows that two product codes are the most profitable.

The analyst uses VLOOKUP to find the product names connected to those product codes.

This helps confirm what the product codes actually mean before analysis continues.

---

# 6. Referencing Another Sheet

When using VLOOKUP, analysts may need to reference another sheet.

An exclamation point `!` indicates that the formula is referencing a cell or range from another sheet.

Example structure:

```excel
=VLOOKUP(A2,Sheet2!A:B,2,FALSE)
```

This means the formula is looking for the value from `A2` in `Sheet2`, using columns `A:B`, and returning a value from the second column.

---

# 7. Absolute References

A dollar sign `$` can be used to lock part of a cell reference.

This keeps the reference from changing when the formula is copied.

Examples:

| Reference | Meaning |
|---|---|
| `$A$2` | Locks both column and row |
| `$A2` | Locks the column only |
| `A$2` | Locks the row only |

---

# 8. Plotting Data

## Definition

**Plotting** means putting data into a graph, chart, table, or other visual format.

Plotting helps analysts quickly see what the data looks like.

---

## Plotting for Data Cleaning

Plotting is useful for identifying:

- skewed data
- outliers
- incorrect values
- unusual patterns
- values that look too high or too low

---

## Example: Product Prices

An analyst wants to check whether product prices are correct.

They create a column chart of product prices.

One product price looks extremely low.

After investigating, the analyst finds that the decimal point is in the wrong place.

The price should be:

```text
$7.30
```

not:

```text
$0.73
```

---

## Why This Matters

A small price error can have a big impact on total profits.

Plotting helps catch these errors before analysis begins.

---

# 9. Outliers

## Definition

An **outlier** is a data point that is very different from the rest of the data.

Outliers may be valid, but they can also be signs of dirty data.

---

## Example

If most product prices are between `$5` and `$20`, but one product is listed as `$0.73`, that value may be an outlier.

The analyst should investigate whether it is correct.

---

# 10. Tool Summary Table

| Tool | Main Purpose | How It Helps With Cleaning |
|---|---|---|
| Sorting | Arranges data in order | Helps find duplicates and unusual values |
| Filtering | Shows only data that meets criteria | Helps focus on specific records or errors |
| Pivot tables | Summarizes and reorganizes data | Gives a clean view of important values |
| VLOOKUP | Searches for a value and returns related data | Helps connect information across sheets |
| Plotting | Visualizes data | Helps identify outliers and suspicious values |

---

# 11. Common Mistakes to Avoid

## Mistake 1: Looking at data only one way

Different views can reveal different problems.

## Mistake 2: Ignoring duplicates when sorting

Sorting can bring duplicates closer together, but the analyst still needs to check them.

## Mistake 3: Forgetting filters hide data

Filtering does not delete data. It only hides records that do not meet the criteria.

## Mistake 4: Assuming product codes are obvious

Product codes should be confirmed instead of guessed.

## Mistake 5: Ignoring outliers

Outliers may reveal important errors, such as misplaced decimal points.

## Mistake 6: Using VLOOKUP without exact match when needed

For IDs and product codes, exact matches are usually important.

---

# 12. Key Takeaways

- Looking at data from different perspectives helps analysts clean data more effectively.
- Sorting organizes data and can make duplicates easier to find.
- Filtering shows only data that meets specific criteria.
- Pivot tables summarize and reorganize data for a clearer view.
- VLOOKUP searches for a value and returns related information from another place.
- Plotting data helps analysts identify outliers and suspicious values.
- Visualizing data can reveal errors that are hard to notice in rows and columns.
- Different tools help analysts find different types of dirty data.
- Clean data leads to more reliable insights and better decisions.

---

# Final Summary

Different data perspectives help Data Analysts clean data more efficiently. Sorting arranges data into a meaningful order and can bring duplicates closer together. Filtering shows only the records that meet specific criteria, helping analysts focus on the data they need. Pivot tables summarize and reorganize data, giving a cleaner view of important values. VLOOKUP helps analysts find related information across sheets or datasets, such as matching product codes to product names. Plotting data in charts helps identify outliers and suspicious values, such as a decimal point error in a product price. The main lesson is that viewing data in different ways helps analysts find dirty data faster and prepare more reliable datasets for analysis.
