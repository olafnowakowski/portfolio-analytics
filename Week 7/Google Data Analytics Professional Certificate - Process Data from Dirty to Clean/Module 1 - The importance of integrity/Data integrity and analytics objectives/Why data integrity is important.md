# Data Integrity Wrap-Up

## Main Idea

A strong analysis depends on strong data.

If the data is inaccurate, incomplete, inconsistent, or untrustworthy, the analysis can lead to wrong conclusions even if the analyst does everything correctly.

The quality of the analysis depends heavily on the quality of the data being analyzed.

---

# 1. What Is Data Integrity?

**Data integrity** is the accuracy, completeness, consistency, and trustworthiness of data throughout its lifecycle.

This means data should remain reliable from the moment it is created or collected until it is stored, used, transferred, analyzed, and archived.

---

# 2. Why Data Integrity Matters

Data integrity matters because poor-quality data can weaken or ruin an analysis.

If the data is wrong, the conclusions may also be wrong.

This can happen even if the analyst uses the correct tools and methods.

Low data integrity can cause serious problems, such as:

- incorrect analysis results
- incomplete datasets
- inconsistent reports
- poor business decisions
- incorrect medical decisions
- unusable data

Sometimes, even one missing or corrupted piece of data can make an entire dataset unreliable.

---

# 3. Key Qualities of Data Integrity

| Quality | Meaning |
|---|---|
| Accuracy | The data is correct |
| Completeness | No important data is missing |
| Consistency | The data matches across systems, files, or copies |
| Trustworthiness | The data can be relied on for analysis |

---

# 4. Accuracy

**Accuracy** means the data is correct and represents reality.

Example:

If a customer’s purchase total was $75, the dataset should not show $57.

Inaccurate data can lead to incorrect analysis and poor decisions.

---

# 5. Completeness

**Completeness** means all necessary data is present.

A dataset may lack completeness if it has:

- missing rows
- missing columns
- blank fields
- incomplete records
- missing time periods

Incomplete data can make analysis unreliable because the analyst may not have the full picture.

---

# 6. Consistency

**Consistency** means the data matches across different systems, files, or copies.

Example:

If one system shows a customer’s address as London, but another system shows Manchester, the data is inconsistent.

Inconsistent data can cause confusion and conflicting results.

---

# 7. Trustworthiness

**Trustworthiness** means the data is reliable enough to use for analysis.

Trustworthy data usually comes from a credible source and has been collected, stored, and handled properly.

---

# 8. How Data Integrity Can Be Compromised

Data integrity can be at risk whenever data is:

- replicated
- transferred
- manipulated
- copied
- updated
- stored in multiple places
- affected by human or system errors

Every time data is changed or moved, there is a chance something can go wrong.

---

# 9. Data Replication

**Data replication** is the process of storing data in multiple locations.

This can be useful, but it creates risk.

If data is copied at different times or stored in different places, the copies may become out of sync.

## Example

One team may use an older version of the data while another team uses a newer version.

This creates inconsistency and weakens data integrity.

---

# 10. Data Transfer

**Data transfer** is the process of copying data from one place to another.

Examples:

- from a storage device to memory
- from one computer to another
- from one system to another
- from a database into a spreadsheet

If the transfer is interrupted, the dataset may become incomplete.

An incomplete dataset may not be useful for analysis.

---

# 11. Data Manipulation

**Data manipulation** means changing data to make it more organized, readable, or useful for analysis.

Data manipulation is meant to make analysis easier, but mistakes during this process can damage data integrity.

Examples of risky manipulation errors:

- deleting important rows
- changing values incorrectly
- applying the wrong formula
- sorting data incorrectly
- filtering out needed records
- formatting data in a misleading way
- copying and pasting values into the wrong cells

---

# 12. Other Risks to Data Integrity

Data can also be compromised by:

- human error
- viruses
- malware
- hacking
- system failures
- corrupted files
- interrupted processes

These problems can make data incomplete, inaccurate, inconsistent, or unusable.

---

# 13. Human Error

Human error is one of the most common risks to data integrity.

Examples include:

- typing the wrong value
- deleting a row by mistake
- copying data into the wrong place
- using the wrong formula
- saving over the wrong file
- sorting only one column instead of the full dataset

---

# 14. Viruses, Malware, and Hacking

Viruses, malware, and hacking can damage or change data.

They may cause data to become:

- corrupted
- stolen
- altered
- deleted
- unreliable

This is why data security is closely connected to data integrity.

---

# 15. System Failures

System failures can also harm data integrity.

Examples:

- computer crashes
- failed uploads
- interrupted downloads
- server issues
- storage problems
- software errors

If a system fails while data is being saved or transferred, the dataset may become incomplete or corrupted.

---

# 16. Who Helps Protect Data Integrity?

In many companies, the **data warehouse team** or **data engineering team** helps ensure data integrity.

These teams often manage how data is:

- stored
- transferred
- structured
- protected
- validated
- maintained

However, Data Analysts still need to check the data before using it.

---

# 17. What Data Analysts Should Do

Before analysis, Data Analysts should check that data is:

- complete
- valid
- accurate enough for the task
- consistent across sources
- trustworthy
- ready for analysis

This step helps make sure the analysis and conclusions are reliable.

---

# 18. Extra Study Checklist: How to Check Data Integrity

Before analysis, ask:

- Is the data accurate?
- Is the data complete?
- Are there missing values?
- Are there duplicate records?
- Is the data consistent across files or systems?
- Was the data transferred correctly?
- Was the data manipulated or cleaned correctly?
- Is the data from a trustworthy source?
- Is the data valid for the business question?
- Are the formats correct?
- Are the values reasonable?
- Are there obvious outliers or errors?
- Are all required fields included?

---

# 19. Common Data Integrity Risks

| Risk | What Can Go Wrong |
|---|---|
| Data replication | Different copies may become out of sync |
| Data transfer | Interrupted transfer can create incomplete data |
| Data manipulation | Mistakes can change, delete, or damage the data |
| Human error | Values may be entered, deleted, copied, or changed incorrectly |
| Malware or hacking | Data may be corrupted, stolen, or altered |
| System failure | Files or systems may lose or damage data |

---

# 20. Data Integrity and Analysis Quality

Data integrity is important because analysis is only as reliable as the data being analyzed.

If the data has low integrity, the analysis may be flawed from the beginning.

This means the analyst could reach the wrong conclusion even if their formulas, charts, or methods are correct.

---

# 21. Big Lesson

Good analysis depends on good data.

If data integrity is low, the analysis may be flawed before the analyst even begins.

Checking data integrity is a vital part of preparing data for analysis.

---

# Key Takeaways

- Data integrity means data is accurate, complete, consistent, and trustworthy.
- Strong analysis depends on strong data integrity.
- Low data integrity can lead to incorrect conclusions.
- Data can be compromised when it is replicated, transferred, or manipulated.
- Data replication can create out-of-sync copies.
- Data transfer problems can create incomplete datasets.
- Data manipulation errors can damage data quality.
- Human error, malware, hacking, viruses, and system failures can also harm data integrity.
- Data warehouse and data engineering teams often help protect data integrity.
- Data Analysts should still double-check that data is complete and valid before analysis.
- Analysis is only as reliable as the data being analyzed.

---

# Final Summary

Data integrity is the accuracy, completeness, consistency, and trustworthiness of data throughout its lifecycle. It is essential because even a well-performed analysis can produce wrong conclusions if the original data is flawed. Data integrity can be compromised through replication, transfer, manipulation, human error, viruses, malware, hacking, or system failures. Replicated data can become inconsistent, transferred data can become incomplete, and manipulated data can be changed incorrectly. Although data warehouse or data engineering teams often help protect data integrity, Data Analysts must still check that their data is complete, valid, consistent, and trustworthy before beginning analysis. The main lesson is that good analysis depends on good data.
