# Data Transformation

## Main Idea

**Data transformation** is the process of changing data’s **format, structure, or values**.

Data Analysts often transform data to make it easier to organize, combine, compare, and analyze.

---

# What Is Data Transformation?

## Definition

**Data transformation** means changing data so it becomes more useful for analysis.

This can include changing:

- the format of the data
- the structure of the data
- the values in the data

---

# Common Data Transformation Tasks

Data transformation usually involves:

- adding data
- copying data
- replicating data
- deleting fields
- deleting records
- standardizing variable names
- renaming columns
- moving columns
- combining columns
- joining one dataset with another
- saving a file in a different format

---

# File Format Example

One common example of data transformation is saving a spreadsheet as a different file type.

Example:

- saving a spreadsheet as a **comma-separated values file**
- file extension: **.csv**

---

# Why Transform Data?

Data is transformed so it can be easier to use and analyze.

Main goals include:

1. **Data organization**
2. **Data compatibility**
3. **Data migration**
4. **Data merging**
5. **Data enhancement**
6. **Data comparison**

---

# 1. Data Organization

Better organized data is easier to use.

When data is arranged clearly, analysts can work with it more efficiently.

---

# 2. Data Compatibility

Data compatibility means different applications or systems can use the same data.

This is important when data comes from different sources or systems.

---

# 3. Data Migration

Data migration means moving data from one system to another.

For data migration to work well, the data must have matching formats.

---

# 4. Data Merging

Data merging means combining multiple datasets.

For datasets to be merged correctly, they should have the same or compatible organization.

---

# 5. Data Enhancement

Data enhancement means improving the data by adding more useful or detailed fields.

This can make the data more helpful for analysis.

---

# 6. Data Comparison

Data transformation allows analysts to make fair comparisons.

This is sometimes called an **apples-to-apples comparison**.

It means the data is organized consistently enough to compare correctly.

---

# Example: Data Merging

## Scenario

Mario owns a plumbing company.

He buys another plumbing company and wants to combine the customer information from both companies.

---

## Problem

The acquired company uses a different database.

Because the data is stored differently, Mario cannot immediately merge the two customer lists.

---

## Transformation Needed

Mario needs to:

- transform the format of the acquired company’s data
- make the data compatible with his own database
- remove duplicate rows for customers both companies had in common

---

## Result

After transformation, Mario’s company will have one complete, merged customer database.

### Important Lesson

Data transformation helps combine data from different systems into one usable dataset.

---

# Example: Data Organization

Another reason to transform data is to make it easier to create charts.

A common example is transforming **long data** into **wide data**.

---

# Long Data

## Definition

**Long data** is data where each row contains a single data point for a particular item.

---

## Stock Price Example

In a long stock price dataset, each row might contain:

- stock symbol
- date
- opening stock price

Example structure:

| Symbol | Date | Open |
|---|---|---:|
| AAPL | 2023-01-01 | 130.00 |
| AMZN | 2023-01-01 | 85.00 |
| GOOGL | 2023-01-01 | 90.00 |
| AAPL | 2023-01-02 | 132.00 |
| AMZN | 2023-01-02 | 86.00 |
| GOOGL | 2023-01-02 | 91.00 |

Each row is one data point for one company on one date.

---

# Wide Data

## Definition

**Wide data** is data where each row contains multiple data points for the items identified in the columns.

---

## Stock Price Example

In wide format, each company becomes its own column.

Example structure:

| Date | AAPL | AMZN | GOOGL |
|---|---:|---:|---:|
| 2023-01-01 | 130.00 | 85.00 | 90.00 |
| 2023-01-02 | 132.00 | 86.00 | 91.00 |

Each row shows stock prices for multiple companies on the same date.

---

# Long Data vs Wide Data

| Format | Meaning | Example |
|---|---|---|
| **Long Data** | Each row contains one data point for one item | One row for AAPL on one date |
| **Wide Data** | Each row contains multiple data points across columns | One row for a date with AAPL, AMZN, and GOOGL columns |

---

# Why Transform Long Data to Wide Data?

Wide data can be easier to read and understand.

It is also useful for creating charts that compare several items over the same time period.

---

## Stock Chart Example

If stock price data is transformed from long to wide format, an analyst can create a chart comparing how these companies changed over time:

- Apple
- Amazon
- Google

### Important Lesson

Wide data can make side-by-side comparisons easier.

---

# Does Wide Data Contain Different Information?

No.

The same information from the long format can also appear in the wide format.

The difference is the structure.

The data is organized differently to make it easier to read, compare, or visualize.

---

# When Wide Data Is Preferred

Wide data is preferred when:

- creating tables with a few variables about each subject
- creating charts with a few variables
- comparing straightforward line graphs
- making simple side-by-side comparisons

---

# When Long Data Is Preferred

Long data is preferred when:

- storing many variables about each subject
- working with large amounts of repeated data
- performing advanced statistical analysis
- creating more advanced graphs

---

# Example: Long Data Preferred

Long data may be better for storing:

- 60 years of interest rates for each bank
- many repeated measurements over time
- large datasets with many variables

---

# Summary Table

| Wide Data Is Preferred When | Long Data Is Preferred When |
|---|---|
| Creating tables and charts with a few variables about each subject | Storing many variables about each subject |
| Comparing straightforward line graphs | Performing advanced statistical analysis |
| Making simple side-by-side comparisons | Creating more advanced graphs |

---

# Big Lesson

Data transformation changes data into a more useful structure.

The goal is not to change the meaning of the data, but to make it easier to use for a specific task.

---

# Key Takeaways

- Data transformation changes the format, structure, or values of data.
- Analysts transform data to make it easier to analyze.
- Transformation can involve adding, copying, deleting, renaming, moving, combining, or joining data.
- Saving a file in a new format, such as .csv, is also data transformation.
- Data transformation helps with organization, compatibility, migration, merging, enhancement, and comparison.
- Data merging often requires transformation when two systems store data differently.
- Long data stores one data point per row.
- Wide data stores multiple data points across columns.
- Wide data is often easier for simple charts and comparisons.
- Long data is often better for advanced analysis or storing many variables.
- Transforming long data to wide data can make charts easier to create and understand.

---

# Extra Important Notes

- Data transformation is a common part of data preparation.
- Transformation helps make data analysis-ready.
- Compatible data is easier to move, combine, and compare.
- Removing duplicate records is sometimes part of transformation.
- Long and wide data can contain the same information, just arranged differently.
- The best format depends on the analysis goal.
- Analysts often transform long data to wide data when they want to create simple comparison charts.

---

# Final Summary

Data transformation is the process of changing a dataset’s format, structure, or values so it becomes easier to use and analyze. Common transformation tasks include adding or deleting data, renaming columns, standardizing variable names, joining datasets, removing duplicates, and saving files in different formats. Data transformation supports organization, compatibility, migration, merging, enhancement, and comparison. In the Mario plumbing example, data must be transformed so two customer databases can be merged. Another common transformation is changing long data into wide data. Long data has one data point per row, while wide data places related data points into separate columns. Wide data is often easier for simple charts and comparisons, while long data is useful for advanced analysis and storing many variables.
