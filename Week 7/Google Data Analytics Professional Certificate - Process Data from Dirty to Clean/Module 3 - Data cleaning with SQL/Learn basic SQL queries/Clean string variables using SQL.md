# Clean String Variables Using SQL

## Main Idea

SQL can be used to clean and prepare data before analysis.

In this lesson, the focus is on:

- removing duplicates with `DISTINCT`
- checking text length with `LENGTH`
- extracting part of a string with `SUBSTRING`
- removing extra spaces with `TRIM`

These SQL tools help make string variables clean, complete, and consistent.

---

# 1. Why Clean String Variables?

A **string variable** is text data made of characters.

String variables may include:

- names
- addresses
- country codes
- state codes
- customer IDs
- product codes

String variables need cleaning when they are entered differently across a database.

---

# 2. Common String Problems

String variables can have problems such as:

- duplicate values
- inconsistent country codes
- extra spaces
- values that are too long
- values that are too short
- inconsistent formatting
- repeated customer records

These problems can cause incorrect analysis if they are not fixed or accounted for.

---

# 3. Removing Duplicates With DISTINCT

In spreadsheets, analysts can remove duplicates using the **Remove duplicates** tool.

In SQL, analysts can remove duplicates in query results using:

```sql
DISTINCT
```

---

# 4. Example Without DISTINCT

Suppose you want customer IDs from the `customer_address` table.

```sql
SELECT
    customer_id
FROM
    customer_data.customer_address;
```

This query may return duplicate customer IDs if the same customer appears more than once.

---

# 5. Example With DISTINCT

To return only unique customer IDs, use:

```sql
SELECT DISTINCT
    customer_id
FROM
    customer_data.customer_address;
```

This makes each customer ID appear only once in the results.

---

# 6. Why DISTINCT Matters

`DISTINCT` helps prevent duplicate records from affecting analysis.

It is useful when you need:

- unique customer IDs
- unique user IDs
- unique product codes
- unique names
- unique records

---

# 7. LENGTH

## Definition

`LENGTH` is a SQL function that returns the number of characters in a string.

In some databases, this function may be written as:

```sql
LEN
```

Both are used to count characters in a string.

---

# 8. Why LENGTH Is Useful

`LENGTH` is useful when you know how long a string should be.

For example:

- country codes should have 2 characters
- state codes should have 2 characters
- IDs may need a fixed number of characters
- product codes may need a specific length

---

# 9. Example: Check Country Code Length

Suppose the `country` column should contain two-letter country codes.

You can check the length of each country value with:

```sql
SELECT
    LENGTH(country) AS letters_in_country
FROM
    customer_data.customer_address;
```

This returns the number of characters in each country value.

---

# 10. Finding Country Codes That Are Too Long

If country codes should only have 2 letters, you can filter for values longer than 2 characters.

```sql
SELECT
    country
FROM
    customer_data.customer_address
WHERE
    LENGTH(country) > 2;
```

This helps identify values like:

```text
USA
```

when the expected value is:

```text
US
```

---

# 11. Important Rule About Updating Data

If you did not create or own the table, you should not directly update it unless you have permission.

Instead of changing the original table, you can write a query that accounts for the error in your results.

---

# 12. SUBSTRING

## Definition

`SUBSTRING` is a SQL function that extracts part of a text string.

It is useful when you need only part of a value.

---

# 13. SUBSTRING Syntax

```sql
SUBSTRING(column_name, start_position, number_of_characters)
```

| Part | Meaning |
|---|---|
| `column_name` | The column containing the string |
| `start_position` | Where SQL should start extracting characters |
| `number_of_characters` | How many characters SQL should return |

---

# 14. Example: Fix Country Code in Query Results

Suppose some country values are written as:

```text
US
```

and some are written as:

```text
USA
```

To treat both as `US`, use `SUBSTRING` to pull only the first two letters.

```sql
SELECT
    customer_id
FROM
    customer_data.customer_address
WHERE
    SUBSTRING(country, 1, 2) = 'US';
```

This returns customers whose country begins with `US`.

---

# 15. Combining DISTINCT and SUBSTRING

If there are duplicate customer IDs, add `DISTINCT`.

```sql
SELECT DISTINCT
    customer_id
FROM
    customer_data.customer_address
WHERE
    SUBSTRING(country, 1, 2) = 'US';
```

This returns a clean list of unique customer IDs for customers in the United States, including records where the country was entered as `USA`.

---

# 16. TRIM

## Definition

`TRIM` is a SQL function that removes extra spaces from a string.

It removes leading and trailing spaces.

Depending on the database system, it may also help with repeated spaces.

---

# 17. Why TRIM Is Useful

Extra spaces can be difficult to see, but SQL still counts them as characters.

Extra spaces can cause problems when:

- filtering
- grouping
- joining tables
- comparing values
- searching for exact matches

---

# 18. Example: Finding State Codes That Are Too Long

Suppose state codes should have 2 letters.

You can find values longer than 2 characters with:

```sql
SELECT
    state
FROM
    customer_data.customer_address
WHERE
    LENGTH(state) > 2;
```

If the result looks like:

```text
OH
```

but SQL says it has more than 2 characters, there may be an extra hidden space.

Example:

```text
OH 
```

---

# 19. Example: Use TRIM to Remove Extra Spaces

To find all customers in Ohio, including records with extra spaces, use:

```sql
SELECT DISTINCT
    customer_id
FROM
    customer_data.customer_address
WHERE
    TRIM(state) = 'OH';
```

This removes extra spaces from the `state` value before comparing it to `OH`.

---

# 20. SQL String Cleaning Function Summary

| Function | Purpose | Example |
|---|---|---|
| `DISTINCT` | Removes duplicate results | `SELECT DISTINCT customer_id` |
| `LENGTH` | Counts characters in a string | `LENGTH(country)` |
| `LEN` | Alternative to `LENGTH` in some databases | `LEN(country)` |
| `SUBSTRING` | Extracts part of a string | `SUBSTRING(country, 1, 2)` |
| `TRIM` | Removes extra spaces | `TRIM(state)` |

---

# 21. SQL Cleaning Examples

## Remove Duplicate Customer IDs

```sql
SELECT DISTINCT
    customer_id
FROM
    customer_data.customer_address;
```

## Check Country Code Length

```sql
SELECT
    LENGTH(country) AS letters_in_country
FROM
    customer_data.customer_address;
```

## Find Country Codes Longer Than 2 Characters

```sql
SELECT
    country
FROM
    customer_data.customer_address
WHERE
    LENGTH(country) > 2;
```

## Return US Customers Using SUBSTRING

```sql
SELECT DISTINCT
    customer_id
FROM
    customer_data.customer_address
WHERE
    SUBSTRING(country, 1, 2) = 'US';
```

## Return Ohio Customers Using TRIM

```sql
SELECT DISTINCT
    customer_id
FROM
    customer_data.customer_address
WHERE
    TRIM(state) = 'OH';
```

---

# 22. Common Mistakes to Avoid

## Mistake 1: Forgetting DISTINCT

If duplicate records exist, your results may count the same customer more than once.

## Mistake 2: Assuming values are clean because they look clean

A value like `OH` may look correct but still contain a hidden space.

## Mistake 3: Updating tables without permission

If you do not own or control the table, avoid changing the original data directly.

## Mistake 4: Ignoring inconsistent string lengths

String lengths can reveal hidden errors, extra characters, or inconsistent formatting.

## Mistake 5: Forgetting database differences

Some databases use `LENGTH`, while others use `LEN`.

---

# 23. Key Takeaways

- SQL can clean data before analysis.
- `DISTINCT` removes duplicate results.
- `LENGTH` checks how many characters are in a string.
- Some SQL databases use `LEN` instead of `LENGTH`.
- `SUBSTRING` extracts part of a string.
- `TRIM` removes extra spaces from string values.
- String cleaning helps make data consistent.
- Clean string variables prevent errors and miscalculations later.
- SQL lets analysts account for data problems without always changing the original table.

---

# Final Summary

This lesson explains how SQL can be used to clean string variables before analysis. Analysts can use `DISTINCT` to remove duplicate results, `LENGTH` or `LEN` to check whether strings have the expected number of characters, `SUBSTRING` to extract part of a string, and `TRIM` to remove extra spaces. For example, if country values include both `US` and `USA`, `SUBSTRING(country, 1, 2)` can return the first two letters so both values are treated consistently. If a state value such as `OH` contains a hidden space, `TRIM(state)` can remove it before filtering. The main lesson is that SQL string functions help clean inconsistent text data and make results more reliable.
