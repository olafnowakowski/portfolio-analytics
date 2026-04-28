# Case Study: Northwind Traders and the 5 Whys Technique

## Main Topic

This lesson shows how to use **Root Cause Analysis (RCA)** and the **5 Whys technique** to investigate a business problem.

The business problem is a sudden decline in online sales for a retail company called **Northwind Traders**.

---

# Scenario Overview

Northwind Traders is a successful retail company with a strong online store.

Recently, the company noticed a serious problem:

- online sales dropped sharply
- the decline happened across all product categories
- both new customers and returning customers were affected

The leadership team decides to use **Root Cause Analysis** to find the real reason behind the decline instead of guessing.

---

# Step 1: Define the Problem Clearly

## Weak Problem Statement

The original problem statement was:

**Declining sales**

This is too vague because it does not explain:

- what kind of sales declined
- when the decline happened
- how large the decline was
- which customers or products were affected

---

## Better Problem Statement

A stronger problem statement is:

**The online sales of Northwind Traders have experienced a 20% decline in revenue from online sales in the past quarter. The decline appears across multiple product categories, affecting new and returning customers.**

---

## Why This Is Better

This problem statement is stronger because it is:

- **specific**
- **measurable**
- **time-bound**
- connected to a clear business metric

It explains:

- the sales channel: online sales
- the size of the decline: 20%
- the time period: past quarter
- the scope: multiple product categories
- the customers affected: new and returning customers

---

# Given Data

## Revenue from Online Sales

| Product | Quarter 1 | Quarter 2 |
|---|---:|---:|
| Product A | 1,200,000 | 950,000 |
| Product B | 800,000 | 650,000 |
| **Total Revenue** | **2,000,000** | **1,600,000** |

Revenue drop:

- 2,000,000 to 1,600,000
- total decline = **20%**

---

## Website Traffic

| Visitor Type | Quarter 1 | Quarter 2 |
|---|---:|---:|
| New visitors | 200,000 | 300,000 |
| Returning visitors | 300,000 | 236,470 |
| **Total website visits** | **500,000** | **536,470** |

Important observation:

- website traffic increased
- revenue decreased

This means the problem is probably not simply fewer visitors.

---

# Step 2: Apply the 5 Whys Technique

## What Is the 5 Whys Technique?

The **5 Whys technique** is a simple root cause analysis method.

It works by repeatedly asking:

**Why?**

The goal is to move past symptoms and uncover the real root cause.

---

# Five Whys Analysis: Northwind Traders

## Why 1

### Question

**Why did online sales revenue decline by 20% in the past quarter?**

### Answer

Because the conversion rate on the e-commerce platform dropped from **4.5% to 3.4%**.

---

## Conversion Metrics

| Metric | Q1 | Q2 |
|---|---:|---:|
| Total number of sales | 22,500 | 18,240 |
| Average order value | 88.9 | 87.7 |
| Conversion rate | 4.5% | 3.4% |

---

## Important Lesson

The conversion rate decline explains why revenue dropped, but it is not the root cause.

It is still a symptom.

The next question should be:

**Why did the conversion rate decrease from 4.5% to 3.4%?**

---

# Why 2

## Question

**Why did the conversion rate decrease from 4.5% to 3.4%?**

## Answer

Because more visitors left the site without making a purchase.

The bounce rate increased.

---

## Bounce Rate Data

| Metric | Quarter 1 | Quarter 2 |
|---|---:|---:|
| Average time spent on website | 5 | 3 |
| Bounce rate | 20% | 45% |

The bounce rate increased from:

- 20% to 45%

This means many more visitors abandoned the site without buying.

---

## Important Lesson

The higher bounce rate is also a symptom, not the root cause.

The next question should be:

**Why did 25% more visitors abandon the site without making a purchase?**

---

# Why 3

## Question

**Why did 25% more visitors abandon the site without making a purchase?**

## Answer

Because users abandoned their carts at a higher rate due to a longer and more complex checkout process.

---

## Important Lesson

A longer and more complex checkout process is closer to the problem, but it is still not the deepest cause.

The next question should be:

**Why did the checkout process become longer and more complex?**

---

# Why 4

## Question

**Why did the checkout process become longer and more complex?**

## Answer

Because implementing a new payment gateway created technical issues that slowed down the payment processing steps.

The issue was intermittent, so it was missed during testing.

---

# Root Cause

The root cause of the 20% drop in online sales was:

**A technical fault with the new payment gateway implementation.**

This technical problem slowed down the checkout process, causing more customers to abandon their carts.

---

# Full Cause-and-Effect Chain

1. Online sales revenue dropped by 20%.
2. Revenue dropped because the conversion rate fell from 4.5% to 3.4%.
3. The conversion rate fell because more visitors abandoned the site without purchasing.
4. Visitors abandoned the site because the checkout process became longer and more complex.
5. The checkout process became worse because the new payment gateway had technical issues.
6. The technical issue was missed during testing because it was intermittent.

---

# Possible Additional Issue

The payment gateway technical fault appears to be the main root cause.

However, the team also uncovered another possible problem:

**The testing process may not have been strong enough.**

Because the issue was intermittent, it was not caught before launch.

The team should investigate whether:

- testing covered enough scenarios
- intermittent problems were tested properly
- payment gateway testing was realistic
- quality assurance processes need improvement

---

# Recommended Next Steps

## Immediate Action

Fix the technical issue with the payment gateway.

## Follow-Up Action

Check whether online sales return to normal after the fix.

Important metrics to monitor:

- conversion rate
- bounce rate
- cart abandonment rate
- average time spent on website
- number of completed sales
- revenue from online sales
- new customer purchases
- returning customer purchases

## Additional Investigation

Review the testing process to understand why the issue was missed.

---

# Important Lessons from the Case Study

## Do Not Stop Too Early

A major mistake in the 5 Whys technique is stopping too soon.

For example, stopping at “conversion rate dropped” would not solve the real problem.

The conversion rate drop was only a symptom.

---

## Symptoms vs Root Cause

| Symptom | Deeper Cause |
|---|---|
| Revenue dropped | Conversion rate decreased |
| Conversion rate decreased | Bounce rate increased |
| Bounce rate increased | More cart abandonment |
| Cart abandonment increased | Checkout process became longer |
| Checkout became longer | Payment gateway had technical issues |

---

## The Root Cause May Not Be Obvious

At first, the company only saw declining sales.

But the real problem was hidden inside the checkout and payment process.

This shows why analysts need to keep asking questions.

---

# Benefits of the 5 Whys Technique

The 5 Whys technique helps business analysts:

- go beyond surface-level symptoms
- challenge assumptions
- avoid guessing
- uncover hidden causes
- find practical solutions
- understand the chain of events behind a problem

---

# Pitfalls to Avoid

When using the 5 Whys technique, avoid:

- stopping too early
- accepting surface-level answers
- blaming people instead of analyzing processes
- asking questions without evidence
- ignoring data
- using only one perspective
- failing to involve the right experts

---

# Important Reminder

Even though it is called the **5 Whys**, you do not always need exactly five questions.

You may need:

- fewer than five questions
- exactly five questions
- more than five questions

You stop when you reach the most probable root cause.

---

# Key Takeaways

- The problem statement should be specific, measurable, and time-bound.
- “Declining sales” is too vague to begin solving the problem.
- Northwind Traders had a 20% decline in online revenue in the past quarter.
- Website traffic increased, so the problem was not fewer visitors.
- Revenue dropped because the conversion rate decreased.
- The conversion rate decreased because the bounce rate increased.
- Bounce rate increased because more users abandoned their carts.
- Users abandoned carts because the checkout process became longer and more complex.
- The checkout process became worse because of a technical issue with the new payment gateway.
- The technical issue was missed during testing because it was intermittent.
- The root cause was a technical fault with the payment gateway implementation.
- A possible additional issue is a weakness in the testing process.
- The 5 Whys technique helps uncover the root cause by repeatedly asking why.

---

# Final Summary

In the Northwind Traders case study, the company first described its problem as “declining sales,” but this was too vague. A better problem statement identified a 20% decline in online sales revenue during the past quarter across multiple product categories and customer types. Using the 5 Whys technique, the team discovered that the decline was caused by a lower conversion rate, which was caused by a higher bounce rate, which was caused by increased cart abandonment, which was caused by a longer and more complex checkout process. The root cause was a technical fault with the new payment gateway implementation. The team also identified a possible weakness in the testing process because the issue was missed before launch. The main lesson is that business analysts should keep asking why until they move past symptoms and uncover the real cause of the problem.
