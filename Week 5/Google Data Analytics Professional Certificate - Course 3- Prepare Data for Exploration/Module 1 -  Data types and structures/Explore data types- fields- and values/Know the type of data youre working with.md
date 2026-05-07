# Data Types in Spreadsheets

## Main Idea

A **data type** tells you what kind of value the data is.

In other words, a data type helps you understand what kind of data you are working with.

Knowing data types helps Data Analysts avoid errors and use data correctly.

---

# What Is a Data Type?

## Definition

A **data type** is a specific kind of data attribute that tells what kind of value the data contains.

Data types help identify whether a value is:

- a number
- text
- true or false
- another specific kind of value

---

# Why Data Types Matter

Data types matter because they affect what you can do with the data.

For example:

- numbers can be used in calculations
- text can be sorted or categorized
- Boolean values can show whether something is true or false

### Important Lesson

Using the wrong data type can cause errors in analysis.

---

# Data Types Can Vary by Tool

Different tools and query languages may classify data types differently.

For example, SQL data types can vary depending on the database being used.

In this lesson, the focus is on data types commonly used in spreadsheets.

---

# Common Spreadsheet Data Types

In spreadsheets, data types usually fall into three main categories:

1. **Number**
2. **Text or string**
3. **Boolean**

Some spreadsheet programs may classify data types differently, but these three types cover most spreadsheet data.

---

# Example Spreadsheet

The lesson uses a spreadsheet called:

**Worldwide Interests in Sweets through Google Searches**

This spreadsheet includes Google search interest data for treats such as:

- cupcakes
- ice cream
- candy

The data shows search interest by week.

---

# 1. Number Data Type

## Definition

A **number data type** contains values that can be used in calculations.

Numbers can represent:

- counts
- amounts
- percentages
- currency
- scores
- measurements

---

## Example From the Spreadsheet

Columns B, D, and F contain number data.

Each number represents search interest for:

- cupcakes
- ice cream
- candy

The closer the number is to **100**, the more popular that search term was during that week.

---

# Relative Value

In this example, **100** does not mean there were exactly 100 searches.

Instead, 100 represents the highest search interest during the selected time period.

All other values are measured relative to that peak.

### Example

If ice cream has a value of 100, it means ice cream had peak popularity during that time.

If cupcakes has a value of 50, it means its search interest was half of the peak value.

---

# Number Formats

Number data can be displayed in different formats, such as:

- regular numbers
- percentages
- currency
- decimals

Even if the format changes, the data type can still be numeric.

---

# 2. Text or String Data Type

## Definition

A **text data type**, also called a **string data type**, is a sequence of characters and punctuation that contains textual information.

Text data can include:

- words
- names
- categories
- descriptions
- letters
- punctuation
- numbers that are not used for calculations

---

## Example From the Spreadsheet

Column H shows the most popular treat for each week.

Example:

For the week beginning July 28, 2019, the most popular treat was:

**ice cream**

This is text data because it is a word, not a value used for calculation.

---

# Numbers Can Be Text

Some values may look like numbers but are treated as text.

Examples:

- phone numbers
- street addresses
- ZIP codes
- ID numbers

These values include numbers, but they are not usually used in calculations.

### Important Lesson

A value can contain numbers and still be a text/string data type if it is not meant for math.

---

# 3. Boolean Data Type

## Definition

A **Boolean data type** has only two possible values:

- **TRUE**
- **FALSE**

Boolean data is often used to answer yes/no or true/false questions.

---

## Example From the Spreadsheet

Columns C, E, and G contain Boolean data.

These columns show whether the search interest for each treat is at least **50 out of 100**.

---

## How It Works

A formula checks whether a value is greater than or equal to 50.

Example:

- Cell B4 has a search interest value of 14.
- Cell C4 shows FALSE.
- This is because 14 is less than 50.

If the search interest were 50 or higher, the Boolean result would be TRUE.

---

# Boolean Values Can Appear as Other Words

A formula can be changed so that other words appear instead of TRUE or FALSE.

For example:

- Yes / No
- Pass / Fail
- Above threshold / Below threshold

But if the logic still has only two possible outcomes, it is still Boolean data.

---

# Data Types vs Cell Values

A common spreadsheet issue is confusing data types with cell values.

## Cell Value

A **cell value** is the actual content inside a spreadsheet cell.

## Data Type

A **data type** tells what kind of value that cell contains.

---

# Example: Using a Formula

If a spreadsheet column contains numbers, you can use formulas to calculate values.

Example:

You can calculate the average search interest for cupcakes if the cupcake column contains number data.

---

# Error Example

If you try to calculate an average using text or string data, the spreadsheet may return an error.

This happens because text values cannot be averaged like numbers.

### Important Lesson

Spreadsheet formulas work correctly only when the data type matches the formula.

---

# Why Errors Happen

Errors often happen when:

- data is entered incorrectly
- the wrong data type is used
- text is treated like a number
- numbers are stored as text
- formulas are applied to incompatible values

---

# How Knowing Data Types Helps

Understanding data types helps you:

- choose the right formulas
- avoid spreadsheet errors
- clean data correctly
- analyze data accurately
- understand what each column means
- avoid treating text as numbers
- avoid treating numbers as text

---

# Summary Table

| Data Type | Meaning | Example |
|---|---|---|
| **Number** | Values that can be used in calculations | 14, 50, 100, $25.00 |
| **Text/String** | Characters, words, names, or numbers not used for math | ice cream, cupcakes, phone number |
| **Boolean** | Values with only two possible outcomes | TRUE or FALSE |

---

# Big Lesson

Data types help analysts understand what kind of data they are working with.

The correct data type helps formulas and analysis work properly.

The wrong data type can cause errors.

---

# Key Takeaways

- A data type tells what kind of value the data contains.
- Data types may differ depending on the tool or query language.
- In spreadsheets, common data types include number, text/string, and Boolean.
- Number data can be used in calculations.
- Number data can be displayed as percentages, currency, decimals, or regular numbers.
- Text or string data contains characters and textual information.
- Numbers such as phone numbers or street addresses can be treated as text if they are not used for calculations.
- Boolean data has only two possible values: TRUE or FALSE.
- Boolean data is useful for checking whether a condition is met.
- Confusing data types with cell values can cause spreadsheet errors.
- Formulas must be used with the correct data type.
- Knowing data types helps reduce errors and improve analysis accuracy.

---

# Extra Important Notes

- A number can be formatted in different ways and still be numeric.
- A value that looks like a number may actually be text.
- Boolean data is often created by formulas that test conditions.
- The value 100 in Google Trends-style data may be relative, not an actual count.
- Always understand what a number represents before analyzing it.
- Correct data types make spreadsheets easier to calculate, filter, and interpret.

---

# Final Summary

This lesson explains data types in spreadsheets. A data type tells you what kind of value the data contains. In spreadsheets, the most common data types are number, text or string, and Boolean. Number data can be used in calculations, such as averages or totals. Text or string data contains words, names, descriptions, or numbers that are not meant for calculations, such as phone numbers. Boolean data has only two possible values, TRUE or FALSE, and is often used to test whether a condition is met. Understanding data types helps Data Analysts avoid spreadsheet errors and choose the right formulas for analysis.
