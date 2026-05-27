# Develop Your Approach to Cleaning Data

## Main Idea

Data is often messy, especially raw or primary data.

Because of this, Data Analysts need a clear and organized approach to data cleaning.

A strong cleaning approach helps save time, reduce errors, and make sure the dataset is clean, reliable, and usable for analysis.

---

# 1. Why a Cleaning Approach Matters

Data cleaning can take a lot of:

- time
- energy
- attention
- careful checking
- decision-making

Creating a personal approach before cleaning helps make the process more efficient and consistent.

---

# 2. Two Steps Before Cleaning Data

Before beginning the cleaning process, analysts can make their work easier by doing two things:

1. Create a cleaning checklist.
2. Decide on preferred cleaning methods.

These steps help analysts know what to look for and how they want to handle common data problems.

---

# 3. Cleaning Checklist

A **cleaning checklist** is a default list of things to check when reviewing a dataset.

It helps analysts identify:

- common data problems
- the scale of the dataset
- the scope of the cleaning work
- possible data integrity issues
- what cleaning techniques may be needed

---

# 4. Why Use a Cleaning Checklist?

A checklist helps analysts clean data more methodically.

It can help prevent missed errors and make the cleaning process more repeatable.

A checklist also helps analysts stay organized when working with large or messy datasets.

---

# 5. Checklist Item: Determine the Size of the Dataset

Before cleaning, check how large the dataset is.

Large datasets may:

- contain more errors
- take longer to clean
- require different cleaning tools
- need more processing time
- affect project deadlines

## Key Lesson

Dataset size can influence which cleaning techniques you use and how much time you should plan for cleaning.

---

# 6. Checklist Item: Determine the Number of Categories or Labels

Categories and labels help describe groups in the dataset.

Examples may include:

- customer type
- membership level
- product category
- location
- department
- survey response group

Understanding categories and labels helps analysts understand the diversity and structure of the dataset.

---

## Why Categories and Labels Matter

Knowing the categories and labels can help with:

- data merging
- data migration
- grouping data
- filtering data
- checking inconsistent labels
- identifying duplicate or overlapping categories

---

# 7. Checklist Item: Identify Missing Data

Missing data can affect the quality and reliability of analysis.

Missing data may appear as:

- blank cells
- null values
- incomplete records
- missing columns
- missing time periods

## Key Lesson

Identifying missing data helps analysts decide how to fix or handle the issue before analysis.

---

# 8. Why Missing Data Matters

Missing data can lead to:

- incomplete analysis
- inaccurate conclusions
- biased results
- incorrect calculations
- poor business decisions

Data integrity depends on having complete and reliable data.

---

# 9. Checklist Item: Identify Unformatted Data

Unformatted or inconsistently formatted data can make analysis harder.

Examples include:

- dates in different formats
- currency values formatted differently
- inconsistent capitalization
- numbers stored as text
- extra spaces
- inconsistent labels

## Key Lesson

Formatting should be consistent so the data can be analyzed and visualized correctly.

---

# 10. Checklist Item: Explore Different Data Types

Before cleaning, understand what types of data are in the dataset.

Common data types include:

- numerical data
- categorical data
- text data
- date data
- Boolean data

---

## Why Data Types Matter

Different data types require different cleaning methods.

For example:

| Data Type | Possible Cleaning Need |
|---|---|
| Numerical data | Check ranges, outliers, missing values |
| Categorical data | Standardize labels and categories |
| Text data | Remove extra spaces, fix spelling, clean capitalization |
| Date data | Standardize date formats |
| Boolean data | Check true/false consistency |

---

# 11. Making the Checklist Personal

A cleaning checklist should match the analyst’s needs and the type of work they do.

Analysts can add items based on what they commonly encounter.

Possible extra checklist items:

- check for duplicates
- check for outliers
- check for incorrect values
- check for misfielded values
- check data source reliability
- check whether data aligns with the business objective
- check whether the data is current
- check whether formulas work correctly

---

# 12. Preferred Cleaning Methods

Preferred cleaning methods are the tools, functions, or actions an analyst likes to use when cleaning data.

These methods should match the cleaning checklist.

---

# 13. Why Preferred Methods Matter

Having preferred methods saves time because the analyst already knows how they will approach common issues.

For example, if missing data is common, the analyst should know how they prefer to:

- find missing values
- highlight missing values
- remove missing values
- replace missing values
- explain missing values in the final report

---

# 14. Example: Large Dataset With Missing Data

Suppose an analyst has a large dataset with missing data.

Before cleaning, the analyst should decide:

- how to check for missing data
- which tool to use
- whether missing values should be removed
- whether missing values should be filled in
- whether missing values should be kept and explained
- whether stakeholders should be informed

Having a plan prevents confusion during cleaning.

---

# 15. Examples of Preferred Cleaning Tools

Preferred tools may include:

- filters
- sorting
- conditional formatting
- remove duplicates
- spellcheck
- find and replace
- pivot tables
- data validation
- spreadsheet functions
- SQL queries
- scripts

---

# 16. Examples of Useful Spreadsheet Functions

Common functions for cleaning include:

```excel
=TRIM(A2)
```

```excel
=LEN(A2)
```

```excel
=COUNTIF(A:A,"")
```

```excel
=LEFT(A2,5)
```

```excel
=RIGHT(A2,4)
```

```excel
=MID(A2,4,2)
```

```excel
=CONCATENATE(A2," ",B2)
```

These functions can help remove spaces, check text length, count values, extract parts of text, and combine text strings.

---

# 17. Cleaning Checklist Example

| Checklist Item | What to Check |
|---|---|
| Dataset size | How many rows and columns are there? |
| Categories and labels | Are labels consistent and meaningful? |
| Missing data | Are there blanks, nulls, or incomplete records? |
| Formatting | Are dates, numbers, currency, and text consistent? |
| Data types | Are values stored as the correct type? |
| Duplicates | Are any records repeated? |
| Outliers | Are any values unusually high or low? |
| Business objective | Does the data support the analysis question? |

---

# 18. Preferred Methods Example

| Problem | Preferred Method |
|---|---|
| Missing data | Use filters or conditional formatting to find blanks |
| Extra spaces | Use `TRIM` |
| Duplicate records | Use Remove duplicates after making a backup |
| Inconsistent labels | Use Find and Replace or standardize categories |
| Incorrect dates | Apply consistent date formatting |
| Numbers stored as text | Convert format or use spreadsheet tools |
| Outliers | Use sorting, filters, or charts |
| Wrong field values | Compare columns and check source systems |

---

# 19. Planning Helps Data Cleaning

Planning before cleaning helps analysts:

- work faster
- avoid repeated mistakes
- use the right tools
- stay focused
- protect data integrity
- meet deadlines
- produce cleaner results

Good planning sets the project up for success.

---

# 20. Important Reminder

Not every dataset will perfectly match your checklist or preferred methods.

Some datasets may require different tools or extra investigation.

However, having a checklist and preferred methods makes common cleaning tasks easier and more organized.

---

# 21. Common Mistakes to Avoid

## Mistake 1: Cleaning without a plan

Without a plan, it is easier to miss errors or waste time.

## Mistake 2: Using the same method for every dataset

Different datasets may need different cleaning techniques.

## Mistake 3: Ignoring dataset size

Large datasets may need more time and stronger tools.

## Mistake 4: Forgetting missing data

Missing values can affect accuracy and fairness.

## Mistake 5: Ignoring data types

Different data types need different cleaning methods.

## Mistake 6: Not checking alignment with the business objective

Clean data still needs to be relevant to the problem being solved.

---

# 22. Key Takeaways

- Raw data is often messy and imperfect.
- Data cleaning takes time, energy, and attention.
- A cleaning checklist helps analysts identify common data problems.
- A checklist can include dataset size, categories, labels, missing data, formatting, and data types.
- Preferred cleaning methods help analysts decide how to handle common problems.
- Planning cleaning steps saves time and improves consistency.
- Different datasets may require different approaches.
- Thoughtful planning helps protect data integrity and supports reliable analysis.

---

# Final Summary

This reading explains how Data Analysts can develop a personal approach to cleaning data. Since raw data is often messy, analysts should plan their cleaning process before making changes. Two helpful steps are creating a cleaning checklist and deciding on preferred cleaning methods. A checklist helps identify common issues such as dataset size, missing data, inconsistent formatting, categories, labels, and data types. Preferred methods help analysts decide which tools or actions to use for each issue. Although every dataset is different, having a clear approach makes data cleaning faster, more consistent, and more reliable. The main lesson is that thoughtful planning helps ensure data is clean, usable, and ready for accurate analysis.
