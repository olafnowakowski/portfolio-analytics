# Choosing Between Spreadsheets and SQL

## Main Idea

Data Analysts need to choose the right tool based on:

- the size of the dataset
- the complexity of the data
- where the data is stored
- the type of output needed
- whether the data is stored in one file or multiple related tables

---

# When to Use SQL

Use **SQL** when:

- data is stored in a relational database
- data is spread across multiple tables
- tables need to be joined
- the dataset is large or complex
- you need to filter, aggregate, or rank data efficiently
- you need to query only specific records from a larger dataset

---

# When to Use a Spreadsheet

Use a **spreadsheet** when:

- the dataset is small
- the data is stored in a CSV file
- the task is simple or quick
- you need basic calculations
- you need a simple chart or visualization
- the data does not require complex table relationships

---

# Scenario 1: Identify Top 10 Pet Supply Products

## Situation

A junior Data Analyst works at a major online pet supplies business.

The product development team wants to identify the top 10 products with the highest sales in the last month.

The data comes from multiple database tables:

- product details table
- sales data table

---

## Best Tool

**SQL**

---

## Why SQL Is Best

SQL is appropriate because the data is stored in multiple tables within the company database.

The analyst can use SQL to:

- join product details with sales data
- filter sales from the last month
- calculate total sales by product
- sort products by highest sales
- return the top 10 products

---

## Sample Response

I would use SQL because the product and sales data are stored in multiple related database tables. SQL can join these tables, filter sales from the last month, calculate total sales by product, and return the top 10 results efficiently. I would access the data by querying the company database directly.

---

# Scenario 2: Determine New Store Location

## Situation

A small fitness tech company wants to decide where to build its next retail store.

The manager wants to identify cities with a large population of customers.

The data is stored in a CSV file with 300 records, including:

- names
- phone numbers
- addresses

The manager also wants a quick bar chart for comparison.

---

## Best Tool

**Spreadsheet**

---

## Why a Spreadsheet Is Best

A spreadsheet is appropriate because the dataset is small and stored in a CSV file.

The analyst can use a spreadsheet to:

- import the CSV file
- group customers by city
- count customers in each city
- create a simple bar chart
- make quick comparisons

---

## Sample Response

I would use a spreadsheet because the dataset is small, with only 300 customer records, and the data is already in a CSV file. A spreadsheet can quickly group customers by city and create a simple bar chart for comparison. I would access the data by importing the CSV file into spreadsheet software.

---

# Scenario 3: Customer Satisfaction Survey Results

## Situation

A fashion retailer’s marketing team conducted a customer satisfaction survey.

The results are stored in a CSV file.

The team wants to:

- calculate the average satisfaction score
- compare it to the previous survey average
- segment responses by demographics

Demographic fields include:

- age
- gender
- location

---

## Best Tool

**Spreadsheet**

---

## Why a Spreadsheet Is Best

A spreadsheet is appropriate because the survey results are in a CSV file and the requested analysis is manageable.

The analyst can use a spreadsheet to:

- calculate average satisfaction scores
- compare current and past survey results
- segment data by age, gender, and location
- create quick summaries or charts

---

## Sample Response

I would use a spreadsheet because the survey results are stored in a CSV file and the analysis requires basic calculations and segmentation. A spreadsheet can calculate average satisfaction scores, compare them with the previous survey, and group responses by age, gender, or location. I would access the data by importing the CSV file.

---

# Scenario 4: Calculate Course Completion Rates

## Situation

The manager of an online education platform wants to know which courses have the lowest completion rates.

The data is stored in a relational database with separate tables for:

- user registration
- course enrollment
- course completion

---

## Best Tool

**SQL / Database**

---

## Why SQL Is Best

SQL is appropriate because the data is stored in multiple related database tables.

The analyst can use SQL to:

- join registration, enrollment, and completion tables
- calculate course completion rates
- group results by course
- sort courses by lowest completion rate
- identify courses needing support or improvement

---

## Sample Response

I would use SQL because the data is stored in separate relational database tables for registration, enrollment, and course completion. SQL can join these tables and calculate completion rates efficiently for each course. I would access the data by connecting to the platform’s relational database and running SQL queries.

---

# Comparison Table

| Scenario | Best Tool | Reason |
|---|---|---|
| Identify top 10 pet supply products | SQL | Data is in multiple database tables and needs joins, filtering, ranking, and aggregation |
| Determine new store location | Spreadsheet | Data is small, stored in a CSV file, and needs a simple chart |
| Customer satisfaction survey results | Spreadsheet | Data is in a CSV file and needs averages, comparisons, and demographic segmentation |
| Calculate course completion rates | SQL | Data is in a relational database with multiple connected tables |

---

# Decision Guide

## Choose SQL when:

- the data is stored in a database
- multiple tables must be joined
- the dataset is large
- the analysis requires filtering and aggregation
- relationships between tables matter

## Choose a spreadsheet when:

- the data is stored in a CSV file
- the dataset is small
- the task is quick and simple
- you need a basic visualization
- the analysis can be done with formulas, sorting, filtering, or charts

---

# Big Lesson

The best tool depends on the data and the task.

Spreadsheets are best for smaller, simpler, self-contained datasets.

SQL is best for larger, more complex datasets stored in relational databases.

---

# Key Takeaways

- Data Analysts must choose the right tool for the job.
- SQL is useful for large or complex data stored in databases.
- SQL is especially useful when data comes from multiple related tables.
- Spreadsheets are useful for small CSV files and quick analysis.
- Spreadsheets are good for simple calculations and visualizations.
- The location of the data matters when choosing a tool.
- The complexity of the dataset matters when choosing a tool.
- The desired output also affects tool choice.
- If the data needs joins, use SQL.
- If the data needs a quick chart from a small CSV, use a spreadsheet.

---

# Final Summary

This activity focuses on choosing between spreadsheets and SQL for different workplace scenarios. SQL is the better choice when data is stored in multiple related database tables, such as identifying top-selling pet products or calculating course completion rates. SQL can join tables, filter records, aggregate results, and handle larger datasets efficiently. Spreadsheets are better for smaller CSV-based tasks, such as analyzing 300 customer addresses for store location planning or calculating satisfaction survey averages. Spreadsheets are easier for quick calculations, grouping, filtering, and simple visualizations. The main lesson is that tool choice depends on dataset size, complexity, storage location, and the output needed.
