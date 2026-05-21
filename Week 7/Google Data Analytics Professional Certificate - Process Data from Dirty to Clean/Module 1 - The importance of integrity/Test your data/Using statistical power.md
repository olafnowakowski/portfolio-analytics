# Statistical Power and Sample Size

## Main Idea

**Statistical power** is the probability of getting meaningful results from a test.

For Data Analysts, statistical power matters because it helps determine whether the results of a test or study are likely to be real instead of caused by random chance.

A larger and well-chosen sample size usually increases statistical power.

---

# 1. What Is Statistical Power?

**Statistical power** is the probability of getting meaningful results from a test.

In simple terms, it tells you how likely your test is to detect a real effect if that effect exists.

---

# 2. Why Statistical Power Matters

Statistical power helps analysts understand whether a test result is reliable.

If statistical power is too low, the test may fail to detect a real result.

This means the analyst could incorrectly conclude that something does not work, even when it actually does.

---

# 3. Hypothesis Testing

**Hypothesis testing** is a way to check whether a survey, experiment, or test has meaningful results.

It helps analysts determine whether the result is likely real or caused by random chance.

---

# 4. Example: Milkshake Ad Campaign

A restaurant chain wants to launch a marketing campaign for new milkshakes.

Before using the ad nationwide, the company wants to test it on a group of customers.

The analyst wants to know:

- whether customers like or dislike the campaign
- whether the ad affects milkshake orders
- whether outside factors influenced the results

---

# 5. Why Sample Size Matters in the Milkshake Example

Using all customers would be too expensive and time-consuming.

Instead, the analyst needs to choose a sample.

If the sample is too small, such as 50 customers, it may not include enough different types of people.

For example, the sample might accidentally include many people who do not like milkshakes at all.

That would make it harder to measure whether the ad itself was effective.

---

# 6. Larger Sample Size and Statistical Power

Usually, a larger sample size increases the chance of getting statistically significant results.

A larger sample helps include a wider variety of people.

This makes it easier to detect real differences between groups.

---

# 7. Statistical Significance

**Statistical significance** means the result of a test is likely real and not caused by random chance.

In simple terms, if a result is statistically significant, it is more likely to be meaningful and reliable.

---

# 8. Statistical Power as a Value

Statistical power is usually shown as a value out of 1.

Examples:

| Statistical Power | Percentage Meaning |
|---|---|
| `0.6` | 60% |
| `0.8` | 80% |
| `0.9` | 90% |

---

# 9. Example: 60% Statistical Power

If the milkshake ad test has statistical power of `0.6`, that means there is a 60% chance of getting a statistically significant result.

It also means there is a 40% chance the test result could be wrong or unreliable.

---

# 10. Common Statistical Power Standard

Usually, analysts want statistical power of at least:

```text
0.8
```

This means:

```text
80%
```

A statistical power of 80% is commonly used as a minimum target for considering test results strong enough.

---

# 11. Example: Birthday Cake Milkshake

A restaurant chain wants to test a new birthday cake flavored milkshake.

The new milkshake costs more to produce than the company’s other milkshakes.

The company hopes the new flavor will create excitement, bring in more customers, and increase sales enough to offset the extra cost.

---

# 12. Choosing Test Locations

The company wants to test the new milkshake in a few restaurant locations first.

The analyst needs to decide how many locations to include in the test.

To do this, the analyst must consider factors that could affect the results.

---

# 13. Factors That Could Affect the Test

Before choosing test locations, the analyst should ask:

- Are some restaurants running other promotions?
- Do some locations already have customers who always buy new products?
- Are any restaurants affected by construction?
- Are customer patterns different by location?
- Could another factor increase or decrease sales besides the new milkshake?

---

# 14. Why Outside Factors Matter

The analyst wants to make sure any increase in sales or customers is most likely caused by the new milkshake.

If other factors are affecting the results, the test may not accurately measure the effect of the new flavor.

---

# 15. Measurable Effects

In the birthday cake milkshake example, the measurable effects could include:

- increase in sales
- increase in number of customers
- increase in milkshake orders
- change in revenue at test locations

---

# 16. Relationship Between Sample Size and Statistical Power

| Concept | Meaning |
|---|---|
| Larger sample size | Usually increases statistical power |
| Higher statistical power | Increases the chance of detecting meaningful results |
| Low statistical power | Increases the chance of unreliable or missed results |
| Statistically significant result | Result is likely real and not due to random chance |

---

# 17. Common Mistakes to Avoid

## Mistake 1: Using a sample that is too small

A very small sample may not include enough variety to represent the full population.

## Mistake 2: Ignoring outside factors

Other promotions, location issues, or customer habits can affect test results.

## Mistake 3: Assuming results are meaningful without statistical power

A result may look useful, but low statistical power can make it unreliable.

## Mistake 4: Confusing sample size with quality

A larger sample helps, but it still needs to be chosen carefully.

## Mistake 5: Ignoring statistical significance

Analysts need to know whether results are likely real or possibly due to chance.

---

# 18. Key Takeaways

- Statistical power is the probability of getting meaningful results from a test.
- Hypothesis testing helps determine whether a survey or experiment has meaningful results.
- Larger sample sizes usually increase statistical power.
- Statistical power is shown as a value out of 1.
- A power of `0.6` means 60%.
- A power of `0.8` means 80%.
- Analysts usually want statistical power of at least 80%.
- Statistical significance means a result is likely real and not caused by random chance.
- Outside factors can affect test results.
- Analysts should choose sample sizes carefully to make results more reliable.

---

# Final Summary

Statistical power is the probability of getting meaningful results from a test. It helps Data Analysts understand whether a test is likely to detect a real effect. In the milkshake ad example, a small sample of 50 customers might not be enough because it may not include enough different types of customers. A larger sample size usually increases statistical power and improves the chance of getting statistically significant results. Statistical power is shown as a value out of 1, such as `0.6` for 60% or `0.8` for 80%. Analysts often aim for at least 80% statistical power. The main lesson is that sample size, outside factors, and statistical power all affect whether test results are meaningful and reliable.
