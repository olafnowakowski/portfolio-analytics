# SQL Queries and Filtering Data in Databases

## Main Idea

Sorting and filtering help Data Analysts focus on the exact data they need.

In spreadsheets, analysts use sorting and filtering tools.

In databases, analysts use **SQL queries** to view specific data from large datasets.

---

# Why SQL Queries Matter

Sometimes a dataset is too large to download or too large to fit in a spreadsheet.

In those cases, Data Analysts use SQL to request only the data they need.

SQL helps analysts:

- view selected data
- filter large datasets
- inspect data before analysis
- work with relational databases
- focus on relevant records
- avoid downloading unnecessary data

---

# Quick Review: Database

## Definition

A **database** is a collection of data stored in a computer system.

Databases help analysts store, access, organize, and analyze large amounts of data.

---

# Quick Review: SQL

## Definition

**SQL** stands for **Structured Query Language**.

SQL is a language Data Analysts use to communicate with databases.

---

# Query Language

A **query language** is used to ask a database for specific information.

SQL is one of the most common query languages used by Data Analysts.

---

# Relational Databases

## Definition

A **relational database** contains a series of tables that can be connected through relationships.

These relationships are represented by:

- primary keys
- foreign keys

---

# Primary and Foreign Keys

## Primary Key

A **primary key** uniquely identifies each row in a table.

## Foreign Key

A **foreign key** is a field in one table that connects to a primary key in another table.

These keys allow analysts to connect related tables.

---

# Why Preview Data?

Before writing or running queries, analysts often preview the dataset.

Previewing helps analysts:

- understand what the dataset contains
- check if the data is useful for the project
- inspect a few rows before querying
- identify possible data quality issues
- confirm the dataset is relevant

---

# Table Viewer

A **Table Viewer** lets analysts view available datasets and inspect tables.

Some table viewers allow users to preview a few rows before writing a query.

---

# Example Dataset: Solar Potential

The lesson uses a sample dataset about how much sunlight hits rooftops in a year.

This type of data could be useful for a solar energy project.

---

# Solar Energy Example

A Data Analyst working on a solar energy project might use this dataset to study:

- regions
- states
- yearly sunlight
- solar potential by location
- postal code-level solar information

---

# Finding the Dataset Name

Before writing a query, analysts need the complete and correct dataset name.

In BigQuery, selecting **Query table** shows the dataset name inside backticks.

---

# Backticks in SQL

Backticks can make a dataset name easier to read in a query.

In some cases, the query can still run without backticks.

---

# Database Name and Table Name

In a full dataset name:

- the words before the dot represent the database name
- the words after the dot represent the table name

---

# Basic SQL Query Structure

Most SQL queries begin with:

SELECT

Then analysts specify what data they want.

---

# SELECT

## Meaning

**SELECT** tells the database which columns to return.

---

# Asterisk in SQL

## Symbol

*

## Meaning

The asterisk means **all columns**.

---

# SELECT *

`SELECT *` tells the database to return every column in the selected table.

This is useful when analysts want to inspect the full dataset.

---

# FROM

## Meaning

**FROM** tells the database where the data is coming from.

It identifies the table or dataset being queried.

---

# Query to View an Entire Dataset

A basic query to view all columns in a dataset follows this structure:

SELECT *
FROM dataset_name

---

# Why Use SELECT *?

Using an asterisk is a shortcut.

Without it, analysts would need to type every column name manually.

---

# Query Formatting

SQL queries can be written in different ways and still return the same results.

For example, a query can be written:

- on multiple lines
- on one long line

The result may be the same.

---

# Why Format SQL Clearly?

Extra lines and spaces do not usually change the query result.

However, formatting helps make the query:

- easier to read
- easier to understand
- easier to edit
- easier to share with others

---

# Filtering Data With WHERE

## Definition

The **WHERE** clause filters data based on a condition.

It allows analysts to view only rows that meet specific criteria.

---

# Example: Filter for Pennsylvania

Suppose an analyst wants to see only solar potential data for Pennsylvania.

The query would use:

- SELECT *
- FROM the solar potential dataset
- WHERE state_name = 'Pennsylvania'

---

# SQL String Values

In SQL, text values are called strings.

Strings are usually written inside single quotes.

## Example

'Pennsylvania'

The single quotes show where the string begins and ends.

---

# Example SQL Query

SELECT *
FROM solar_potential_dataset
WHERE state_name = 'Pennsylvania'

---

# What This Query Does

This query returns:

- all columns
- from the solar potential dataset
- only for rows where the state_name is Pennsylvania

---

# SQL vs Spreadsheet Filtering

| Tool | How Filtering Works |
|---|---|
| **Spreadsheet** | Use filter menus to show matching rows |
| **SQL Database** | Use a WHERE clause to return matching rows |

---

# Why SQL Is Useful for Large Datasets

SQL lets analysts work with datasets that are too large for spreadsheets.

Instead of downloading everything, analysts can query only what they need.

---

# Data Analysts Use SQL To

- inspect datasets
- select columns
- filter rows
- query large datasets
- work with relational tables
- prepare data for analysis
- find relevant information
- reduce unnecessary data

---

# Module Review

This lesson reviews several important skills:

- understanding metadata
- accessing internal and external data
- sorting spreadsheet data
- filtering spreadsheet data
- using SQL queries
- previewing datasets
- filtering database results

---

# Metadata Review

**Metadata** describes what data is about.

It helps keep data organized by explaining the context, structure, source, and meaning of the data.

---

# Internal and External Data Review

## Internal Data

Data from inside an organization.

## External Data

Data from outside an organization.

Data Analysts use both to find insights and solve business problems.

---

# Sorting and Filtering Review

Sorting and filtering help analysts pinpoint the information they need.

These tools make large datasets easier to understand and analyze.

---

# Big Lesson

SQL is the database version of filtering and focusing data.

It allows analysts to communicate with databases and request exactly the information needed for analysis.

# Question

In an existing company database, the customers table contains the following columns: CustomerId, FirstName, LastName, Company, Address, City, State, Country, PostalCode, Phone, Fax, Email, and SupportRepId.

Create a query to return all the columns in the customer table for only customers in Germany.

`SELECT` *
`FROM` customers
`WHERE` Country = 'Germany'

---

# Key Takeaways

- Sorting and filtering help analysts customize information.
- Databases can be too large to download or fit in spreadsheets.
- SQL allows analysts to query specific data from large datasets.
- SQL stands for Structured Query Language.
- Data Analysts use SQL to communicate with databases.
- A relational database contains connected tables.
- Primary and foreign keys represent relationships between tables.
- Table viewers can help preview data before writing a query.
- Previewing data helps analysts check whether a dataset is useful.
- Most SQL queries begin with SELECT.
- `SELECT *` returns all columns.
- FROM identifies where the data comes from.
- WHERE filters rows based on a condition.
- Single quotes are used around string values in SQL.
- SQL queries can be formatted in different ways and still return the same results.
- Clear formatting makes SQL easier to read and share.
- SQL helps analysts focus on relevant data without downloading everything.

---

# Extra Important Notes

- Always inspect a dataset before using it for analysis.
- Use the complete and correct dataset name in a query.
- Backticks can make dataset names easier to read.
- The database name usually appears before the dot.
- The table name usually appears after the dot.
- Use an asterisk when you want all columns.
- Use WHERE when you need only specific rows.
- SQL is especially useful for large datasets.
- Query writing becomes easier with practice.

---

# Final Summary

This lesson explains how Data Analysts use SQL to focus on relevant data in large databases. Sorting and filtering are useful in spreadsheets, but some datasets are too large to download or fit in a spreadsheet. In those cases, analysts use SQL queries to request specific information from a database. SQL stands for Structured Query Language, and it allows analysts to communicate with databases. A basic query uses SELECT to choose columns and FROM to identify the dataset. Using `SELECT *` returns all columns. Analysts can add a WHERE clause to filter rows, such as showing only records where the state name is Pennsylvania. The lesson also explains the importance of previewing datasets before querying them and formatting SQL clearly so it is easier to read and share. The main lesson is that SQL helps analysts inspect, filter, and retrieve exactly the data they need from large datasets.
