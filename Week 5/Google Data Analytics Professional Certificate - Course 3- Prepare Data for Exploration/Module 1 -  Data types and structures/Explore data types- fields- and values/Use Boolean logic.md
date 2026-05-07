# Boolean Logic

## Main Idea

**Boolean logic** is a system of logic that uses conditions to produce a result of either **TRUE** or **FALSE**.

Data Analysts use Boolean logic to filter results, write queries, search for information, and check conditions in programming code.

---

# What Is Boolean Logic?

Boolean logic uses logical statements to decide whether something is true or false.

A Boolean statement checks whether certain conditions are met.

Examples:

- Is the color grey?
- Is the color pink?
- Is the shoe waterproof?
- Is the value greater than 50?

The answer to each condition is usually:

- **TRUE**
- **FALSE**

---

# Boolean Operators

A **Boolean operator** is an operator used to create logical statements.

The main Boolean operators are:

- **AND**
- **OR**
- **NOT**

These operators help filter data based on one or more conditions.

---

# What Is an Operator?

An **operator** is a symbol or word that names the operation or calculation to be performed.

In Boolean logic, operators are used to connect conditions.

Examples:

- AND combines conditions
- OR allows either condition
- NOT excludes a condition

---

# Boolean Logic Example: Shoe Shopping

Imagine you are shopping for shoes.

You have different preferences:

- You will buy shoes only if they are both grey and pink.
- You will buy shoes if they are grey, pink, or both.
- You will buy grey shoes, but not if they have pink.

These preferences can be written as Boolean statements.

---

# The AND Operator

## Definition

The **AND** operator requires all conditions to be true.

If even one condition is false, the result is false.

---

## Shoe Example

You will buy the shoes only if they are both grey and pink.

Boolean statement:

IF (Color = "Grey") AND (Color = "Pink") THEN buy them

---

## Meaning

The shoes must meet both conditions:

- the shoes must be grey
- the shoes must be pink

Only shoes that are both grey and pink will be marked TRUE.

---

## AND Truth Table

| Color is Grey | Color is Pink | If Grey AND Pink, then Buy | Boolean Logic |
|---|---|---|---|
| True | True | True / Buy | True AND True = True |
| True | False | False / Do not buy | True AND False = False |
| False | True | False / Do not buy | False AND True = False |
| False | False | False / Do not buy | False AND False = False |

---

## Important Lesson

AND narrows results because all conditions must be true.

---

# The OR Operator

## Definition

The **OR** operator requires at least one condition to be true.

If either condition is true, the result is true.

---

## Shoe Example

You will buy the shoes if they are grey or pink.

Boolean statement:

IF (Color = "Grey") OR (Color = "Pink") THEN buy them

---

## Meaning

The shoes can meet either condition:

- the shoes can be grey
- the shoes can be pink
- the shoes can be both grey and pink

Any of these results will be marked TRUE.

---

## OR Truth Table

| Color is Grey | Color is Pink | If Grey OR Pink, then Buy | Boolean Logic |
|---|---|---|---|
| False | False | False / Do not buy | False OR False = False |
| False | True | True / Buy | False OR True = True |
| True | False | True / Buy | True OR False = True |
| True | True | True / Buy | True OR True = True |

---

## Important Lesson

OR expands results because only one condition needs to be true.

---

# The NOT Operator

## Definition

The **NOT** operator excludes a condition.

It reverses the truth value of a condition.

- NOT TRUE becomes FALSE
- NOT FALSE becomes TRUE

---

## Shoe Example

You will buy grey shoes, but not if they include pink.

Boolean statement:

IF (Color = "Grey") AND (Color = NOT "Pink") THEN buy them

---

## Meaning

The shoes must be grey, but they must not be pink.

Shoes with pink are excluded.

---

## NOT Truth Table

| Color is Grey | Color is Pink | Boolean Logic for NOT Pink | If Grey AND NOT Pink, then Buy | Boolean Logic |
|---|---|---|---|---|
| True | False | NOT False = True | True / Buy | True AND True = True |
| True | False | NOT False = True | True / Buy | True AND True = True |
| True | False | NOT False = True | True / Buy | True AND True = True |
| True | True | NOT True = False | False / Do not buy | True AND False = False |

---

## Important Lesson

NOT removes specific results from your data.

---

# AND vs OR vs NOT

| Operator | Meaning | Result |
|---|---|---|
| **AND** | All conditions must be true | Narrows results |
| **OR** | At least one condition must be true | Expands results |
| **NOT** | Excludes a condition | Removes results |

---

# Multiple Conditions

The real power of Boolean logic comes from combining multiple conditions in one statement.

This lets Data Analysts create more specific filters.

---

## Example

You want shoes that are grey or pink, and also waterproof.

Boolean statement:

IF ((Color = "Grey") OR (Color = "Pink")) AND (Waterproof = "True") THEN buy them

---

# Parentheses in Boolean Statements

Parentheses are used to group conditions together.

They help control the order of logic.

In this example:

IF ((Color = "Grey") OR (Color = "Pink")) AND (Waterproof = "True")

The grouped condition is:

(Color = "Grey") OR (Color = "Pink")

This means the shoe must be grey or pink first.

Then it must also be waterproof.

---

# Why Parentheses Matter

Without parentheses, a Boolean statement may be interpreted incorrectly.

Parentheses make the logic clearer and more precise.

### Important Lesson

Use parentheses when combining multiple Boolean conditions.

---

# Boolean Logic in Data Analysis

Data Analysts use Boolean logic for many tasks, including:

- filtering data
- writing search queries
- checking conditions
- creating spreadsheet formulas
- writing programming code
- querying databases
- narrowing search results
- excluding unwanted results

---

# Boolean Logic in Queries

In queries, Boolean logic helps filter results based on conditions.

Example:

Find customers who live in California and purchased a product last month.

Boolean logic:

State = "California" AND Purchase_Date = "Last Month"

---

# Boolean Logic in Searches

Boolean operators can also improve searches.

Examples:

- data analyst AND SQL
- marketing OR advertising
- customer data NOT test data

These searches help include or exclude specific results.

---

# Boolean Logic in Programming

In programming, Boolean logic is often used in conditional statements.

Example:

IF score >= 80 AND attendance = "Complete" THEN pass

This checks whether both conditions are true.

---

# Big Lesson

Boolean logic helps Data Analysts create clear conditions that filter information and return only the results that match the logic.

---

# Key Takeaways

- Boolean logic uses conditions that evaluate to TRUE or FALSE.
- Boolean operators include AND, OR, and NOT.
- AND requires all conditions to be true.
- OR requires at least one condition to be true.
- NOT excludes a condition.
- Boolean operators can be used to filter results.
- Boolean statements are useful in searches, queries, spreadsheets, and programming.
- Parentheses help group conditions and control the logic.
- Multiple conditions allow more specific filtering.
- Data Analysts use Boolean logic to analyze data more efficiently.

---

# Extra Important Notes

- AND narrows your results.
- OR expands your results.
- NOT removes unwanted results.
- Boolean logic is useful when working with large datasets.
- Boolean statements help make filtering more precise.
- Boolean conditions can be combined to create complex queries.
- A Boolean statement should be written clearly so the logic is easy to understand.

---

# Final Summary

This reading introduces Boolean logic and Boolean operators. Boolean logic uses conditions that return TRUE or FALSE. The main Boolean operators are AND, OR, and NOT. AND requires all conditions to be true, OR requires at least one condition to be true, and NOT excludes a condition. Data Analysts use Boolean logic to filter data, write queries, search for information, and check conditions in code. Boolean statements can also combine multiple conditions using parentheses, which makes filtering more precise. The main lesson is that Boolean logic helps analysts create clear, logical filters to find exactly the data they need.
