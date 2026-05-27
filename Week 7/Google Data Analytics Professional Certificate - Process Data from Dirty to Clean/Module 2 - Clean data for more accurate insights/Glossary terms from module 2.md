# Terms and Definitions for Course 4, Module 2

## Main Idea

Course 4, Module 2 focuses on **cleaning data**, identifying **dirty data**, using spreadsheet tools and functions, and preparing datasets so they are accurate, consistent, complete, and ready for analysis.

---

# 1. Clean and Dirty Data

| Term | Definition |
|---|---|
| Clean data | Data that is complete, correct, and relevant to the problem being solved |
| Dirty data | Data that is incomplete, incorrect, or irrelevant to the problem to be solved |
| Duplicate data | Any record that inadvertently shares data with another record |
| Incomplete data | Data that is missing important fields |
| Inconsistent data | Data that uses different formats to represent the same thing |
| Incorrect/inaccurate data | Data that is complete but inaccurate |
| Outdated data | Any data that has been replaced by newer and more accurate information |
| Null | An indication that a value does not exist in a dataset |

---

# 2. Data Cleaning and Validation

| Term | Definition |
|---|---|
| Data validation | A tool for checking the accuracy and quality of data |
| Conditional formatting | A spreadsheet tool that changes how cells appear when values meet specific conditions |
| Remove duplicates | A spreadsheet tool that automatically searches for and eliminates duplicate entries from a spreadsheet |
| Field length | A tool for determining how many characters can be keyed into a spreadsheet field |
| Unique | A value that cannot have a duplicate |

---

# 3. Data Combining and Compatibility

| Term | Definition |
|---|---|
| Compatibility | How well two or more datasets are able to work together |
| Data mapping | The process of matching fields from one data source to another |
| Data merging | The process of combining two or more datasets into a single dataset |
| Merger | An agreement that unites two organizations into a single new one |

---

# 4. Data Professionals

| Term | Definition |
|---|---|
| Data engineer | A professional who transforms data into a useful format for analysis and gives it a reliable infrastructure |
| Data warehousing specialist | A professional who develops processes and procedures to effectively store and organize data |

---

# 5. Text Strings and Text Cleaning

| Term | Definition |
|---|---|
| Text string | A group of characters within a cell, most often composed of letters |
| Substring | A smaller subset of a text string |
| Length | The number of characters in a text string |
| Delimiter | A character that indicates the beginning or end of a data item |

---

# 6. Spreadsheet Functions

| Function | Definition |
|---|---|
| CONCATENATE | A spreadsheet function that joins together two or more text strings |
| LEFT | A function that returns a set number of characters from the left side of a text string |
| LEN | A function that returns the length of a text string by counting the number of characters it contains |
| MID | A function that returns a segment from the middle of a text string |
| Split | A function that divides text around a specified character and puts each fragment into a new, separate cell |
| TRIM | A function that removes leading, trailing, and repeated spaces in data |

---

# 7. Function Examples

## CONCATENATE

Joins text strings together.

```excel
=CONCATENATE(A2," ",B2)
```

Example result:

```text
John Smith
```

---

## LEFT

Returns characters from the left side of a text string.

```excel
=LEFT(A2,5)
```

---

## LEN

Counts the number of characters in a text string.

```excel
=LEN(A2)
```

---

## MID

Returns characters from the middle of a text string.

```excel
=MID(A2,4,2)
```

---

## TRIM

Removes extra spaces from data.

```excel
=TRIM(A2)
```

---

# 8. Quick Study Notes

## Clean Data

Clean data is ready for analysis because it is:

- complete
- correct
- relevant
- consistent
- usable

## Dirty Data

Dirty data needs cleaning because it may contain:

- duplicates
- missing values
- incorrect values
- outdated information
- inconsistent formats
- irrelevant records

## Data Mapping and Merging

Data mapping and merging are important when combining datasets from different sources.

Before merging, check:

- field names
- formats
- data types
- duplicate records
- missing values
- compatibility between datasets

## Spreadsheet Tools

Spreadsheet tools help clean data efficiently.

Useful tools include:

- conditional formatting
- remove duplicates
- data validation
- text functions
- split text to columns
- clear formatting

---

# 9. Key Takeaways

- Clean data is complete, correct, and relevant.
- Dirty data can be incomplete, incorrect, duplicated, outdated, inconsistent, or irrelevant.
- Data validation helps check data quality before analysis.
- Conditional formatting helps highlight values that meet specific conditions.
- Remove duplicates helps eliminate repeated records.
- Compatibility matters when combining datasets.
- Data mapping matches fields from one data source to another.
- Data merging combines datasets into one.
- Text strings can be cleaned and transformed using spreadsheet functions.
- CONCATENATE joins text.
- LEFT, MID, and Split separate text.
- LEN counts characters.
- TRIM removes extra spaces.
- Clean data leads to more reliable analysis and better decisions.

---

# Final Summary

Course 4, Module 2 focuses on identifying and cleaning dirty data. Clean data is complete, correct, and relevant to the problem being solved, while dirty data may be incomplete, incorrect, duplicated, outdated, inconsistent, or irrelevant. Analysts use tools such as data validation, conditional formatting, remove duplicates, and field length rules to improve data quality. They also use functions such as CONCATENATE, LEFT, LEN, MID, Split, and TRIM to clean and transform text. When working with multiple datasets, analysts need to check compatibility, map fields correctly, and merge data carefully. The main lesson is that clean, well-organized data supports accurate analysis and reliable business decisions.
