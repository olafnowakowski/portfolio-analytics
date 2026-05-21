# Additional Terms and Definitions: Data Integrity, Sampling, and Validation

## Main Idea

These terms are connected to preparing data for analysis.

They focus on:

- checking data quality
- validating data
- understanding sample size
- measuring uncertainty
- making sure analysis results are meaningful and reliable

---

# 1. Data Integrity Terms

## Data Integrity

**Data integrity** is the accuracy, completeness, consistency, and trustworthiness of data throughout its life cycle.

This means data should stay reliable from the moment it is created or collected until it is stored, processed, analyzed, and used.

---

## Accuracy

**Accuracy** is the degree to which data conforms to the actual entity being measured or described.

In simple terms, the data should be correct.

### Example

If a customer’s real age is 35, the dataset should not show 53.

---

## Completeness

**Completeness** is the degree to which the data contains all desired components or measures.

In simple terms, all required data should be present.

### Example

If a customer profile requires name, email, and phone number, the record is incomplete if the phone number is missing.

---

## Consistency

**Consistency** is the degree to which data is repeatable from different points of entry or collection.

In simple terms, the same data should match across different systems, forms, or databases.

### Example

If a customer’s address is different in the sales database and support database, the data is inconsistent.

---

# 2. Data Validation and Constraint Terms

## Data Constraints

**Data constraints** are the criteria that determine whether a piece of data is clean and valid.

Constraints help prevent invalid, missing, or inconsistent data from being used in analysis.

---

## Mandatory

**Mandatory** means a data value cannot be left blank or empty.

### Example

If email address is mandatory, every record must include an email address.

---

## Data Range

**Data range** means numerical values must fall between predefined minimum and maximum values.

### Example

If a survey rating must be between 1 and 5, then 6 is outside the valid data range.

---

## Cross-Field Validation

**Cross-field validation** is a process that ensures certain conditions for multiple data fields are satisfied.

### Example

If several percentage fields must add up to 100%, cross-field validation checks that total.

---

## Regular Expression / RegEx

**Regular expression**, or **RegEx**, is a rule that says values in a table must match a prescribed pattern.

### Example

A phone number may need to follow this pattern:

```text
###-###-####
```

A value that does not match the pattern would fail validation.

---

# 3. Data Handling Terms

## Data Manipulation

**Data manipulation** is the process of changing data to make it more organized and easier to read.

This can include sorting, filtering, formatting, combining, or restructuring data.

---

## Data Replication

**Data replication** is the process of storing data in multiple locations.

Replication can be useful, but it can also create data integrity risks if different copies become out of sync.

---

# 4. Spreadsheet Function Term

## DATEDIF

**DATEDIF** is a spreadsheet function that calculates the number of days, months, or years between two dates.

### Example Use

```excel
=DATEDIF(A2,B2,"D")
```

This calculates the number of days between the date in A2 and the date in B2.

---

# 5. Sampling and Survey Terms

## Random Sampling

**Random sampling** is a way of selecting a sample from a population so that every possible type of sample has an equal chance of being chosen.

Random sampling helps reduce sampling bias.

---

## Estimated Response Rate

**Estimated response rate** is the average number or percentage of people who typically complete a survey.

### Example

If you send a survey to 1,000 people and expect 100 responses, the estimated response rate is:

```text
10%
```

---

# 6. Confidence and Error Terms

## Confidence Level

**Confidence level** is the probability that a sample size accurately reflects the greater population.

### Example

A 95% confidence level means the analyst is aiming for strong confidence that the sample represents the population.

---

## Confidence Interval

**Confidence interval** is a range of values that conveys how likely a statistical estimate reflects the population.

It is usually calculated using the sample result plus or minus the margin of error.

### Example

If the sample result is 60% and the margin of error is 5%, the confidence interval is:

```text
55% to 65%
```

---

## Margin of Error

**Margin of error** is the maximum amount that the sample results are expected to differ from those of the actual population.

A smaller margin of error means more precise results.

### Example

If a survey result is 60% and the margin of error is 5%, the actual population result may be between:

```text
55% and 65%
```

---

# 7. Hypothesis Testing

## Hypothesis Testing

**Hypothesis testing** is a process used to determine whether a survey or experiment has meaningful results.

It helps analysts decide whether results are likely real or possibly caused by random chance.

---

# 8. Quick Reference Table

| Term | Short Definition |
|---|---|
| Accuracy | Data correctly represents what is being measured |
| Completeness | Data contains all required parts |
| Confidence interval | Range of likely values for a population estimate |
| Confidence level | Probability that the sample reflects the population |
| Consistency | Data matches across collection points or systems |
| Cross-field validation | Checks that multiple fields satisfy a condition together |
| Data constraints | Rules that determine whether data is valid |
| Data integrity | Accuracy, completeness, consistency, and trustworthiness of data |
| Data manipulation | Changing data to make it organized and readable |
| Data range | Valid values between a minimum and maximum |
| Data replication | Storing data in multiple locations |
| DATEDIF | Spreadsheet function for calculating time between dates |
| Estimated response rate | Expected percentage of people who complete a survey |
| Hypothesis testing | Process for checking whether results are meaningful |
| Mandatory | A field that cannot be blank |
| Margin of error | Expected difference between sample and population results |
| Random sampling | Selecting a sample so all types have equal chance |
| RegEx | Rule requiring values to match a pattern |

---

# Key Takeaways

- Data integrity depends on accuracy, completeness, consistency, and trustworthiness.
- Data constraints help ensure data is clean and valid.
- Mandatory fields, data ranges, RegEx, and cross-field validation are examples of constraints.
- Data manipulation can make data easier to use, but it must be done carefully.
- Data replication can create risks if copies become inconsistent.
- DATEDIF is useful for calculating time between dates.
- Random sampling helps create a more representative sample.
- Confidence level, confidence interval, and margin of error help analysts understand uncertainty.
- Hypothesis testing helps determine whether results are meaningful.

---

# Final Summary

These terms support the process of preparing reliable data for analysis. Data integrity refers to the accuracy, completeness, consistency, and trustworthiness of data throughout its life cycle. Data constraints, such as mandatory fields, data ranges, RegEx, and cross-field validation, help determine whether data is valid. Sampling terms such as random sampling, confidence level, confidence interval, margin of error, and estimated response rate help analysts understand how well sample results represent a population. Together, these concepts help analysts prepare better data, reduce errors, and make stronger conclusions.
