# Capitalization, indentation, and semicolons.
- You can write your SQL queries in all lowercase and don’t have to worry about extra spaces between words.
- However, using capitalization and indentation can help you read the information more easily
- The semicolon is a statement terminator and is part of the American National Standards Institute (ANSI) SQL-92 standard, which is a recommended common syntax for adoption by all SQL databases. - not all SQL databases have adopted or enforce the semicolon

# WHERE conditions.
```
SELECT field1
FROM table
WHERE field1 = condition;
```
> - The `SELECT` clause identifies the column you want to pull data from by name, field1
> - The `FROM` clause identifies the table where the column is located by name, table. 
> - The `WHERE` clause narrows your query so that the database returns only the data with an exact value match or the data that matches a certain condition that you want to satisfy.

If you are looking for a **specific customer** with the last name *Chavez*, the `WHERE` clause would be: 
```
WHERE field1 = 'Chavez'
```
However, if you are looking for **all customers** with a last name that begins with the letters “*Ch*," the `WHERE` clause would be:
```
WHERE field1 LIKE 'Ch%'
```
`LIKE` clause 
- It allows you to tell the database to look for a certain pattern!

The percent sign `%` is used as a wildcard to match one or more characters.

In the example above, both *Chavez* and *Chen* would be returned. 
> Note that in some databases an asterisk `*` is used as the wildcard instead of a percent sign `%`.

# SELECT all columns. 
-  if you replace `SELECT` field1 with `SELECT *` ,
-  - you would be selecting all of the columns in the table instead of the field1 column only.
> Selecting too much data can cause a query to run slowly.

# Comments
- If *field1* was the column for a customer’s last name, but you wouldn’t know it by the name.
> In these cases, you can place comments alongside your SQL to help you remember what the name represents.

Comments are text placed between certain characters
- `/*`,
- `*/`,
- `--`
<img width="769" height="390" alt="image" src="https://github.com/user-attachments/assets/fd06636b-9007-4ca8-9c5a-6ffea51bf006" />

# Example of a query with comments
Example of how comments could be written in BigQuery:
```
-- Pull basic information from the customer table
SELECT
	customer_id, --main ID used to join with customer_addresss
	first_name, --customer's first name from loyalty program
	last_name --customer's last name
FROM
	customer_data.customer_name
```
# Aliases
Adding **Alias** which is `AS` to the column or table names to make them easier to work with (and avoid the need for comments)
**Example of a query with aliases**
```
SELECT 
	my_table_alias.actual_column_name AS my_column_alias
FROM
	actual_table_name AS my_table_alias
```
> An alias doesn’t change the actual name of a column or table in the database.

# Putting SQL to work as a data analyst
**Example**
- Imagine you are a data analyst for a small business and your manager asks you for some employee data. You decide to write a query with SQL to get what you need from the database.
You want to pull all the columns: **empID, firstName, lastName, jobCode, and salary**. Because you know the database isn’t that big, instead of entering each column name in the `SELECT` clause, you use `SELECT *`.
```
SELECT
	*
FROM
	Employee
```
> This will select all the columns from the Employee table in the FROM clause.

If you want to be specific about the data you want from the **Employee** table. If you want all the data about employees working in the 'SFI' job code, you can use a `WHERE` clause to filter out the data based on this additional requirement. 
```
SELECT
	*
FROM
	Employee
WHERE
	jobCode = 'SFI'
```
<img width="772" height="320" alt="image" src="https://github.com/user-attachments/assets/87ad4408-1849-418d-b86f-070c24aa07e1" />
Suppose you notice a large salary range for the **'SFI'** job code. You might like to flag all employees in all departments with lower salaries for your manager. Because interns are also included in the table and they have salaries **less than $30,000**, you want to make sure your results give you only the full time employees with salaries that are **$30,000 or less**. In other words, you want to exclude interns with the **'INT'** job code who also earn **less than $30,000**. The `AND` clause enables you to test for both conditions. 
```
SELECT
	*
FROM
	Employee
WHERE
	jobCode <> 'INT' 
      AND salary <= 30000;
```
<img width="775" height="286" alt="image" src="https://github.com/user-attachments/assets/a3bb7216-a514-4c0a-a7b0-1f96a0b39cad" />


