# Deciding When to Use SQL or Spreadsheets

## Main Idea

Data Analysts need to choose the right tool based on where the data is stored and what kind of task they need to complete.

If the data is stored in a spreadsheet, spreadsheet tools and formulas may be the best option.

If the data is stored in a database, SQL is usually the best tool.

---

# 1. What Is SQL?

**SQL** stands for:

```text
Structured Query Language
```

SQL is the main language Data Analysts use to extract, organize, clean, and analyze data stored in databases.

---

# 2. Why SQL Is Important

SQL is important because Data Analysts often work with databases.

SQL helps analysts:

- access data in databases
- query large datasets
- filter records
- count records
- remove duplicates
- combine data from tables
- prepare data for further analysis
- answer business questions efficiently

---

# 3. Business Scenario: Social Media Company

A junior Data Analyst works for a social media company.

The company implemented a new business model on:

```text
February 15, 2020
```

The company wants to compare user growth to the previous year.

The analyst is asked to answer this question:

```text
How many users have joined since February 15, 2020?
```

---

# 4. Choosing the Right Tool

Before starting the task, the analyst needs to decide whether to use:

- spreadsheet functions and formulas
- SQL queries

The decision depends mainly on where the data lives.

---

# 5. If the Data Is in a Spreadsheet

If the data is stored in a spreadsheet, the analyst would likely work in the spreadsheet.

They might use:

- pivot tables
- filters
- formulas
- sorting
- spreadsheet functions

## Example Spreadsheet Process

The analyst could:

1. Create a pivot table.
2. Filter users by join date.
3. Count users who joined after February 15, 2020.
4. Make sure duplicate users are not counted more than once.

This process works, but it may involve multiple steps.

---

# 6. If the Data Is in a Database

If the data is stored in a database, SQL is the better tool.

In this scenario, the data is stored in a database.

That means the analyst can answer the business question with one SQL query.

---

# 7. SQL Query Example

The analyst can use this query:

```sql
SELECT
    COUNT(DISTINCT user_id) AS count_of_unique_users
FROM
    table
WHERE
    join_date >= '2020-02-15';
```

---

# 8. What the Query Does

## `SELECT`

```sql
SELECT
```

The `SELECT` clause tells SQL what result to return.

In this case, the analyst wants to return a count of unique users.

---

## `COUNT(DISTINCT user_id)`

```sql
COUNT(DISTINCT user_id)
```

This counts each unique `user_id` only once.

This is useful because one user could appear more than once in the data.

Using `DISTINCT` helps avoid duplicate counting.

---

## `AS count_of_unique_users`

```sql
AS count_of_unique_users
```

This gives the result column a clear name.

Instead of showing a generic function name, the output column will be named:

```text
count_of_unique_users
```

---

## `FROM`

```sql
FROM
    table
```

The `FROM` clause tells SQL which table contains the data.

In a real database, `table` would be replaced by the actual table name.

---

## `WHERE`

```sql
WHERE
    join_date >= '2020-02-15'
```

The `WHERE` clause filters the data.

This condition keeps only users whose join date is on or after:

```text
2020-02-15
```

---

# 9. Why This SQL Query Is Efficient

This query is efficient because it performs the whole task in one step.

It:

- filters users by join date
- counts only unique users
- returns a clear result
- avoids manual spreadsheet steps

---

# 10. Spreadsheets vs SQL Databases

| Feature | Spreadsheets | SQL Databases |
|---|---|---|
| Dataset size | Better for smaller datasets | Better for larger datasets |
| Data entry | Good for manual data entry | Better for stored database records |
| Data access | Works with data inside a spreadsheet | Accesses tables across a database |
| Visualization | Can create charts in the same program | Usually prepares data for visualization in another tool |
| Built-in tools | Spellcheck, formulas, pivot tables, formatting | Fast querying, filtering, joining, and aggregation |
| Collaboration | Best for solo or smaller projects | Better for collaborative database work |
| Query tracking | Limited query history | Can track queries run by users |
| Speed | Can slow down with large data | Fast and powerful for large datasets |

---

# 11. When to Use Spreadsheets

Use spreadsheets when:

- the data is already in a spreadsheet
- the dataset is small or manageable
- you need quick visualizations
- you need manual review
- you are working solo
- you need built-in tools like spellcheck or simple formulas

---

# 12. When to Use SQL

Use SQL when:

- the data is stored in a database
- the dataset is large
- you need to query multiple tables
- you need fast processing
- you need to count, filter, group, or join data
- you are working in a collaborative database environment
- you need repeatable queries

---

# 13. Key Rule

The main factor is where the data lives.

```text
Data in a spreadsheet → use spreadsheet tools
Data in a database → use SQL
```

---

# 14. Common Mistakes to Avoid

## Mistake 1: Using spreadsheets for very large database data

Large datasets may be too slow or difficult to manage in spreadsheets.

## Mistake 2: Using SQL when the data is already simple and spreadsheet-ready

For small spreadsheet tasks, spreadsheet tools may be faster and easier.

## Mistake 3: Forgetting to count unique users

If users can appear more than once, use `DISTINCT` to avoid duplicate counts.

## Mistake 4: Forgetting the date condition

Without the `WHERE` clause, the query would count all users, not only users who joined after the target date.

## Mistake 5: Using unclear column names

Using `AS` helps make query results easier to understand.

---

# 15. Key Takeaways

- SQL is the main tool analysts use to extract data from databases.
- Spreadsheets are useful for smaller datasets and spreadsheet-based analysis.
- SQL is better for large datasets and database queries.
- The tool you use depends mostly on where the data is stored.
- If data is already in a spreadsheet, analysis will usually happen there.
- If data is stored in a database, SQL is usually the best option.
- SQL can answer business questions efficiently with a single query.
- `COUNT(DISTINCT user_id)` counts unique users.
- `WHERE` filters records based on a condition.
- `AS` gives the result column a clear name.

---

# Final Summary

This reading explains how Data Analysts decide whether to use spreadsheets or SQL. The main factor is where the data is stored. If the data is already in a spreadsheet, spreadsheet tools such as formulas, filters, and pivot tables may be the best choice. If the data is stored in a database, SQL is usually the better tool. In the social media company example, the analyst needs to count how many users joined after February 15, 2020. Because the data is stored in a database, the analyst can use one SQL query with `COUNT(DISTINCT user_id)` and a `WHERE` condition to get the result. The main lesson is that SQL is powerful for querying large datasets in databases, while spreadsheets are useful for smaller, spreadsheet-based tasks.
