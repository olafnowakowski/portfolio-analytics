# Clean Data and Dirty Data

## Main Idea

Clean data is essential for effective analysis.

If data is incomplete, incorrect, duplicated, blank, inconsistent, or irrelevant, it becomes **dirty data**.

Dirty data can make analysis difficult or even impossible, while clean data helps analysts identify patterns, connect information, and make useful conclusions.

---

# 1. What Is Dirty Data?

**Dirty data** is data that is incomplete, incorrect, or irrelevant to the problem you are trying to solve.

Dirty data can include:

- incorrect entries
- repeated data
- blank fields
- inconsistent formats
- irrelevant information
- duplicate records
- null values

---

# 2. Why Dirty Data Is a Problem

Small data mistakes can create big problems later.

Dirty data can lead to:

- inaccurate analysis
- misleading conclusions
- poor business decisions
- wasted time
- financial costs
- confusion among stakeholders

If the data is wrong, the analysis may also be wrong.

---

# 3. What Is Clean Data?

**Clean data** is data that is complete, correct, and relevant to the problem being solved.

Clean data allows analysts to:

- understand information
- analyze data accurately
- identify important patterns
- connect related information
- draw useful conclusions
- support effective decisions

---

# 4. Dirty Data vs Clean Data

| Type of Data | Meaning | Effect on Analysis |
|---|---|---|
| Dirty data | Incomplete, incorrect, duplicated, inconsistent, or irrelevant data | Makes analysis difficult or unreliable |
| Clean data | Complete, correct, consistent, and relevant data | Supports accurate analysis and useful conclusions |

---

# 5. Why Data Cleaning Matters

**Data cleaning** is the process of fixing or removing incorrect, incomplete, duplicated, or irrelevant data.

Data cleaning is important because no dataset is perfect.

Even if data comes from a trusted internal source, analysts should still examine and clean it before analysis.

---

# 6. Internal Data

**Internal data** is data that comes from within a company’s own systems.

Internal data is often cleaner when it has been verified and managed by:

- data engineers
- data warehousing specialists
- data warehouse teams

However, internal data can still have problems and should still be checked.

---

# 7. Role of Data Engineers

**Data engineers** transform data into a useful format for analysis and help create reliable data infrastructure.

They may:

- develop databases
- maintain databases
- test databases
- manage data processors
- build systems that support analysis

Data engineers help make data easier and safer for analysts to use.

---

# 8. Role of Data Warehousing Specialists

**Data warehousing specialists** develop processes and procedures for storing and organizing data effectively.

They help make sure data is:

- available
- secure
- backed up
- organized
- protected from loss

---

# 9. Why Analysts Still Need to Clean Data

Even when data has been handled by data engineers or data warehouse teams, analysts may still need to clean it.

Important rule:

```text
No dataset is perfect.
```

Analysts should always examine the data before beginning analysis.

---

# 10. Example: Duplicate Usernames

## Scenario

A company wants to know how many people use its software program.

The analyst has a spreadsheet with a column called:

```text
Username
```

At first, it may seem possible to count the rows to determine the number of users.

## Problem

One person may have more than one username.

For example, a person may register using:

- different email addresses
- a work account
- a personal account

This creates duplicate user records.

---

# 11. How to Handle Duplicate Data

To clean the dataset, the analyst needs to identify and remove or account for duplicate rows.

After duplicates are handled, the spreadsheet is more accurate and ready for analysis.

---

# 12. External Data

**External data** comes from outside the organization.

Data cleaning is especially important when working with external data because it may come from:

- multiple sources
- different systems
- surveys
- third-party providers
- public datasets

External data may have more inconsistencies than internal data.

---

# 13. Example: Customer Survey Data

## Scenario

A software company surveys customers to learn how satisfied they are with its product.

When reviewing the survey data, the analyst finds several nulls.

---

# 14. Null Values

A **null** means a value does not exist in a dataset.

A null is not the same as zero.

| Value | Meaning |
|---|---|
| Null | No value exists / the field was left blank |
| Zero | The user entered or provided a value of 0 |

---

# 15. Null Example in a Survey

If a survey response is null, it may mean the customer skipped the question.

If a survey response is zero, it means the customer gave zero as their answer.

These two things should not be treated the same.

---

# 16. What to Do With Nulls

When analysts find nulls, they need to decide how to handle them.

Possible options:

1. Filter them out.
2. Keep them and analyze why responses are missing.

---

# 17. Option 1: Filter Out Nulls

If nulls are removed, the analyst should communicate that the sample size is now smaller.

This is important because removing data changes the amount of data used in the analysis.

---

# 18. Option 2: Keep Nulls

Sometimes nulls are useful because they show that customers did not answer a question.

This may reveal a problem with the survey itself.

Possible reasons for null responses:

- the question was confusing
- the question was biased
- the question was poorly written
- customers did not understand what was being asked
- customers chose not to answer

---

# 19. Data Cleaning and Survey Quality

Nulls in survey data can help analysts identify issues with survey design.

If many people skip the same question, the analyst should investigate why.

The problem may not be the customers; it may be the question.

---

# 20. Common Mistakes to Avoid

## Mistake 1: Assuming internal data is always clean

Internal data may be more reliable, but it still needs to be checked.

## Mistake 2: Counting rows without checking duplicates

Duplicate records can cause incorrect counts.

## Mistake 3: Treating null as zero

Null means no value exists. Zero is an actual value.

## Mistake 4: Removing nulls without explanation

If nulls are removed, the smaller sample size should be communicated.

## Mistake 5: Ignoring why data is missing

Missing data can reveal problems with data collection, survey design, or user behavior.

---

# 21. Key Takeaways

- Clean data is important for effective analysis.
- Dirty data is incomplete, incorrect, duplicated, inconsistent, or irrelevant.
- Clean data is complete, correct, and relevant.
- Dirty data can lead to inaccurate conclusions and poor decisions.
- Data engineers help prepare data for analysis.
- Data warehousing specialists help store, organize, secure, and back up data.
- Analysts still need to check and clean data before analysis.
- Duplicate records can make counts inaccurate.
- Null values mean a value does not exist.
- Null is not the same as zero.
- Analysts must decide whether to remove nulls or keep them for further insight.

---

# Final Summary

Clean data is complete, correct, and relevant to the problem being solved. Dirty data is incomplete, incorrect, duplicated, inconsistent, or irrelevant, and it can make analysis unreliable. Data engineers and data warehousing specialists help prepare, organize, secure, and maintain data, but analysts still need to examine and clean datasets before analysis. Common data issues include duplicate records and null values. Duplicate records can lead to inaccurate counts, while null values indicate that a value does not exist and should not be confused with zero. The main lesson is that clean data supports accurate analysis, while dirty data can lead to poor conclusions and bad decisions.
