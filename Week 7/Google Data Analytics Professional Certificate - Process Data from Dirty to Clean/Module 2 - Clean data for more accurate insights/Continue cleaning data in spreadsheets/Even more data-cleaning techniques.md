# Even More Data-Cleaning Techniques: Data Mapping

## Main Idea

Data cleaning is not only about fixing individual errors with spreadsheet tools or functions.

Analysts also need to understand how data moves between systems, how it changes, and how to make sure it stays compatible when datasets are merged or transferred.

A key technique for this is **data mapping**.

---

# 1. What Is Data Mapping?

**Data mapping** is the process of matching fields from one database or dataset to another.

It helps make sure that data from different sources can be combined, transferred, or integrated correctly.

---

# 2. Why Data Mapping Matters

Data mapping is important for:

- data migration
- data integration
- data merging
- database updates
- combining datasets from different systems
- making sure fields match correctly
- maintaining data integrity

Without data mapping, data can end up in the wrong place or in the wrong format.

---

# 3. Data Migration and Data Integration

## Data Migration

**Data migration** means moving data from one system or location to another.

Example:

```text
Moving member records from one association database into a new merged database.
```

## Data Integration

**Data integration** means combining data from different sources so it can work together.

Example:

```text
Combining customer data, purchase data, and location data into one analysis-ready dataset.
```

---

# 4. Compatibility

**Compatibility** describes how well two or more datasets are able to work together.

Datasets are compatible when their fields, formats, and structures align well enough to be combined or compared.

---

## Example

One dataset may store a state as:

```text
Maryland
```

Another dataset may store it as:

```text
MD
```

These values mean the same thing, but they are formatted differently.

Data mapping helps identify and resolve these differences.

---

# 5. First Step: Identify What Data Needs to Be Moved

The first step in data mapping is identifying which data needs to be moved.

This includes:

- tables
- fields
- columns
- records
- important identifiers
- values that need to be preserved

---

## Example

In a merger between two logistics associations, both organizations have member IDs.

The analyst needs to identify both member ID fields before mapping them into the new merged dataset.

---

# 6. Define the Desired Format

After identifying the data, analysts need to define the desired format for the destination dataset.

This means deciding what the data should look like after it is moved.

---

## Example

One association uses numeric member IDs.

Another association uses email addresses as member IDs.

The team must decide which format the new merged dataset should use.

Example options:

```text
Numeric member ID
```

or:

```text
Email address member ID
```

---

# 7. Schema

A **schema** is a way of describing how data is organized.

A schema may include:

- table names
- column names
- field types
- relationships
- primary keys
- foreign keys
- data structure

Understanding the schema helps analysts map data correctly.

---

# 8. Primary Key and Foreign Key Review

## Primary Key

A **primary key** is a column where each value is unique.

It uniquely identifies each record in a table.

Example:

```text
Member_ID
```

## Foreign Key

A **foreign key** is a field in one table that refers to a primary key in another table.

Foreign keys help connect related tables.

---

# 9. Why Keys Matter in Data Mapping

Data mapping can be simple or complex depending on the schema and the number of primary and foreign keys.

If multiple tables are connected, analysts must understand those relationships before moving or merging the data.

---

# 10. Data Mapping Tools

For complex projects, analysts can use data mapping software.

These tools can help:

- analyze fields
- match fields between systems
- clean data
- inspect data
- validate data
- create consistent naming conventions
- improve compatibility
- automate parts of data transfer

---

# 11. Choosing a Data Mapping Tool

When selecting a data mapping tool, make sure it supports the file types and systems you are using.

Examples:

- Excel
- SQL
- Tableau
- databases
- spreadsheets
- other business tools

---

# 12. Manual Data Mapping

Data mapping can also be done manually for smaller or simpler projects.

Manual mapping requires the analyst to carefully compare fields and decide where each piece of data should go.

---

# 13. Manual Mapping Step: Determine Field Content

Before moving data, analysts need to understand what each field contains.

This ensures each piece of data ends up in the correct place.

---

## Example

Membership expiration dates from two associations should be consolidated into one column.

Example destination field:

```text
Membership Expiration Date
```

---

# 14. Transforming Data

**Data transformation** means changing data into a consistent format.

This step is needed when the same type of information is stored differently across datasets.

---

## Example: Address Fields

One logistics association stores suite, apartment, or unit number in a separate column.

Another association includes that information in the street address field.

Before merging, the analyst needs to standardize the address format.

---

# 15. Using CONCATENATE for Transformation

**CONCATENATE** is a spreadsheet function that joins two or more text strings together.

It can be used to combine address fields into one consistent format.

---

## CONCATENATE Example

```excel
=CONCATENATE(A2," ",B2)
```

This joins the value in `A2`, a space, and the value in `B2`.

---

# 16. Transferring the Data

After the data is mapped and transformed into a compatible format, it can be transferred to its destination.

Common transfer methods include:

- querying
- import wizards
- drag and drop
- copying and pasting
- database tools
- automated transfer tools

---

# 17. Testing the Mapped Data

After transfer, analysts should test the data to make sure it moved correctly.

Testing helps confirm that the data is:

- clean
- properly formatted
- complete
- compatible
- ready for analysis

---

# 18. Spot Checks

A **spot check** means inspecting a sample of the data to confirm it looks correct.

Spot checks can include checking:

- sample records
- null counts
- formatting
- field values
- duplicates
- totals
- whether data landed in the correct columns

---

# 19. Tools for Testing Data Mapping

Analysts can use previous data-cleaning tools to test mapped data.

Useful tools include:

| Tool | How It Helps |
|---|---|
| Data validation | Checks whether data follows rules |
| Conditional formatting | Highlights missing or unusual values |
| COUNTIF | Counts values that meet a condition |
| Sorting | Helps find duplicates or unusual values |
| Filtering | Shows only records that meet specific criteria |

---

# 20. Why Data Mapping Prevents Bigger Problems

A single mistake during data mapping or merging can spread throughout an organization.

If the data is mapped incorrectly, the same error may appear repeatedly in reports, databases, dashboards, and decisions.

Good data mapping acts like a roadmap that helps data arrive safely and correctly at its destination.

---

# 21. Data Mapping Process Summary

| Step | Purpose |
|---|---|
| Identify data to move | Decide which tables and fields are needed |
| Define destination format | Decide how the data should look after transfer |
| Map fields | Match fields from one dataset to another |
| Transform data | Make formats consistent |
| Transfer data | Move data to its destination |
| Test data | Confirm data is clean, formatted, and compatible |
| Use for analysis | Begin analysis after confirming quality |

---

# 22. Common Mistakes to Avoid

## Mistake 1: Moving data without mapping fields first

Fields from different datasets may not match automatically.

## Mistake 2: Ignoring format differences

Values like `Maryland` and `MD` may represent the same thing but need standardization.

## Mistake 3: Forgetting to define the destination format

You need to know what the final dataset should look like before moving data.

## Mistake 4: Ignoring schema and keys

Primary and foreign keys affect how tables connect.

## Mistake 5: Skipping testing after transfer

Always inspect the merged or transferred dataset before analysis.

---

# 23. Key Takeaways

- Data mapping matches fields from one dataset or database to another.
- Data mapping supports data migration, integration, and merging.
- Compatibility means datasets can work together correctly.
- Different systems may store the same information in different formats.
- Analysts must identify what data needs to move and define the desired destination format.
- Schemas, primary keys, and foreign keys can make mapping more complex.
- Data mapping tools can automate cleaning, matching, inspecting, and validating data.
- CONCATENATE can help transform fields into a consistent format.
- After transferring data, analysts should test and spot-check it.
- Good data mapping protects data integrity and prevents errors from spreading.

---

# Final Summary

Data mapping is the process of matching fields from one database or dataset to another. It is important when data is migrated, integrated, merged, or transferred between systems. Because different systems store data differently, analysts must identify what data needs to move, define the desired format, map fields correctly, transform inconsistent data, and test the final result. For example, one dataset may store a state as `Maryland`, while another stores it as `MD`; data mapping helps make these values compatible. Tools like CONCATENATE, data validation, conditional formatting, COUNTIF, sorting, and filtering can support the process. The main lesson is that data mapping provides a roadmap for moving data safely and accurately so it is ready for reliable analysis.
