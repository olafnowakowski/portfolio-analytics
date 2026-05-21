# Aligning Data With Business Objectives

## Main Idea

Good analysis depends on two things:

1. **Clean data**
2. **Data that aligns with the business objective**

Data alignment means the data is relevant to the business problem and can help answer the question being asked.

When data is clean and aligned with the objective, analysts can make accurate conclusions.

---

# 1. What Does Data Alignment Mean?

**Data alignment** means the data matches the business objective.

Good alignment means the data can help:

- solve a business problem
- answer a business question
- support a decision
- determine a course of action

If the data does not align with the objective, the analysis may not be useful even if the data itself is clean.

---

# 2. Formula for Accurate Conclusions

```text
Clean data + alignment to business objective = accurate conclusions
```

This means analysts need to check both:

- whether the data is clean
- whether the data is relevant to the objective

---

# 3. Scenario 1: Impress Me Subscription Service

## Business Objective

Account managers at Impress Me, an online content subscription service, want to know how soon users view content after their subscriptions are activated.

The analyst needs to calculate the time between:

- subscription activation date
- first content access date

---

## Why the Data Aligns

The analyst confirms that:

- the exported spreadsheet data is clean
- the activation date is available
- user information is available
- first content access date is available

Because the needed data exists and is clean, there is good alignment between the data and the business objective.

---

# 4. Data Processing Steps

The analyst uses data from multiple spreadsheets to calculate how many days pass between activation and first usage.

## Step 1: Look Up Activation Date

The analyst looks up the activation date for the account.

Example account:

```text
V&L Consulting
```

Result:

```text
October 21, 2019
```

---

## Step 2: Look Up User Name

The analyst looks up a user belonging to the V&L Consulting account.

Example user:

```text
Maria Ballantyne
```

---

## Step 3: Find First Content Access Date

The analyst finds the first date when Maria accessed content.

Result:

```text
October 31, 2019
```

---

## Step 4: Calculate Time Between Dates

The analyst calculates the time between activation and first content usage.

Activation date:

```text
October 21, 2019
```

First access date:

```text
October 31, 2019
```

Result:

```text
10 days
```

---

# 5. Useful Spreadsheet Functions

## VLOOKUP

**VLOOKUP** is a spreadsheet function that searches for a value in a column and returns related information.

It can save time because the analyst does not need to manually search for names, dates, or account details.

Example use cases:

- look up activation date
- look up user name
- look up first content access date

---

## DATEDIF

**DATEDIF** calculates the difference between two dates.

It can be used to calculate the number of days between activation and first access.

Example logic:

```excel
=DATEDIF(Activation_Date, First_Access_Date, "D")
```

This returns the number of days between the two dates.

---

## DAYS360

**DAYS360** is used in accounting spreadsheets that use a 360-day year.

A 360-day year assumes:

- 12 months
- 30 days per month

---

# 6. Scenario 2: Cloud Gate Webinars

## Business Objective

Cloud Gate, a software company, hosted public webinars as free product introductions.

The analyst and webinar program manager want to identify companies that had five or more people attend the webinars.

The goal is to give this list to sales managers so they can follow up for potential sales.

---

# 7. Webinar Attendance Data

The webinar attendance data includes:

| Field | Example | Notes |
|---|---|---|
| Name | First name + last name | Required |
| Email Address | username@company.com | Required |
| Company | Company name | Optional |

---

# 8. Alignment Plus Additional Cleaning

The data seems to align with the business objective because it contains attendee names, email addresses, and company information.

However, the data still needs cleaning before analysis.

```text
Alignment to business objective + additional data cleaning = accurate conclusions
```

---

# 9. Cleaning Issue 1: Missing Company Names

The company field was optional, so some attendees may have left it blank.

If the company name is missing, the analyst may be able to infer it from the email address.

Example:

```text
username@google.com
```

The analyst may fill in:

```text
Google
```

---

## Important Assumption

This cleaning step assumes that people using company-assigned email addresses attended the webinar for business purposes.

This assumption should be considered carefully because it may not always be true.

---

# 10. Cleaning Issue 2: Inconsistent Names

Attendees could enter any name.

This can create problems if the same person attends multiple webinars using different versions of their name.

Example:

```text
Joe Cox
```

and:

```text
Joseph Cox
```

These may look like two different people, but they could be the same attendee.

---

## Solution

The analyst should validate names against unique email addresses.

If the email address is the same, the analyst can identify that the records belong to the same person.

Then the name can be standardized.

Example:

```text
Joseph Cox → Joe Cox
```

---

# 11. Why Unique Email Addresses Matter

Email addresses are useful because they can help identify unique attendees.

Names can vary, but email addresses are more likely to remain consistent.

Using email addresses helps prevent counting the same person twice.

---

# 12. Scenario 3: A+ Education Tutoring Company

## Business Objective

A+ Education wants to know if there is a minimum number of tutoring hours needed before students improve their assessment scores by at least 10%.

The analyst wants to understand the relationship between:

- tutoring hours
- assessment score improvement

---

# 13. Why the Data Seems Aligned

The analyst initially thinks the data aligns with the business objective because:

- students log in and out of the tutoring system
- tutoring hours are tracked
- assessment scores are recorded regularly

This means the analyst has data about both tutoring time and assessment results.

---

# 14. Newly Discovered Variables

After reviewing the data, the analyst discovers another important variable:

```text
Tutoring session consistency
```

Some students had consistent weekly sessions.

Other students had random schedules, even if their total tutoring hours were the same.

---

# 15. Why the New Variable Matters

Two students may both complete the same number of tutoring hours, but their schedules may be different.

Example:

| Student | Total Tutoring Hours | Schedule |
|---|---|---|
| Student A | 20 hours | Weekly sessions |
| Student B | 20 hours | Random sessions |

These students may not have the same learning experience.

So the data does not align as well with the original objective as the analyst first thought.

---

# 16. Using Data Constraints

A **data constraint** is a rule that limits which data is included in the analysis.

The analyst adds a constraint to focus only on students with consistent weekly sessions.

This helps make the analysis more accurate.

---

## Example Constraint

```text
Only include students with consistent weekly tutoring sessions.
```

This creates a more focused subset of data that better aligns with the business objective.

---

# 17. Alignment Plus Variables Plus Constraints

```text
Alignment to business objective + newly discovered variables + constraints = accurate conclusions
```

This means that when new variables are discovered, analysts may need to adjust the dataset or analysis method.

---

# 18. Why Constraints Help

Constraints help analysts:

- focus on relevant data
- remove misleading comparisons
- control for important variables
- improve accuracy
- keep the data aligned with the objective

---

# 19. Key Lessons From the Three Scenarios

## Scenario 1 Lesson

If the data is clean and contains the needed information, the analyst can use it to answer the business question.

## Scenario 2 Lesson

Even if the data aligns with the objective, it may still need cleaning before analysis.

## Scenario 3 Lesson

If the data only partially aligns with the objective, the analyst may need to use constraints or modify the objective.

---

# 20. Common Data Alignment Questions

Before analysis, ask:

- What is the business objective?
- What question needs to be answered?
- Does the dataset contain the needed fields?
- Is the data clean?
- Are there missing values?
- Are there duplicate records?
- Are there inconsistent entries?
- Are there new variables that affect the analysis?
- Do I need to apply constraints?
- Does the data support the conclusion I want to make?

---

# 21. Common Mistakes to Avoid

## Mistake 1: Assuming clean data is automatically useful

Clean data still needs to align with the business objective.

## Mistake 2: Ignoring missing optional fields

Optional fields, such as company name, may need extra cleaning or validation.

## Mistake 3: Counting the same person twice

Names can vary, so unique identifiers like email addresses may be needed.

## Mistake 4: Ignoring newly discovered variables

New variables can affect whether the data truly supports the objective.

## Mistake 5: Not using constraints

Constraints can help create a more relevant dataset for analysis.

---

# 22. Key Takeaways

- Data must be clean and aligned with the business objective.
- Good alignment means the data is relevant and useful for solving a business problem.
- Clean data plus good alignment can lead to accurate conclusions.
- If data aligns with the objective but needs cleaning, clean it before analysis.
- Optional fields may require extra work, such as filling in company names from email domains.
- Unique identifiers, such as email addresses, can help prevent duplicate counting.
- New variables discovered during analysis may affect the accuracy of conclusions.
- Data constraints can help keep the analysis focused and aligned.
- If data only partially aligns with the objective, modify the objective or use constraints.
- Accurate conclusions depend on using data that supports the business question.

---

# Final Summary

This reading explains how Data Analysts judge whether data aligns with business objectives. Good alignment means the data is relevant and can help solve a business problem or support a decision. In the Impress Me scenario, clean data and good alignment allow the analyst to calculate how long users take to access content after activation. In the Cloud Gate scenario, the data aligns with the objective, but it needs cleaning because company names may be missing and attendee names may be inconsistent. In the A+ Education scenario, the data initially seems aligned, but a new variable, tutoring schedule consistency, affects the analysis. The analyst adds a data constraint to focus on students with consistent weekly sessions. The main lesson is that accurate conclusions depend on clean data, strong alignment with the business objective, and appropriate constraints when new variables appear.
