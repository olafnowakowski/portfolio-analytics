# Inspecting Data Before Analysis

## Main Idea

Before starting an analysis, a Data Analyst should inspect the dataset to check whether it contains the information needed to answer stakeholder questions.

A dataset may not always have all the data required for analysis.

---

# Why Inspect Data?

Inspecting data helps analysts determine:

- what questions can be answered
- what questions cannot be answered
- what data is missing
- whether the data is valid
- whether another data source is needed
- what limitations should be communicated to stakeholders

---

# Common Data Problems

A dataset may have several issues.

## 1. The Data Is Not There

The dataset may not contain the type of data needed.

### Example

You have sandwich data, but you need pizza data.

---

## 2. The Data Is Insufficient

The dataset may contain some relevant data, but not enough.

### Example

You have pizza data for June 1-7, but you need data for the entire month of June.

---

## 3. The Data Is Incorrect

The dataset may contain values that seem wrong or unrealistic.

### Example

Your pizza data lists the cost of one slice as $250.

This makes you question whether the dataset is valid.

---

# Scenario: Ice Cream Company

## Role

You are a Data Analyst working for an ice cream company.

## Business Goal

Management wants to improve ice cream sales.

## Available Data

The company has collected limited internal sales data from 2019.

---

# Stakeholder Questions

Management wants answers to these questions:

1. What is the most popular flavor of ice cream?
2. How does temperature affect sales?
3. How do weekends and holidays affect sales?
4. How does profitability differ for new versus returning customers?

---

# Question 1: What Is the Most Popular Flavor?

## First Step

Before answering, define what “popular” means.

Popular could mean:

- the flavor with the most revenue
- the flavor with the most units sold

---

## Available Data

The flavors sheet has:

- 3 columns
- 209 rows

Column headers:

- week
- units sold
- flavor

---

## What the Data Shows

The data appears to show the number of units sold for each ice cream flavor by week in 2019.

---

## How to Answer the Question

Because the dataset includes units sold, you can use total units sold to determine the most popular flavor.

You would calculate the total number of units sold during the year for each flavor.

---

## Data Limitation

The dataset does not provide annual sales amount by flavor.

This means you cannot determine the most popular flavor based on revenue unless another data source is available.

---

## Next Step

Ask stakeholders whether annual sales by flavor is available from another source.

If it is not available, include the limitation in the analysis.

---

# Question 2: How Does Temperature Affect Sales?

## Available Data

The temperatures sheet has:

- 2 columns
- 366 rows

Column headers:

- temperature
- sales

---

## Possible Meaning of the Data

The data could mean one of two things:

1. Total 2019 sales grouped by temperature.
2. A daily snapshot of temperature and sales for each day in 2019.

---

## Most Likely Interpretation

The data is probably a daily snapshot because:

- there are 365 entries for temperature
- multiple rows have the same temperature with different sales values

This suggests each row represents one day.

---

## Uncertainty

You cannot be completely certain without more information.

You also do not know whether the data is in date order.

---

## Next Step

Contact the dataset owner for clarification.

---

## Possible Insight

If temperature affects sales, you could tell stakeholders something like:

When daily highs are above a certain temperature, average ice cream sales increase by a specific amount.

---

## Business Use

This insight could help the company:

- increase inventory during warmer days
- plan staffing
- prepare marketing campaigns
- maximize sales during high-demand periods

---

# Question 3: How Do Weekends and Holidays Affect Sales?

## Available Data

The sales sheet has:

- 2 columns
- 366 rows

Column headers:

- date
- sales

---

## What the Data Likely Shows

The data most likely shows total daily sales in 2019.

This is because sales are recorded for each date in 2019.

---

## How to Analyze It

You can add a new column that identifies whether each date is:

- a weekday
- a weekend
- a holiday

Then you can compare sales across those groups.

---

## Possible Analysis Questions

You could ask:

- Are weekend sales higher than weekday sales?
- Are holiday sales higher than non-holiday sales?
- Do certain holidays increase sales more than others?
- Are there specific days when inventory should be increased?

---

## Business Use

This analysis would help with:

- inventory planning
- marketing planning
- staffing decisions
- promotion timing

---

# Question 4: How Does Profitability Differ for New vs Returning Customers?

## Problem

The dataset does not contain sales data related to new customers.

Because of this, the current dataset cannot answer the question.

---

## Missing Data

To answer this question, you need customer data showing whether a customer is:

- new
- returning

---

## Possible Solution

The company may store customer data in a different table.

If so, you can access that table and join it with the sales data.

---

## How to Analyze It

You would need to:

1. Find the customer data table.
2. Join customer data with revenue or sales data.
3. Categorize sales as new customer sales or returning customer sales.
4. Compare profitability between the two groups.

---

## Business Use

This analysis could help stakeholders:

- build marketing campaigns
- increase brand loyalty
- improve profitability
- better understand customer behavior

---

# Important Analyst Actions

When data is missing or unclear, a Data Analyst should:

- ask questions
- contact the data owner
- identify other useful datasets
- research external sources
- explain limitations clearly
- avoid making unsupported conclusions

---

# Dataset Limitations

The ice cream sales dataset has several limitations:

- It only includes data from 2019.
- It may not contain all variables needed.
- It does not include annual revenue by flavor.
- It does not clearly explain the temperature data.
- It does not include new versus returning customer data.
- It does not come with a full data description.

---

# Why Data Descriptions Matter

A data description helps analysts understand:

- what each column means
- how data was collected
- what each row represents
- whether values are summaries or individual observations
- whether data is complete
- whether data is reliable

Without a data description, analysts may need to infer meaning and confirm details with the data owner.

---

# Answerable vs Not Answerable Questions

| Stakeholder Question | Can It Be Answered With Current Data? | Notes |
|---|---|---|
| What is the most popular flavor? | Partially | Can answer using units sold, but not revenue |
| How does temperature affect sales? | Possibly | Need clarification about temperature data |
| How do weekends and holidays affect sales? | Yes | Add weekend and holiday labels to date data |
| How does profitability differ for new vs returning customers? | No | Need customer data from another table |

---

# Key Takeaways

- Analysts should inspect data before starting analysis.
- Not every dataset contains all the information needed.
- Some data may be missing, insufficient, or incorrect.
- Analysts should identify what questions can and cannot be answered.
- When data is missing, analysts may need other data sources.
- Stakeholder questions may require clarification.
- Definitions matter, such as what “popular” means.
- Data limitations should be clearly communicated.
- Analysts should avoid unsupported conclusions.
- Inspecting data improves the quality of the final analysis.

---

# Big Lesson

Carefully inspecting a dataset helps Data Analysts understand what is possible, what is missing, and what questions need more information.

Good analysis starts with knowing whether the data can actually answer the business question.

---

# Final Summary

This reading explains why Data Analysts must inspect data before beginning an analysis. A dataset may be missing the required data, may not contain enough data, or may include incorrect values. In the ice cream company scenario, management wants to answer questions about popular flavors, temperature effects, weekends and holidays, and customer profitability. Some questions can be answered with the available 2019 internal sales data, while others require clarification or additional datasets. The most popular flavor can be analyzed using units sold, but revenue by flavor is missing. Temperature effects may be analyzed, but the dataset owner should clarify what each row represents. Weekend and holiday effects can be studied by adding date-based labels. Profitability for new versus returning customers cannot be answered without customer data. The main lesson is that inspecting data helps analysts identify answerable questions, missing data, and limitations before making recommendations.
