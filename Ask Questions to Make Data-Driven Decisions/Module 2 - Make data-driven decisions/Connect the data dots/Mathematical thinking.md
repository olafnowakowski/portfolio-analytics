# Mathematical Thinking and Bed Occupancy Rate Notes

## What Is Mathematical Thinking?

**Mathematical thinking** means solving a problem in a logical, step-by-step way.  
It does **not** mean you need to be a math expert. It means breaking a problem into smaller parts so you can understand relationships, patterns, and the best way to analyze the data.

### Why it matters
Mathematical thinking helps data analysts:

- break complex problems into smaller steps
- identify important variables and metrics
- choose the right tools for analysis
- find patterns in data
- make logical, informed decisions

---

## Choosing the Right Tool

One way to decide which tool to use is by looking at the **size of the dataset**.

### Small Data
Small data is:

- focused on specific metrics
- collected over a short, well-defined period
- useful for day-to-day decisions

**Example:**  
Tracking how much water you drink in one day.

**Common tool:**  
- Spreadsheets

---

### Big Data
Big data is:

- larger and less specific at first
- collected over a longer time period
- useful for large-scale questions and business decisions

**Example:**  
Hospital patient and bed usage data collected over time.

**Common tool:**  
- SQL

---

## Hospital Example: Bed Optimization

A hospital may have a problem with **overusing** or **underusing** beds.  
Its goal is to make sure beds are available for patients who need them, while also avoiding wasted money and space from too many empty beds.

This is a good example of using mathematical thinking in data analysis.

---

## Step-by-Step Problem Solving

### 1. Define the problem
The hospital wants to improve how its beds are used.

### 2. Focus on key variables
Important factors include:

- number of beds available
- number of beds used
- time period being studied

### 3. Use a metric
A useful metric for this problem is the **bed occupancy rate**.

---

## Bed Occupancy Rate Formula

**Bed Occupancy Rate =**  
**(Total number of inpatient days for a given period × 100) / (Available beds × Number of days in the period)**

### Formula in plain language
This formula compares:

- how many inpatient days were actually used
- how many bed-days were available in total

It then converts that into a percentage.

---

## What the Bed Occupancy Rate Tells Us

The **bed occupancy rate** shows how fully the hospital is using its available beds.

### If the rate is too low
- too many beds may be unused
- the hospital may be wasting space and money

### If the rate is too high
- the hospital may not have enough beds available
- patient care could be affected

This metric helps the hospital balance efficiency and patient needs.

---

## Why SQL Is a Good Tool Here

Hospitals generate a **large amount of data** over long periods of time.  
Because this is a **big data** problem, SQL is a logical tool choice.

### Why SQL works well
- handles large datasets
- helps organize and query complex data
- makes it easier to analyze long-term patterns

---

## Example Insight

After analyzing the data, the hospital may find that it **always has unused beds**.

### Possible business decision
The hospital could reduce the number of beds, which would save:

- space
- money

Those resources could then be used for something more valuable, such as:

- storing protective equipment
- improving patient support resources

---

## Main Lesson

Mathematical thinking helped the analyst:

- define the problem clearly
- identify the right variables
- use the correct metric
- choose the correct tool
- find a useful pattern in the data
- support a real business decision

---

## Key Terms

### Mathematical thinking
A logical, step-by-step approach to solving problems.

### Small data
Smaller, focused datasets over a short period of time.

### Big data
Large datasets collected over a longer period of time.

### Metric
A measurable value used to track or evaluate something.

### Bed occupancy rate
A metric that measures how much of the hospital’s bed capacity is being used.

---

## Key Takeaways

- Mathematical thinking means solving problems logically and step by step.
- It helps analysts identify patterns and choose the best tools.
- **Small data** is often analyzed with spreadsheets.
- **Big data** is often analyzed with SQL.
- The **bed occupancy rate** helps hospitals understand how efficiently beds are being used.
- Metrics help turn raw data into useful information for decisions.

---

## Quick Summary Table

| Concept | Meaning | Example |
|---|---|---|
| Mathematical thinking | Breaking problems into logical steps | Analyzing hospital bed usage |
| Small data | Specific data over a short period | Daily water intake |
| Big data | Large data over a long period | Hospital records |
| Metric | Measurable value used in analysis | Bed occupancy rate |
| Spreadsheet | Tool for smaller datasets | Personal tracking |
| SQL | Tool for larger datasets | Hospital data analysis |

---

## Short Summary

Mathematical thinking helps data analysts solve problems by breaking them into smaller, logical steps. In the hospital example, the analyst uses the **bed occupancy rate** to measure how efficiently beds are used and chooses **SQL** because the hospital generates large amounts of data over time. This approach helps the hospital make smarter decisions about resources.
