# Principles of Data Integrity

## Main Idea

Before a dataset is ready for analysis, analysts should make sure the data follows key data integrity principles.

The four main principles here are:

- validity
- accuracy
- completeness
- consistency

If data is valid, accurate, complete, and consistent, it is much more reliable for analysis.

---

# 1. Validity

## Definition

**Validity** means using data integrity principles to make sure measures follow defined business rules or constraints.

In simple terms, valid data follows the rules set by the business or system.

---

## Example

Data collected five years ago used technology that is not approved or supported by the business.

This creates a validity issue because the data does not meet current business rules or requirements.

---

## Key Lesson

Data can exist and still not be valid if it does not follow business rules, approved standards, or required constraints.

---

# 2. Accuracy

## Definition

**Accuracy** is the degree to which a measure conforms to a standard or a true value.

In simple terms, accurate data is correct.

---

## Example

Addresses in the business database are identified as incorrect when compared to the public postal service database.

This is an accuracy issue because the stored addresses do not match the trusted standard.

---

## Key Lesson

Accuracy checks whether the data reflects the real-world value or an accepted trusted source.

---

# 3. Completeness

## Definition

**Completeness** is the degree to which all required measures are known.

In simple terms, complete data has all the required information.

---

## Example

A dataset has a `NULL` or missing value for:

```text
Number of employees per store
```

This is a completeness issue because an important required value is missing.

---

## Key Lesson

A dataset may not be ready for analysis if important fields are blank or missing.

---

# 4. Consistency

## Definition

**Consistency** is the degree to which a set of measures is equivalent across systems.

In simple terms, consistent data is stored and represented the same way in different places.

---

## Example

The date of a store opening is stored in both formats:

```text
MM/DD/YYYY
```

and:

```text
MM/YY
```

This is a consistency issue because the same type of data is stored in different formats.

---

## Key Lesson

Data should follow the same format and meaning across systems, tables, and files.

---

# 5. Quick Reference Table

| Principle | Meaning | Example Issue |
|---|---|---|
| Validity | Data follows business rules or constraints | Data collected with unsupported technology |
| Accuracy | Data matches the true value or trusted standard | Address does not match postal service database |
| Completeness | All required values are present | Missing number of employees per store |
| Consistency | Data is equivalent across systems | Store opening date stored in different formats |

---

# 6. Common Mistakes to Avoid

## Mistake 1: Thinking valid and accurate mean the same thing

Valid data follows rules. Accurate data matches the truth.

Data can be valid in format but still inaccurate.

## Mistake 2: Ignoring missing values

Missing values can make analysis incomplete or misleading.

## Mistake 3: Ignoring format differences

Different formats across systems can cause errors when combining or comparing data.

## Mistake 4: Trusting old data without checking business rules

Older data may not meet current standards, tools, or business constraints.

---

# 7. Key Takeaways

- Validity means data follows business rules and constraints.
- Accuracy means data matches the true value or trusted standard.
- Completeness means all required data is present.
- Consistency means data is equivalent across systems or sources.
- A dataset should be checked for validity, accuracy, completeness, and consistency before analysis.
- These principles help make data more trustworthy and analysis more reliable.

---

# Final Summary

The main principles of data integrity are validity, accuracy, completeness, and consistency. Validity checks whether data follows business rules or constraints. Accuracy checks whether data matches a true value or trusted standard. Completeness checks whether all required values are present. Consistency checks whether data is equivalent across systems and stored in the same format. A dataset that meets these principles is better prepared for analysis and more likely to produce reliable conclusions.
