# Cleaning and Merging Multiple Datasets

## Main Idea

Data Analysts often work with data from more than one source.

When two or more datasets are combined, the data usually needs to be cleaned, standardized, and checked for compatibility before analysis.

This process is especially important when organizations merge, departments share data, or analysts combine multiple sources to answer a business question.

---

# 1. What Is Data Merging?

**Data merging** is the process of combining two or more datasets into a single dataset.

This is common when:

- two organizations merge
- data comes from multiple departments
- data comes from different systems
- analysts need a fuller picture of a business problem
- customer, sales, or membership data is stored in separate places

---

# 2. Example: Organization Merger

A **merger** is an agreement that unites two organizations into one new organization.

In the example, the International Logistics Association and the Global Logistics Association decide to merge.

Because the organizations are combining, their member datasets also need to be combined.

---

# 3. Why Merging Datasets Is Challenging

When two datasets come from different organizations or systems, they are often inconsistent or misaligned.

Common problems include:

- different column structures
- different ID systems
- duplicate members
- different labels for the same category
- different membership types
- inconsistent address formats
- different cleaning standards

---

# 4. Problem 1: Different Address Formats

One organization may store address information differently from another.

## Example

The Global Logistics Association has a separate column for:

```text
Suite, apartment, or unit number
```

The International Logistics Association includes that information inside the street address column.

## Why This Is a Problem

Before merging, both datasets need the same structure.

If one dataset has separate address columns and the other does not, the merged dataset will be inconsistent.

---

# 5. Problem 2: Different Member ID Systems

Different organizations may use different identifiers for the same type of record.

## Example

One organization uses email addresses as member IDs.

Another organization uses numbers as member IDs.

## Why This Is a Problem

The same person could appear in both datasets but be identified differently.

This makes duplicate detection harder.

---

# 6. Problem 3: Duplicate Members

People in the same industry may belong to multiple professional associations.

This means both datasets may contain records for the same person.

## Why Duplicates Matter

If duplicates are not removed, they can cause:

- inflated member counts
- incorrect totals
- inaccurate reports
- confusion during analysis
- poor business decisions

---

# 7. Problem 4: Different Labels and Categories

Different datasets may use different labels to describe the same thing.

## Example

One organization uses:

```text
Young Professional
```

Another organization uses:

```text
Student Associate
```

Both may describe members who are still in school or just starting their careers.

## Why This Is a Problem

If labels are not standardized, the analyst may treat the same membership group as two different groups.

---

# 8. Compatibility

**Compatibility** describes how well two or more datasets are able to work together.

Compatible datasets are easier to merge because they follow similar rules, formats, and structures.

---

# 9. Why Compatibility Matters

Before merging datasets, analysts need to check if the datasets are compatible.

This helps avoid:

- redundancy
- duplicated records
- mismatched columns
- inconsistent categories
- incorrect calculations
- misleading analysis

---

# 10. Key Questions Before Merging Datasets

Before merging, analysts should ask several important questions.

## Question 1: Do I have all the data I need?

The analyst should confirm that the available datasets contain enough information to answer the business question.

### Example

To analyze customer purchases, the analyst may need data about:

- customers
- purchases
- store locations
- where customers shopped

---

## Question 2: Does the data I need exist within these datasets?

The analyst should review the datasets before using them.

This helps the analyst understand:

- what data is included
- what the schema looks like
- whether the data is relevant
- whether the data supports the objective
- whether the data is clean enough to use

---

## Question 3: Do the datasets need to be cleaned?

The analyst should check if either dataset contains dirty data.

Common issues include:

- duplicates
- missing values
- inconsistent formatting
- outdated records
- different labels
- different field structures

---

## Question 4: Are the datasets cleaned to the same standard?

When using more than one source, it is important to know whether each dataset was cleaned in the same way.

The analyst should ask:

- What fields are regularly repeated?
- How are missing values handled?
- How recently was the data updated?
- Are labels standardized?
- Are formats consistent?
- Are duplicates already removed?

---

# 11. Schema

A **schema** describes how data is organized.

This can include:

- table names
- column names
- field types
- relationships between fields
- data structure

Understanding the schema helps analysts know whether datasets can be merged correctly.

---

# 12. Cleaning Standards

Cleaning standards are rules or practices used to make data consistent and reliable.

Examples include:

- using the same date format
- using the same currency format
- using the same labels for categories
- handling missing values consistently
- removing duplicates in the same way
- keeping field names consistent

---

# 13. Tools for Merging and Cleaning Data

Analysts can use different tools depending on the size and complexity of the datasets.

Common tools include:

- spreadsheets
- SQL queries
- database tools
- data cleaning tools

---

# 14. Spreadsheets vs SQL

| Tool | Best For |
|---|---|
| Spreadsheets | Smaller datasets, quick cleaning, manual review |
| SQL | Larger datasets, relational data, complex joins, repeated cleaning tasks |

Both tools can be used to clean, merge, and prepare data for analysis.

---

# 15. Common Mistakes to Avoid

## Mistake 1: Merging without checking compatibility

Datasets may look similar but still use different structures, labels, or formats.

## Mistake 2: Ignoring duplicate records

Duplicate members, customers, or transactions can inflate counts and totals.

## Mistake 3: Keeping different labels for the same category

Different names for the same group should be standardized before analysis.

## Mistake 4: Ignoring schema differences

Different column structures can cause data to merge incorrectly.

## Mistake 5: Assuming both datasets were cleaned the same way

Datasets from different sources may follow different cleaning standards.

---

# 16. Data Merging Checklist

Before merging datasets, ask:

- Do I have all the data I need?
- Does the required data exist in these datasets?
- Are the datasets relevant to the business objective?
- Are the schemas compatible?
- Are the column names and field structures aligned?
- Are there duplicate records?
- Are labels and categories consistent?
- Are missing values handled consistently?
- Were the datasets updated recently?
- Do the datasets need more cleaning before merging?

---

# 17. Key Takeaways

- Data merging combines two or more datasets into one.
- Merging datasets is common when organizations combine or when analysts use multiple data sources.
- Datasets from different sources are often inconsistent or misaligned.
- Common issues include different address formats, different ID systems, duplicates, and inconsistent labels.
- Compatibility means how well datasets can work together.
- Analysts should check whether they have all required data before merging.
- Analysts should review schema, relevance, cleanliness, and cleaning standards.
- Spreadsheets and SQL can both be used to clean and merge data.
- Cleaning and checking compatibility before merging helps prevent inaccurate analysis.

---

# Final Summary

Cleaning and merging multiple datasets is a common task for Data Analysts. Data merging means combining two or more datasets into one. This often happens during organization mergers or when analysts need data from multiple sources. However, merged datasets can create challenges because different sources may use different formats, labels, IDs, or structures. For example, one logistics association may store suite numbers separately while another includes them in the street address. One may use email addresses as member IDs while another uses numbers. Analysts must also watch for duplicate records and inconsistent membership labels. Before merging, analysts should check whether they have all the data they need, whether the data exists in the datasets, whether the datasets need cleaning, and whether they were cleaned to the same standard. The main lesson is that datasets must be compatible, cleaned, and aligned before they can be merged reliably.
