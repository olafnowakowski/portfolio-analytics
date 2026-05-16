# Dynamic Data Imports in Google Sheets

## Main Idea

Data Analysts can import data into Google Sheets in different ways.

Some imports are **static**, meaning they do not update automatically.

Other imports are **dynamic**, meaning they update automatically when the source data changes.

Dynamic imports save time and reduce errors when working with data that changes over time.

---

# Static Imports

## Definition

A **static import** brings data into a spreadsheet once.

If the original source changes later, the imported data does not update automatically.

---

# Example: Importing a CSV File

You can import a **.csv file** into Google Sheets using the **File** menu.

However, if the CSV file is updated later, those updates will not automatically appear in the Google Sheet.

The data must be manually updated.

---

# When Static Imports Are Useful

Static imports can be useful when you want to:

- keep a fixed copy of the data
- track changes you make
- preserve the original imported version
- avoid automatic updates changing your work

---

# Problems With Static Imports

Static imports can be time-consuming when data changes often.

They may require manual and repeated updates.

Maintaining the same dataset in multiple places can also cause errors later.

---

# Dynamic Imports

## Definition

Dynamic data is interactive and automatically changes or updates over time.

A **dynamic import** allows data in one spreadsheet or source to update automatically in another spreadsheet.

---

# Why Dynamic Imports Matter

Dynamic imports help analysts:

- save time
- reduce manual work
- avoid repeated updates
- reduce errors
- keep data consistent across files
- work with changing data more efficiently

---

# General Store Example

## Scenario

A small general store has three cash registers.

Each register is handled by a different clerk.

At the end of each day, the owner wants to calculate:

- total sales
- amount of cash in each register

---

## Manual Process

Without automation, each clerk would need to enter their data into the owner’s spreadsheet.

This would take extra time and effort.

---

## Dynamic Import Process

Each clerk enters their sales total into their own spreadsheet.

The owner’s spreadsheet imports each clerk’s data automatically.

Then the owner’s spreadsheet calculates the total sales for all three registers.

---

## Important Lesson

Dynamic imports save time and help keep related spreadsheets updated automatically.

---

# IMPORT Functions in Google Sheets

Google Sheets has several functions that allow dynamic importing.

The reading introduces three important functions:

1. **IMPORTRANGE**
2. **IMPORTHTML**
3. **IMPORTDATA**

---

# 1. IMPORTRANGE Function

## Definition

The **IMPORTRANGE** function imports all or part of a dataset from another Google Sheet.

---

# What IMPORTRANGE Needs

To use IMPORTRANGE, you need two pieces of information:

1. The URL of the Google Sheet you want to import data from.
2. The sheet name and range of cells you want to import.

---

# IMPORTRANGE Syntax

The structure is:

=IMPORTRANGE("URL", "sheet_name!cell_range")

---

# Important Syntax Note

An exclamation point separates the sheet name and the cell range.

Example structure:

sheet1!A1:F13

This means:

- sheet name: sheet1
- cell range: A1 through F13

---

# IMPORTRANGE Example

=IMPORTRANGE("https://docs.google.com/thisisatestabc123", "sheet1!A1:F13")

This example is only for syntax practice.

It is not meant to be entered into your own spreadsheet.

---

# How to Use IMPORTRANGE

## Steps

1. Open the Google Sheet where you want the imported data to appear.
2. Select the cell where the first imported value should appear.
3. Type an equals sign.
4. Enter the IMPORTRANGE function.
5. Add the source spreadsheet URL.
6. Add the sheet name and cell range.
7. Allow access when prompted.

---

# Allow Access Prompt

The first time you import data from another Google Sheet, a box will appear asking you to allow access.

You must select **Allow access** before the data can be imported.

---

# Why Access Permission Matters

Google Sheets needs permission to connect the destination spreadsheet to the source spreadsheet.

This helps control access to the data.

---

# 2. IMPORTHTML Function

## Definition

The **IMPORTHTML** function imports data from an HTML table or list on a public web page into Google Sheets.

---

# Web Scraping

Importing HTML tables from public web pages is a basic form of extracting web data.

This process is often called **scraping**.

---

# What IMPORTHTML Can Import

IMPORTHTML can import:

- tables
- lists

from web pages.

---

# When IMPORTHTML Is Useful

IMPORTHTML is useful when data is displayed on a public web page in a table or list format.

Example uses:

- importing sports tables
- importing public rankings
- importing web-based lists
- importing publicly available statistics

---

# 3. IMPORTDATA Function

## Definition

The **IMPORTDATA** function imports data from a comma-delimited or tab-delimited file on the web into Google Sheets.

---

# What IMPORTDATA Can Import

IMPORTDATA can import data from files that are:

- comma-delimited
- tab-delimited

---

# Comma-Delimited Data

Comma-delimited data separates values using commas.

This is common in CSV files.

---

# Tab-Delimited Data

Tab-delimited data separates values using tabs.

This is another common plain-text data format.

---

# IMPORTRANGE vs IMPORTHTML vs IMPORTDATA

| Function | What It Imports | Source |
|---|---|---|
| **IMPORTRANGE** | Data from another Google Sheet | Google Sheets |
| **IMPORTHTML** | Tables or lists from a web page | Public HTML web page |
| **IMPORTDATA** | Comma- or tab-delimited data | Web-based file |

---

# Static vs Dynamic Imports

| Import Type | Meaning | Updates Automatically? |
|---|---|---|
| **Static import** | Data is copied once into a spreadsheet | No |
| **Dynamic import** | Data is linked from another source | Yes |

---

# Why Dynamic Imports Reduce Errors

When the same dataset is manually maintained in multiple places, errors can happen.

Dynamic imports reduce this risk because the data updates from the source.

This helps keep spreadsheets aligned.

---

# When Dynamic Imports Are Useful

Dynamic imports are useful when:

- source data changes often
- multiple people update related spreadsheets
- one spreadsheet needs to summarize data from others
- manual updates would be tedious
- consistency is important
- several datasets need to stay connected

---

# When Static Imports May Be Better

Static imports may be better when:

- you need a fixed snapshot of the data
- you want to track changes manually
- the source data should not change your analysis automatically
- you are preserving a historical version

---

# Big Lesson

Google Sheets import functions help analysts bring data into spreadsheets dynamically.

This makes it easier to keep data updated and reduces the need for manual copying.

---

# Key Takeaways

- CSV files can be imported into Google Sheets from the File menu.
- File menu imports are static and do not update automatically.
- Static imports are useful when you want to track changes or keep a fixed copy.
- Static imports can become tedious when data changes often.
- Maintaining the same dataset in multiple places can cause errors.
- Dynamic imports update automatically over time.
- Dynamic data is interactive and changes as the source changes.
- IMPORTRANGE imports data from another Google Sheet.
- IMPORTRANGE requires a source spreadsheet URL and a sheet name with cell range.
- The IMPORTRANGE syntax is `=IMPORTRANGE("URL", "sheet_name!cell_range")`.
- Users must allow access the first time they import from another Google Sheet.
- IMPORTHTML imports tables or lists from public web pages.
- IMPORTHTML is a basic way to scrape data from web pages.
- IMPORTDATA imports comma- or tab-delimited files from the web.
- Dynamic imports help save time, reduce errors, and keep data consistent.

---

# Extra Important Notes

- Imported CSV data does not automatically update in Google Sheets.
- Dynamic imports are helpful when source data changes regularly.
- The exclamation point in IMPORTRANGE separates the sheet name from the cell range.
- IMPORTHTML only works with suitable public web page tables or lists.
- IMPORTDATA works with delimited data available on the web.
- Import functions can make spreadsheets more automated and efficient.
- Automation reduces repeated manual entry.
- Analysts should choose static or dynamic import methods depending on the analysis goal.

---

# Final Summary

This reading explains the difference between static and dynamic data imports in Google Sheets. Importing a CSV file through the File menu creates a static copy, meaning changes to the original CSV do not automatically update the Google Sheet. This can be useful when tracking changes, but it can become tedious and error-prone when the same data must be maintained in multiple places. Dynamic imports solve this problem by automatically updating data over time. Google Sheets includes several import functions for dynamic data: IMPORTRANGE imports data from another Google Sheet, IMPORTHTML imports tables or lists from public web pages, and IMPORTDATA imports comma- or tab-delimited files from the web. The main lesson is that dynamic imports help Data Analysts save time, reduce manual work, and keep datasets consistent across spreadsheets.
