# Working Around Missing, Insufficient, or Wrong Data

## Main Idea

When preparing for data analysis, you may discover that you do not have the data you need, do not have enough data, or have the wrong data.

In these situations, analysts need to decide whether they can:

- collect more data
- use proxy data
- adjust the analysis
- correct the data
- ignore unusable data carefully
- communicate requirements again

---

# 1. What Is Proxy Data?

**Proxy data** is substitute data used when the actual data is unavailable.

It is not the exact data you wanted, but it is similar enough to help with analysis.

A simple comparison is substituting oil for butter in a recipe when you do not have butter.

---

# 2. When Proxy Data Is Useful

Proxy data can be useful when:

- there is no actual data available
- there is too little actual data
- collecting new data would take too long
- a similar dataset can reasonably represent the missing data
- the proxy data matches the situation closely enough

---

# 3. Important Warning About Proxy Data

Proxy data is only a workaround.

It should be used carefully because it may not perfectly represent the real data.

When using proxy data, analysts should explain the limitation clearly in their analysis or report.

---

# 4. Data Issue 1: No Data

Sometimes, there is no data available for the business question.

This means the analyst cannot directly analyze the real situation.

---

## Possible Solution 1: Gather Data on a Small Scale

If there is no data, one option is to collect a small sample first.

This allows the analyst to perform a preliminary analysis.

Then the analyst can request more time to collect a larger dataset.

---

## Example

If you are surveying employees about a new performance and bonus plan, you could first survey a sample of employees.

Then you could ask for another three weeks to collect responses from all employees.

---

## Possible Solution 2: Use Proxy Data

If there is not enough time to collect new data, the most common workaround is to use proxy data from another dataset.

---

## Example

If you are analyzing peak travel times for commuters but do not have data for a particular city, you could use data from another city with a similar size and demographic.

---

# 5. Data Issue 2: Too Little Data

Sometimes, the analyst has some data, but not enough to make a strong conclusion.

This can make the analysis incomplete or less reliable.

---

## Possible Solution 1: Use Proxy Data With Actual Data

If you have too little data, you can combine the actual data with proxy data.

This can make the dataset larger and more useful.

---

## Example

If you are analyzing trends for owners of golden retrievers, you might make the dataset larger by including data from owners of labradors.

This works because labradors may be similar enough to golden retrievers for the purpose of the analysis.

---

## Possible Solution 2: Adjust the Analysis

If the available data is limited, you can adjust your analysis to match the data you already have.

This means narrowing the scope of your conclusion.

---

## Example

If you are missing data for 18- to 24-year-olds, you can still do the analysis but state this limitation:

```text
This conclusion applies to adults 25 years and older only.
```

---

# 6. Data Issue 3: Wrong Data or Data With Errors

Sometimes, the data is incorrect, contains errors, or does not match the original request.

This can happen because:

- requirements were misunderstood
- the wrong dataset was provided
- formulas are incorrect
- conditional statements are wrong
- translations are poor
- values were entered incorrectly

---

## Possible Solution 1: Communicate Requirements Again

If the wrong data was provided because the requirements were misunderstood, explain the requirements again clearly.

---

## Example

If you need data for female voters but receive data for male voters, restate your needs and request the correct dataset.

---

## Possible Solution 2: Correct Errors at the Source

If the data has errors, try to identify the pattern causing the errors.

Then, if possible, correct the issue at the source.

---

## Example

If a spreadsheet has a conditional statement or Boolean expression causing calculations to be wrong, fix the conditional statement instead of only fixing the final calculated values.

---

# 7. Why Correcting the Source Matters

Fixing only the visible results may not solve the real problem.

If the source error remains, the same mistake can happen again.

It is better to fix the formula, condition, process, or original data source causing the problem.

---

# 8. Possible Solution 3: Ignore Wrong Data Carefully

If you cannot correct the data errors yourself, you may be able to ignore the wrong data and continue the analysis.

However, this is only safe if:

- the remaining sample size is still large enough
- ignoring the data will not create systematic bias
- the removed data is not essential to the business question
- you clearly document the limitation

---

## Example

If a dataset was translated from another language and some translations do not make sense, you may ignore the badly translated data and analyze the remaining data.

But this should only be done if removing that data does not bias the results.

---

# 9. Important Warning About Data With Errors

Sometimes, data with errors is a warning sign that the entire dataset may not be reliable.

Use your best judgment before continuing.

If the errors are serious or widespread, the dataset may need to be cleaned, replaced, or recollected.

**Use the following decision tree as a reminder of how to deal with data errors or not enough data:**
<img width="943" height="674" alt="image" src="https://github.com/user-attachments/assets/f56a9d00-60f8-4dce-bbca-94720167e5d8" />


---

# 10. Summary Table: Data Issues and Solutions

| Data Issue | Possible Solution | Example |
|---|---|---|
| No data | Gather data on a small scale first | Survey a sample of employees before surveying everyone |
| No data | Use proxy data | Use commuter data from a similar city |
| Too little data | Combine actual data with proxy data | Add labrador owner data to golden retriever owner data |
| Too little data | Adjust the analysis scope | Report only on adults 25 and older |
| Wrong data | Communicate requirements again | Request female voter data instead of male voter data |
| Data with errors | Correct the issue at the source | Fix the conditional statement causing wrong calculations |
| Data with errors | Ignore bad data carefully | Remove bad translations if the remaining sample is still valid |

---

# 11. Common Mistakes to Avoid

## Mistake 1: Using proxy data without explaining it

Always make it clear when proxy data is being used.

## Mistake 2: Choosing proxy data that is not similar enough

Proxy data should be meaningfully similar to the missing data.

## Mistake 3: Making conclusions beyond the available data

If your data only supports adults 25 and older, do not make claims about all adults.

## Mistake 4: Fixing calculated values instead of the source problem

If a formula or condition is wrong, fix the formula or condition.

## Mistake 5: Ignoring bad data without checking for bias

Removing data can create systematic bias if the removed records represent a specific group.

## Mistake 6: Trusting a dataset with many errors

Many errors can be a sign that the dataset is unreliable.

---

# 12. Questions to Ask Before Continuing Analysis

Before using incomplete, proxy, or corrected data, ask:

- Do I have the data I actually need?
- Do I have enough data?
- Is proxy data reasonable for this objective?
- Is the proxy data similar enough to the missing data?
- Can I collect more data instead?
- Can I adjust the scope of the analysis?
- Are errors isolated or widespread?
- Can the errors be corrected at the source?
- Will ignoring bad data create bias?
- Have I documented the limitation?

---

# 13. Big Lesson

When data is missing, insufficient, or wrong, do not force the analysis.

Choose the best workaround based on the business objective, the available data, and the risk of bias.

---

# Key Takeaways

- Analysts may not always have the data they need.
- Proxy data can sometimes be used as a substitute for missing data.
- Proxy data should be similar enough to the real data to be useful.
- If there is no data, analysts can collect a small sample or use proxy data.
- If there is too little data, analysts can combine actual data with proxy data or adjust the scope.
- If the wrong data is provided, analysts should restate the requirements.
- If data has errors, analysts should try to correct the problem at the source.
- If errors cannot be fixed, analysts may ignore bad data only if the remaining sample is large enough and unbiased.
- Data with many errors may indicate that the dataset is unreliable.
- Any limitations should be clearly documented in the final analysis.

---

# Final Summary

This reading explains how analysts can work around missing, insufficient, or incorrect data. If there is no data, analysts can collect a small sample for preliminary analysis or use proxy data from a similar dataset. If there is too little data, analysts can combine actual data with proxy data or adjust the analysis to match the available data. If the wrong data is provided, the analyst should communicate the requirements again. If data contains errors, the analyst should try to correct the issue at the source instead of only fixing final values. In some cases, incorrect data can be ignored, but only if the sample remains large enough and unbiased. The main lesson is that analysts must carefully choose how to handle data limitations and clearly explain those limitations in their conclusions.
