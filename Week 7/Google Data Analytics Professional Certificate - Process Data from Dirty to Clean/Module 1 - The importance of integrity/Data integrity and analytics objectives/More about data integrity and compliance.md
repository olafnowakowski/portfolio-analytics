# Data Integrity and Data Constraints

## Main Idea

Data integrity is essential for accurate analysis.

A good analysis depends on data that is valid, complete, consistent, clean, and formatted correctly.

Even small issues, such as inconsistent date formats, can lead to major mistakes in analysis and decision-making.

---

# 1. Data Integrity Review

**Data integrity** means the data is accurate, complete, consistent, and trustworthy throughout its lifecycle.

If data integrity is weak, the analysis may be inaccurate even if the analyst uses the correct methods.

---

# 2. Example: Calendar Dates in a Global Company

Calendar dates can be written in different formats depending on the country.

## Common Date Formats

| Format | Meaning | Example |
|---|---|---|
| DD/MM/YY | Day / Month / Year | `12/10/20` = October 12, 2020 |
| YYYY-MM-DD | Year / Month / Day | `2020-10-12` = October 12, 2020 |
| MM/DD/YY | Month / Day / Year | `10/12/20` = October 12, 2020 |

---

# 3. Why Date Formats Matter

If a global company does not standardize date formats, the data may be misunderstood.

For example, `12/10/20` could mean:

- October 12, 2020 in some countries
- December 10, 2020 in others

This could lead to incorrect business decisions.

## Example Problem

A company might order extra inventory for December when it was actually needed in October.

This shows how poor data integrity can directly affect business operations.

---

# 4. Common Format and Data Integrity

Data integrity often depends on using a common format.

A shared standard helps ensure that everyone understands and uses the data the same way.

For dates, companies should agree on one format and make sure all people and systems follow it.

---

# 5. Data Replication Risk

**Data replication** means storing or copying data in multiple locations.

Replication can compromise data integrity if different copies of the data become inconsistent.

## Example

An analyst copies a large dataset to verify date formats.

Because of memory issues, only part of the dataset is copied.

The analyst verifies only the partial dataset, but the full dataset still contains unverified dates.

This creates two versions of the data and can lead to inconsistent results.

## Key Lesson

When data is replicated, make sure the copy is complete and matches the original dataset.

---

# 6. Data Transfer Risk

**Data transfer** means moving or importing data from one place to another.

Data integrity can be compromised during transfer if the data is imported incorrectly.

## Example

An analyst imports standardized date data from a spreadsheet back into a database.

During import, the date field is incorrectly classified as text.

Now some dates are stored as text strings instead of actual date values.

This means the data must be cleaned to restore integrity.

## Key Lesson

When transferring data, check that fields are classified correctly, especially dates, numbers, percentages, and Boolean values.

---

# 7. Data Manipulation Risk

**Data manipulation** means changing data to make it more useful, readable, or organized.

Manipulation can compromise data integrity if changes are made incorrectly.

## Example

An analyst sees what looks like a duplicate record and deletes it.

Later, it turns out the record was not a duplicate. It was a unique record for a company subsidiary.

Now the dataset is missing important data.

## Key Lesson

Before removing records, confirm that they are truly duplicates.

Deleting valid data harms completeness.

---

# 8. How to Maintain Data Integrity

To maintain data integrity:

- Use standard formats.
- Make sure all systems follow the same rules.
- Check that copied data is complete.
- Check that transferred data keeps the correct data types.
- Confirm records before deleting or changing them.
- Validate, clean, and review data before analysis.

---

# 9. Important Rule Before Analysis

Before beginning analysis, always check that the data is:

- valid
- complete
- clean
- consistent
- correctly formatted
- ready for analysis

---

# 10. Data Constraints

**Data constraints** are rules or criteria that determine whether data is valid.

Constraints help protect data integrity by preventing invalid, incomplete, or inconsistent data.

---

# 11. Types of Data Constraints

| Data Constraint | Definition | Example |
|---|---|---|
| Data type | Values must be a certain type, such as date, number, percentage, or Boolean | If the field must be a date, the number `30` would be invalid |
| Data range | Values must fall between a minimum and maximum value | If the range is 10-20, the value `30` is invalid |
| Mandatory | Values cannot be blank or empty | If age is mandatory, the age field must be filled in |
| Unique | Values cannot be duplicated | Two people cannot have the same mobile phone number in the same service area |
| Regular expression / regex | Values must match a required pattern | A phone number must match `###-###-####` |
| Cross-field validation | Multiple fields must satisfy a condition together | Several percentage fields must add up to 100% |
| Primary key | Database value must be unique in a column | A table cannot have two rows with the same primary key |
| Set-membership | Values must come from a specific set of allowed values | A column must contain only Yes, No, or Not Applicable |
| Foreign key | Values must match valid values from another table | A State value must match a valid state listed in a States table |
| Accuracy | Data conforms to the real entity being measured or described | Zip codes validated by street location improve accuracy |
| Completeness | Data contains all required components or measures | If hair and eye color are required and both are collected, the data is complete |
| Consistency | Data is repeatable across different sources or systems | A customer has the same address in both sales and repair databases |

---

# Common Mistakes to Avoid

## Mistake 1: Ignoring date formats

Different countries use different date formats.

Always check the format before analyzing date data.

## Mistake 2: Assuming copied data is complete

When data is replicated, confirm that the full dataset was copied.

## Mistake 3: Importing fields with the wrong data type

A date imported as text can cause problems in analysis.

## Mistake 4: Deleting records too quickly

A record that looks like a duplicate may actually be unique.

## Mistake 5: Starting analysis before validation

Always check that data is valid, complete, and clean before analysis.

---

# 25. Key Takeaways

- Data integrity is essential for accurate analysis.
- Data integrity depends on accuracy, completeness, consistency, and trustworthiness.
- Date formats can create major problems in global datasets.
- A common format helps maintain data integrity.
- Data replication can create incomplete or inconsistent copies.
- Data transfer can cause problems if data types are imported incorrectly.
- Data manipulation can damage data if records are changed or deleted incorrectly.
- Data constraints help determine whether data is valid.
- Constraints include data type, range, mandatory, unique, regex, cross-field validation, primary key, set-membership, and foreign key.
- Always check that data is valid, complete, clean, and consistent before analysis.

---

# Final Summary

This reading explains data integrity through the example of calendar dates in a global company. Since different countries use different date formats, the same date value can be interpreted in multiple ways. If a Data Analyst does not check date formats, the analysis may be inaccurate and lead to poor decisions, such as ordering inventory for the wrong month. Data integrity can also be compromised by replication, transfer, and manipulation. Replication may create incomplete or inconsistent copies, transfer may classify fields incorrectly, and manipulation may accidentally remove valid data. Data constraints help protect integrity by setting rules for valid data, such as required data types, ranges, unique values, mandatory fields, regex patterns, primary keys, foreign keys, and consistency checks. The main lesson is to always verify that data is valid, complete, clean, and consistent before beginning analysis.
