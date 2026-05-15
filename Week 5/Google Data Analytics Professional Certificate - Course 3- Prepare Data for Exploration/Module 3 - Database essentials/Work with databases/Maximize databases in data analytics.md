# Relational Databases and SQL — Notes

## Main Idea

Databases help analysts **manipulate, store, and process data**.  
This makes it much easier to search through data efficiently and gain useful insights.

---

# Relational Databases

## Definition
A **relational database** is a database that contains a series of tables that can be connected to form relationships.

### What this means
Relational databases allow data analysts to:
- organize data
- link data
- connect tables using shared fields
- find and use data more easily

---

# Why Relational Databases Matter

In a **non-relational table**, all possible variables may be grouped together in one large table.  
This can make the data:
- harder to sort through
- harder to manage
- harder to analyze

By contrast, **relational databases** simplify analysis by splitting data into related tables.

### Benefits of relational databases
- simplify analysis processes
- make data easier to find
- improve data organization
- make data easier to use across an entire database

---

# Normalization

## Definition
**Normalization** is the process of organizing data in a relational database.

### Examples of normalization
- creating tables
- establishing relationships between tables

### Goals of normalization
- eliminate data redundancy
- increase data integrity
- reduce complexity in a database

---

# The Key to Relational Databases

Tables in a relational database are connected by the **fields they have in common**.

These shared fields create relationships between tables.

---

# Primary Key

## Definition
A **primary key** is an identifier that references a column in which each value is unique.

### In simple terms
A primary key is a column used to uniquely identify each record in a table.

### Rules for a primary key
- each value must be unique
- no two rows can have the same primary key value

### Example
If **customer_id** is the primary key in a customer table:
- every customer must have a different customer_id
- no two customers can share the same customer_id

---

# Foreign Key

## Definition
A **foreign key** is a field within a table that is a primary key in another table.

### Purpose
Foreign keys connect one table to another.

### Important note
- a table can have only **one primary key**
- a table can have **multiple foreign keys**

### Why foreign keys matter
They create the relationships between tables in a relational database.

---

# How Keys Help

Primary and foreign keys help:
- organize data
- connect data across multiple tables
- make analysis more efficient
- support data integrity

---

# Tables Without a Primary Key

Some tables do not require a primary key.

### Example
A **revenue table** can:
- have multiple foreign keys
- not have a primary key

---

# Composite Key

## Definition
A **composite key** is a primary key made up of multiple columns.

### Example
If **customer_id** and **location_id** together form a composite key in a customer table:
- the combination of customer_id and location_id must be unique in each row

### Key point
A single column alone may not be unique, but the combination of the two columns must be unique.

---

# Example Database Tables

The reading mentions these example tables:
- customer table
- revenue table
- branch table
- date table
- product table

These tables can be connected through primary keys and foreign keys.

---

# SQL

## Definition
**SQL (Structured Query Language)** is a type of query language that enables data analysts to communicate with a database.

---

# What Analysts Use SQL For

Data analysts use SQL to:
- create queries
- view specific data
- retrieve data from large datasets
- work with related tables in relational databases

### In simple terms
SQL helps analysts ask the database for exactly the data they need.

---

# SQL in Relational Databases

In a relational database, analysts can write SQL queries to get data from related tables.

This is powerful because the data may be spread across multiple connected tables.

---

# Why SQL Is Important

SQL is a powerful tool for working with databases because it helps analysts:
- access data efficiently
- filter data
- connect related tables
- extract useful information for analysis

---

# Key Takeaways

- Databases help analysts store, process, and manipulate data.
- A **relational database** contains related tables that can be connected.
- Relational databases make data easier to organize and analyze.
- **Normalization** organizes data to reduce redundancy, improve integrity, and lower complexity.
- Tables in a relational database are connected using shared fields.
- A **primary key** uniquely identifies each record in a table.
- A **foreign key** is a field that connects one table to another.
- A table can have only one primary key, but it can have multiple foreign keys.
- Some tables may not need a primary key.
- A **composite key** is a primary key made from multiple columns.
- **SQL** is the language analysts use to communicate with databases.
- SQL allows analysts to query and retrieve specific data from related tables.

---

# Final Summary

Relational databases are important because they organize data into connected tables, which makes analysis easier and more efficient. The relationships between tables are created using **primary keys** and **foreign keys**. Normalization improves the structure of the database by reducing duplication and increasing integrity. Some tables may use **composite keys**, and some may not need a primary key at all. Data analysts use **SQL** to interact with relational databases and retrieve the exact data they need for analysis.
