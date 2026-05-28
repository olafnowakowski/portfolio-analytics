# Common SQL Queries for Data Cleaning and Analysis

## Main Idea

SQL has many tools that are similar to spreadsheet tools, but SQL works on a much larger scale.

Data Analysts use SQL queries to request information from databases, extract specific data, insert new records, update existing records, create new tables, and clean up unused tables.

---

# 1. What Is a Query?

A **query** is a request sent to a database.

In SQL, queries are used to ask the database to do something, such as:

- return data
- filter data
- insert new data
- update existing data
- create a table
- delete a table
- prepare data for analysis

SQL stands for:

```text
Structured Query Language
```

So, queries are a central part of using SQL.

---

# 2. SELECT

## Definition

`SELECT` is used to specify which columns or data you want to retrieve from a database table.

It tells SQL what information you want to work with.

---

## Example

```sql
SELECT
    name,
    city
FROM
    customer_data.customer_address;
```

This query returns the `name` and `city` columns from the `customer_address` table inside the `customer_data` dataset.

---

# 3. FROM

## Definition

`FROM` tells SQL where the selected data comes from.

It identifies the table or dataset being queried.

---

## SELECT + FROM Together

`SELECT` and `FROM` are often used together.

```sql
SELECT
    column_name
FROM
    table_name;
```

## Key Lesson

- `SELECT` tells SQL what data you want.
- `FROM` tells SQL where to find that data.

---

# 4. Example: Customer Giveaway

A store is hosting a giveaway for customers in certain cities.

The company has a database with customer information.

The analyst can use SQL to pull only the customer names and cities needed for the giveaway.

Example:

```sql
SELECT
    name,
    city
FROM
    customer_data.customer_address;
```

This helps narrow down which customers may be eligible.

---

# 5. INSERT INTO

## Definition

`INSERT INTO` is used to add new data into a database table.

It tells SQL:

- which table to add data to
- which columns will receive the new data
- what values should be inserted

---

## Example

```sql
INSERT INTO customer_data.customer_address
    (name, address, city)
VALUES
    ('Alex Kim', '123 Main Street', 'Chicago');
```

This inserts a new customer record into the `customer_address` table.

---

# 6. Why Specify Column Names?

When using `INSERT INTO`, it is important to specify the column names.

This tells SQL exactly where each value should go.

Example:

```sql
(name, address, city)
```

This prevents values from being inserted into the wrong fields.

---

# 7. UPDATE

## Definition

`UPDATE` is used to change existing data in a database table.

It is useful when a value needs to be corrected or replaced.

---

## Example

```sql
UPDATE
    customer_data.customer_address
SET
    address = '456 Oak Avenue'
WHERE
    name = 'Alex Kim';
```

This changes the address for one specific customer.

---

# 8. Why WHERE Matters in UPDATE

When using `UPDATE`, the `WHERE` clause is extremely important.

Without `WHERE`, SQL may update every row in the table.

## Dangerous Example

```sql
UPDATE
    customer_data.customer_address
SET
    address = '456 Oak Avenue';
```

This could change the address for every customer.

## Safer Example

```sql
UPDATE
    customer_data.customer_address
SET
    address = '456 Oak Avenue'
WHERE
    name = 'Alex Kim';
```

The `WHERE` clause limits the update to the correct record.

---

# 9. CREATE TABLE IF NOT EXISTS

## Definition

`CREATE TABLE IF NOT EXISTS` creates a new table only if that table does not already exist.

This is useful when analysts need to save query results or create a new table for repeated reporting.

---

## Example

```sql
CREATE TABLE IF NOT EXISTS customer_data.weekend_promotion AS
SELECT
    city,
    COUNT(*) AS customer_count
FROM
    customer_data.customer_address
GROUP BY
    city;
```

This creates a new table with customer counts by city if the table does not already exist.

---

# 10. Query Results vs Saved Tables

Running a SQL query does not always create a permanent table.

Often, query results are only shown temporarily or stored in local memory.

To save results, analysts may need to:

- download results as a spreadsheet or CSV file
- save the results into a new database table

---

# 11. When to Download Query Results

Downloading query results can be useful when you need to work with the data in another tool.

## Example

If you need the total number of customers per day to visualize a weekend promotion, you might download the results as a CSV file and open them in a spreadsheet.

---

# 12. When to Create a New Table

Creating a new table is useful when the same data needs to be pulled regularly.

## Example

If stakeholders ask for the same trend report every week, an analyst can create a table that refreshes with the query results.

This makes reporting faster and more repeatable.

---

# 13. DROP TABLE IF EXISTS

## Definition

`DROP TABLE IF EXISTS` deletes a table only if it already exists.

It is often used to clean up temporary or unused tables.

---

## Example

```sql
DROP TABLE IF EXISTS customer_data.weekend_promotion;
```

This removes the `weekend_promotion` table if it exists.

---

# 14. Important Warning About DROP TABLE

Analysts should be very careful with `DROP TABLE`.

Deleting company tables can remove important data from the database.

Usually, analysts should only delete tables they personally created and no longer need.

---

# 15. SQL Housekeeping

Good SQL housekeeping means keeping the database clean and organized.

This includes removing old, unused, or redundant tables that you created.

Good housekeeping helps prevent:

- cluttered databases
- duplicate tables
- outdated query results
- confusion for other users
- unnecessary storage use

---

# 16. Common SQL Queries Summary

| SQL Query | Purpose |
|---|---|
| `SELECT` | Chooses which data to retrieve |
| `FROM` | Specifies where the data comes from |
| `INSERT INTO` | Adds new data to a table |
| `UPDATE` | Changes existing data |
| `CREATE TABLE IF NOT EXISTS` | Creates a new table if it does not already exist |
| `DROP TABLE IF EXISTS` | Deletes a table if it exists |

---

# 17. Common Mistakes to Avoid

## Mistake 1: Forgetting `FROM`

`SELECT` needs `FROM` so SQL knows where to get the data.

## Mistake 2: Updating without `WHERE`

Without `WHERE`, an `UPDATE` query may change every row in the table.

## Mistake 3: Inserting values into the wrong columns

Always specify column names when inserting data.

## Mistake 4: Assuming query results are automatically saved

Running a query does not always create a permanent table.

## Mistake 5: Dropping important company tables

Only delete tables you are allowed to remove, usually ones you created yourself.

---

# 18. Key Takeaways

- SQL queries are requests sent to a database.
- `SELECT` specifies what data to retrieve.
- `FROM` specifies where the data comes from.
- `INSERT INTO` adds new data to a table.
- `UPDATE` changes existing data in a table.
- `WHERE` is important because it limits which records are affected.
- `CREATE TABLE IF NOT EXISTS` creates a new table only if it does not already exist.
- Query results may need to be downloaded or saved into a new table.
- `DROP TABLE IF EXISTS` helps clean up unused tables.
- Analysts should be careful not to delete important company data.
- SQL is useful for cleaning, preparing, and analyzing data at scale.

---

# Final Summary

This lesson introduces common SQL queries that Data Analysts use for data cleaning and analysis. `SELECT` and `FROM` are used to pull specific data from a database table. `INSERT INTO` adds new records, while `UPDATE` changes existing records. When using `UPDATE`, the `WHERE` clause is important because it prevents changes from being applied to every row. Analysts can use `CREATE TABLE IF NOT EXISTS` to save query results into a new table, especially when they need repeatable reports. They can also use `DROP TABLE IF EXISTS` to remove old or unused tables they created. The main lesson is that SQL queries help analysts work efficiently with databases while keeping data organized and analysis-ready.
