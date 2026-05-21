# Proxy Data and Open Datasets

## Main Idea

When actual data is not available, analysts can sometimes use **proxy data**.

Proxy data is substitute data that can help estimate, predict, or approximate an outcome when the real data is missing or not ready yet.

Proxy data is useful, but it must be chosen carefully because it may not perfectly represent the real situation.

---

# 1. What Is Proxy Data?

**Proxy data** is alternate data used in place of the actual data you need.

It is used when:

- actual data is not available
- actual data has not been collected yet
- there is not enough actual data
- waiting for actual data would take too long
- a similar dataset can reasonably support the analysis

---

# 2. Why Proxy Data Is Useful

Proxy data can help analysts continue working when the exact dataset is unavailable.

It can be used to:

- estimate demand
- predict outcomes
- support early analysis
- make preliminary recommendations
- answer a business question when direct data is missing

---

# 3. Proxy Data Warning

Proxy data is not the same as real data.

It should be used carefully because it may not fully match the business problem.

When using proxy data, analysts should explain:

- why proxy data was used
- how closely it matches the real data
- what limitations it creates
- how it may affect the conclusion

---

# 4. Proxy Data Example 1: New Car Model

## Business Scenario

A new car model was launched only a few days ago.

The auto dealership wants sales projections immediately and cannot wait until the end of the month for sales data.

## Proxy Data Used

The analyst uses the number of clicks on the car specifications page on the dealership’s website.

## Why This Works

Website clicks can act as a proxy for customer interest.

More clicks may suggest higher potential demand.

## Important Limitation

Clicks do not always turn into purchases.

Some users may click out of curiosity without planning to buy.

---

# 5. Proxy Data Example 2: Plant-Based Meat Product

## Business Scenario

A new plant-based meat product was recently stocked in grocery stores.

The supplier needs to estimate demand over the next four years.

## Proxy Data Used

The analyst uses sales data from a turkey substitute made out of tofu that has been on the market for several years.

## Why This Works

The tofu turkey substitute is similar enough to help estimate demand for the new plant-based product.

## Important Limitation

The new product may attract different customers, have different pricing, or follow different market trends.

---

# 6. Proxy Data Example 3: Tourism Campaign

## Business Scenario

The Chamber of Commerce wants to know how a tourism campaign will impact travel to their city.

The campaign results are not publicly available yet.

## Proxy Data Used

The analyst uses historical airline booking data from one to three months after a similar campaign ran six months earlier.

## Why This Works

Past travel behavior after a similar campaign may help predict future travel behavior.

## Important Limitation

The current campaign may differ from the earlier campaign, and travel patterns may have changed.

---

# 7. Open and Public Datasets

Analysts can also use **open datasets** or **public datasets** as proxy data sources.

These datasets are available online and can help when internal data is limited or unavailable.

Open or public datasets are useful when the analyst needs data that is:

- outside the company’s own systems
- related to a broader population
- useful for comparison
- available in a common format
- accessible for practice or analysis

---

# 8. Example: Vaccine Contraindications

## Business Scenario

A nasal version of a vaccine was recently made available.

A clinic wants to estimate possible contraindications but has only just started collecting first-party patient data.

A **contraindication** is a condition that may prevent a patient from taking a vaccine because it could harm them.

## Proxy Data Used

The analyst uses an open dataset from a trial of the injection version of the vaccine.

The analyst selects a subset of patient profiles that closely match the clinic’s patient population.

## Why This Works

The injection-version trial data may provide a useful estimate while the clinic collects its own data.

## Important Limitation

The nasal version and injection version may not have exactly the same contraindications.

---

# 9. Dataset Repositories

Online repositories can help analysts find public datasets.

One example is **Kaggle**, which provides datasets in many formats.

Kaggle datasets may be useful for:

- practicing data analysis
- finding proxy data
- exploring public data
- downloading datasets in different formats

---

# 10. Common Dataset Formats

Public datasets can come in many formats.

Common formats include:

| Format | Meaning | Notes |
|---|---|---|
| CSV | Comma-separated values | Basic table format with rows and columns |
| JSON | JavaScript Object Notation | Often used for web data and nested data |
| SQLite | Lightweight database file | Useful for structured relational data |
| BigQuery | Cloud-based data warehouse format | Useful for large public datasets |

---

# 11. CSV Datasets

**CSV** stands for comma-separated values.

CSV files store data in a table-like format.

They are commonly used because they are simple and widely supported.

## Example

A credit card customer dataset may include information such as:

- age
- salary
- marital status
- credit card limit
- credit card category

---

# 12. JSON Datasets

**JSON** is a format often used for web-based data.

It can store nested information and is common in APIs and online platforms.

## Example

A JSON dataset could contain information about trending YouTube videos.

---

# 13. SQLite Datasets

**SQLite** is a lightweight database format.

It is useful when data is structured in database tables.

## Example

A SQLite dataset could contain many years of U.S. wildfire data.

---

# 14. BigQuery Datasets

**BigQuery** is a cloud-based tool used for large datasets.

Some public datasets are available through BigQuery.

## Example

A Google Analytics 360 sample dataset from the Google Merchandise Store can be used for analysis practice.

---

# 15. Things to Check in Open Datasets

When using open datasets, analysts should check for:

- duplicate data
- null values
- missing fields
- unclear definitions
- data quality issues
- whether the dataset fits the business objective

---

# 16. Duplicate Data

**Duplicate data** means the same record appears more than once.

Duplicates can cause incorrect calculations.

## Example

If one customer appears twice, they may be counted as two different customers.

This can affect totals, averages, and trends.

---

# 17. Null Values

**Null** usually means a data field was left empty or unassigned.

However, Null can sometimes be interpreted as the value `0`.

This difference matters because blank data and zero are not always the same thing.

---

## Example

If a sales field is Null, it may mean the value is missing.

If it is interpreted as `0`, it may suggest there were no sales.

These are different meanings and could lead to different conclusions.

---

# 18. Important Rule About Null

Before analyzing a dataset with Null values, make sure you understand what Null means in that dataset.

Ask:

- Does Null mean missing?
- Does Null mean zero?
- Does Null mean not applicable?
- Should Null values be removed, replaced, or kept?

---

# 19. Common Mistakes to Avoid

## Mistake 1: Assuming proxy data is equal to real data

Proxy data is only a substitute and may not perfectly match the actual situation.

## Mistake 2: Using proxy data that is not similar enough

Proxy data should be closely related to the missing data.

## Mistake 3: Ignoring limitations

Always explain the limitations of using proxy data.

## Mistake 4: Not checking for duplicates

Duplicate records can make counts, totals, and averages inaccurate.

## Mistake 5: Misunderstanding Null values

Null may mean missing, zero, or something else depending on the dataset.

## Mistake 6: Using public data without checking fit

Open datasets may be available, but they still need to align with the business objective.

---

# 20. Proxy Data Evaluation Checklist

Before using proxy data, ask:

- Is actual data unavailable?
- Is proxy data necessary?
- Is the proxy data similar enough to the real data?
- Does the proxy data support the business objective?
- What assumptions am I making?
- What limitations should I explain?
- Are there duplicate records?
- Are there Null values?
- Is the dataset clean enough to use?
- Could this proxy data create bias?

---

# 21. Key Takeaways

- Proxy data is substitute data used when actual data is unavailable.
- Proxy data can help estimate or predict outcomes.
- Proxy data should be well-suited to the business objective.
- Proxy data must be used carefully because it may not fully match the real data.
- Open or public datasets can be used as proxy data sources.
- Kaggle is one place to find public datasets.
- Public datasets may come in formats such as CSV, JSON, SQLite, and BigQuery.
- Analysts should check open datasets for duplicate data and Null values.
- Null usually means a field is empty or unassigned, but it can sometimes be interpreted as zero.
- Analysts should explain the limitations of proxy data in their analysis.

---

# Final Summary

Proxy data is alternate data used when the actual data needed for analysis is unavailable. It can help analysts estimate sales, predict demand, or support early decision-making. For example, website clicks can proxy potential car sales, sales of a similar tofu product can proxy demand for a new plant-based meat product, and historical airline bookings can proxy the impact of a tourism campaign. Open or public datasets can also serve as proxy data sources, especially when internal data is limited. These datasets may come in formats such as CSV, JSON, SQLite, or BigQuery. However, proxy data should always be used carefully. Analysts must check whether it fits the business objective and should watch for duplicate records and Null values before analysis.
