# Relational Databases

## Main Idea

A **database** is a collection of data stored in a computer system.

Databases are essential tools for Data Analysts because they help store, organize, manage, and access information.

---

# Why Databases Matter

Databases help Data Analysts:

- store data
- organize data
- access information quickly
- manage large amounts of information
- find insights faster
- make data-driven decisions
- solve business problems

### Important Lesson

Databases make it easier for analysts to find and use the data they need.

---

# Database Structure

A database can contain multiple tables.

Each table stores information about a specific topic.

---

## Car Manufacturer Example

A simple database for a car manufacturer might include tables such as:

- car dealerships
- product details
- repair parts

Each table contains more specific information about that area.

---

# Relational Database

## Definition

A **relational database** is a database that contains a series of related tables that can be connected through their relationships.

---

# How Tables Are Connected

For two tables to have a relationship, one or more of the same fields must exist in both tables.

If a field exists in both tables, that field can be used to connect the tables.

---

## Example

If a **Branch ID** field exists in both a dealership table and another related table, the two tables can be connected using Branch ID.

### Important Lesson

Shared fields allow tables in a relational database to connect.

---

# Keys in Relational Databases

Keys are fields used to identify records and connect tables.

There are two main types of keys:

1. **Primary key**
2. **Foreign key**

---

# Primary Key

## Definition

A **primary key** is an identifier that references a column where each value is unique.

It uniquely identifies each row in a table.

---

## Primary Key Example

In a dealership table, **Branch ID** could be the primary key.

Each dealership branch has a unique Branch ID.

---

## Another Example

In a product details table about cars, **VIN** could be the primary key.

Each car has a unique VIN.

---

# Rules for Primary Keys

A primary key must be:

- unique
- not blank
- not null

---

## Important Notes

A table can have only one primary key.

No two rows can have the same primary key.

The primary key helps make sure each record can be identified clearly.

---

# Foreign Key

## Definition

A **foreign key** is a field in one table that is a primary key in another table.

Foreign keys are used to connect tables.

---

## Foreign Key Example

In a repair parts table, the primary key might be **Part ID**.

Each row represents one unique repair part.

The same table might also include **VIN**.

If VIN is the primary key in the product details table, then VIN is a foreign key in the repair parts table.

---

# Why Foreign Keys Matter

Foreign keys create links between tables.

They help analysts connect related information across a relational database.

---

# Primary Key vs Foreign Key

| Key Type | Meaning | Purpose |
|---|---|---|
| **Primary Key** | A unique identifier for each row in a table | Identifies records |
| **Foreign Key** | A field in one table that is a primary key in another table | Connects tables |

---

# Primary Key Example Table

## Dealership Table

| Branch ID | Branch Name | City |
|---|---|---|
| B001 | North Branch | Dallas |
| B002 | East Branch | Atlanta |
| B003 | West Branch | Phoenix |

In this table:

- **Branch ID** is the primary key.
- Each Branch ID is unique.
- No Branch ID is blank.

---

# Foreign Key Example Table

## Repair Parts Table

| Part ID | Part Name | VIN |
|---|---|---|
| P001 | Brake Pad | VIN123 |
| P002 | Tire | VIN456 |
| P003 | Battery | VIN789 |

In this table:

- **Part ID** is the primary key.
- **VIN** is a foreign key if it connects to the product details table.

---

# Product Details Table Example

| VIN | Model | Year |
|---|---|---|
| VIN123 | Sedan LX | 2023 |
| VIN456 | SUV Sport | 2022 |
| VIN789 | Truck Pro | 2024 |

In this table:

- **VIN** is the primary key.
- The repair parts table can connect to this table using VIN.

---

# One Primary Key, Many Foreign Keys

A table can have:

- only one primary key
- multiple foreign keys

---

## Example

A repair parts table may have:

- **Part ID** as the primary key
- **VIN** as a foreign key
- **Branch ID** as another foreign key
- **Supplier ID** as another foreign key

### Important Lesson

Foreign keys allow one table to connect to multiple other tables.

---

# Why Keys Are Important

Primary and foreign keys help databases:

- avoid duplicate records
- identify each row clearly
- connect related tables
- organize information
- maintain relationships between data
- support accurate analysis

---

# Relational Database Summary

A relational database organizes data into tables.

Those tables are related through shared fields.

Primary keys uniquely identify records.

Foreign keys connect one table to another.

---

# Big Lesson

Relational databases make it possible to organize data across multiple related tables.

Primary keys identify unique records, while foreign keys connect records across tables.

---

# Key Takeaways

- Databases store and organize data.
- Data Analysts use databases to access information and generate insights.
- A relational database contains related tables.
- Tables can be connected when they share one or more fields.
- A primary key uniquely identifies each row in a table.
- A primary key must be unique.
- A primary key cannot be null or blank.
- A table can only have one primary key.
- A foreign key is a field in one table that is a primary key in another table.
- Foreign keys link data between tables.
- A table can have multiple foreign keys.
- Primary and foreign keys are essential for understanding relational databases.

---

# Extra Important Notes

- Branch ID can be a primary key in a dealership table.
- VIN can be a primary key in a product details table.
- Part ID can be a primary key in a repair parts table.
- VIN can be a foreign key in a repair parts table if it links to the product details table.
- Primary keys help keep records unique.
- Foreign keys help connect related information.
- Understanding keys is important for working with databases and SQL.

---

# Final Summary

Databases are essential tools for Data Analysts because they store and organize data, making it easier to manage, access, and analyze information. A relational database is a database made up of related tables. These tables can be connected when they share fields. A primary key is a unique identifier for each row in a table and cannot be blank or null. A foreign key is a field in one table that refers to the primary key in another table, allowing the tables to connect. A table can only have one primary key, but it can have multiple foreign keys. The main lesson is that primary and foreign keys help relational databases organize data clearly and connect related information for analysis.
