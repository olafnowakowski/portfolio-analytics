# Course 3, Module 3: Terms and Definitions

## Main Topic

This module focuses on:

- databases
- metadata
- metadata repositories
- data governance
- CSV files
- SQL query basics
- database keys
- schemas
- normalized databases

---

# Metadata Terms

## Metadata

**Metadata** is data about data.

It describes information such as:

- what the data is
- where it came from
- how it is organized
- when it was created
- how it should be understood

---

## Administrative Metadata

**Administrative metadata** is metadata that indicates the technical source of a digital asset.

### Examples

Administrative metadata may include:

- file type
- creation date
- file size
- device used
- permissions
- technical source information

---

## Descriptive Metadata

**Descriptive metadata** is metadata that describes a piece of data and can be used to identify it later.

### Examples

Descriptive metadata may include:

- title
- author
- subject
- keywords
- ISBN
- description

---

## Structural Metadata

**Structural metadata** is metadata that indicates how a piece of data is organized and whether it is part of one or more data collections.

### Examples

Structural metadata may describe:

- how pages form chapters
- how tables relate to each other
- how files are grouped
- how datasets are connected

---

## Metadata Repository

A **metadata repository** is a database created to store metadata.

It helps organizations manage information about their data in one place.

---

# Data Management Terms

## Data Governance

**Data governance** is a process for ensuring the formal management of a company’s data assets.

It helps manage:

- data security
- data privacy
- data quality
- data integrity
- data access
- data usage

---

## Naming Conventions

**Naming conventions** are consistent guidelines that describe the content, creation date, and version of a file in its name.

### Example

A file name might include:

- project name
- date
- version number

Example:

sales_report_2024_05_v2.csv

---

## Redundancy

**Redundancy** happens when the same piece of data is stored in two or more places.

### Why It Matters

Redundancy can cause:

- duplicated data
- inconsistent records
- storage inefficiency
- update errors

---

# Database Terms

## Normalized Database

A **normalized database** is a database in which only related data is stored in each table.

Normalization helps:

- reduce redundancy
- improve data integrity
- organize data clearly
- reduce complexity

---

## Schema

A **schema** is a way of describing how something, such as data, is organized.

In databases, a schema may describe:

- table names
- column names
- data types
- relationships between tables

---

## Primary Key

A **primary key** is an identifier in a database that references a column in which each value is unique.

### Important Rules

A primary key:

- uniquely identifies each row
- must be unique
- cannot be blank or null

---

## Foreign Key

A **foreign key** is a field within a database table that is a primary key in another table.

### Purpose

Foreign keys connect tables in a relational database.

---

## Primary Key vs Foreign Key

| Term | Meaning | Purpose |
|---|---|---|
| **Primary key** | A unique identifier for each row in a table | Identifies records |
| **Foreign key** | A field that refers to a primary key in another table | Connects tables |

---

# File and Data Format Terms

## CSV File

A **CSV**, or **comma-separated values file**, is a delimited text file that uses commas to separate values.

CSV files are commonly used to transfer data between tools.

### Example

```csv
Name,Age,City
Ava,29,Denver
Liam,34,Austin
Maya,41,Chicago
```

---

## Geolocation

**Geolocation** is the geographical location of a person or device by means of digital information.

### Examples

Geolocation may identify:

- city
- state
- country
- latitude and longitude
- device location

---

# SQL Terms

## SELECT

**SELECT** is the section of a query that indicates the subset of a dataset.

It tells the database which columns to return.

### Example

```sql
SELECT customer_name, sales_amount
```

---

## FROM

**FROM** is the section of a query that indicates where the selected data comes from.

It tells the database which table or dataset to use.

### Example

```sql
FROM sales_table
```

---

## WHERE

**WHERE** is the section of a query that specifies criteria the requested data must meet.

It filters rows based on conditions.

### Example

```sql
WHERE state = 'California'
```

---

## Basic SQL Query Example

```sql
SELECT customer_name, sales_amount
FROM sales_table
WHERE state = 'California';
```

### What This Query Does

This query returns:

- customer names
- sales amounts
- from the sales table
- only for records where the state is California

---

# Programming and Analysis Environment Terms

## Notebook

A **notebook** is an interactive, editable programming environment for creating data reports and showcasing data skills.

Notebooks are often used to combine:

- code
- text explanations
- charts
- outputs
- data analysis steps

---

# Organization Term

## World Health Organization

The **World Health Organization**, or **WHO**, is an organization whose primary role is to direct and coordinate international health within the United Nations system.

---

# Summary Table

| Term | Definition |
|---|---|
| **Administrative metadata** | Metadata that indicates the technical source of a digital asset |
| **CSV file** | A delimited text file that uses commas to separate values |
| **Data governance** | Formal management of a company’s data assets |
| **Descriptive metadata** | Metadata used to describe and identify data later |
| **Foreign key** | A field in one table that is a primary key in another table |
| **FROM** | SQL section that identifies where selected data comes from |
| **Geolocation** | Geographic location of a person or device using digital information |
| **Metadata** | Data about data |
| **Metadata repository** | A database created to store metadata |
| **Naming conventions** | Consistent file-naming guidelines |
| **Normalized database** | A database where only related data is stored in each table |
| **Notebook** | Interactive programming environment for data reports |
| **Primary key** | A unique identifier for rows in a database table |
| **Redundancy** | Same data stored in two or more places |
| **Schema** | Description of how data is organized |
| **SELECT** | SQL section that indicates the subset of a dataset |
| **Structural metadata** | Metadata that shows how data is organized |
| **WHERE** | SQL section that specifies criteria data must meet |
| **World Health Organization** | UN organization coordinating international health |

---

# Big Lesson

Course 3, Module 3 focuses on how data is organized, described, accessed, and queried.

Metadata helps explain data.

Databases help store and structure data.

SQL helps analysts retrieve the exact data they need.

---

# Key Takeaways

- Metadata is data about data.
- Administrative metadata gives technical details about digital assets.
- Descriptive metadata helps identify data later.
- Structural metadata explains how data is organized.
- Metadata repositories store metadata.
- Data governance manages company data assets formally.
- CSV files use commas to separate values.
- Naming conventions help organize files consistently.
- Normalized databases reduce redundancy by storing related data in separate tables.
- Primary keys uniquely identify records.
- Foreign keys connect tables.
- Schemas describe data organization.
- SELECT, FROM, and WHERE are basic SQL query sections.
- Notebooks are interactive environments for data reports.
- The World Health Organization coordinates international health within the UN system.

---

# Final Summary

Course 3, Module 3 introduces important terms related to databases, metadata, SQL, and data organization. Metadata is data about data, and it can be administrative, descriptive, or structural. Metadata repositories store metadata, while data governance ensures formal management of a company’s data assets. CSV files are comma-separated text files used to store and transfer data. In databases, schemas describe how data is organized, primary keys uniquely identify records, and foreign keys connect tables. Normalized databases reduce redundancy by storing only related data in each table. SQL query sections such as SELECT, FROM, and WHERE help analysts request specific data from databases. The main lesson is that understanding metadata, databases, and SQL helps Data Analysts organize, access, and use data effectively.
