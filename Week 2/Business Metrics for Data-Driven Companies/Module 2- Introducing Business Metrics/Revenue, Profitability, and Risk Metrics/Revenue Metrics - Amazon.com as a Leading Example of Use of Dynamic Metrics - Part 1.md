# Dynamic Revenue Metrics and Amazon’s Online Sales Process

## Main Idea

This lesson compares two extremes on the sales continuum:

1. **Enterprise sales**
   - Depends on one-on-one meetings between salespeople and potential customers.
   - Uses more traditional revenue metrics.

2. **Online retail**
   - Customers buy products without interacting with a human salesperson.
   - Uses dynamic revenue metrics and real-time customization.

Amazon is used as the main example of a company that uses dynamic revenue metrics very effectively.

---

## Enterprise Sales vs Online Retail

### Enterprise Sales

Enterprise sales usually involve:

- personal meetings
- direct salespeople
- relationship-building
- phone calls
- in-person visits
- long sales processes

This is one extreme of the sales process.

### Online Retail

Online retail is the opposite extreme.

In online retail:

- customers interact with a website or mobile app
- no salesperson is usually involved
- the website itself manages the sales experience
- the customer journey is shaped by data

### Important Lesson

Successful online retailers make the experience feel personal and helpful, even though it is handled by a computer system.

---

## Amazon as a Best-Practice Example

Amazon is presented as a company that does an excellent job of defining and using **dynamic revenue metrics**.

Amazon manages the customer experience by studying user behavior and changing the experience in real time.

Even if a company is not in retail, Amazon’s methods are still useful because any business with a website can learn from how Amazon studies website behavior.

---

## Clickstream Data

### What Is Clickstream Data?

**Clickstream data** is the pattern of a user’s activity on a website.

It can include:

- clicks
- cursor movements
- movement from page to page
- search terms
- browsing behavior
- what the user views
- what the user ignores

### Why Clickstream Data Matters

Clickstream data helps a company understand what users are doing online.

This allows the company to improve the website experience and increase the chance that users will buy something.

---

## Amazon’s Real-Time Customization

### What Real-Time Customization Means

**Real-time customization** means changing a user’s experience while they are currently using the website.

Amazon can customize the experience based on:

- the user’s current search
- the user’s clickstream data
- the user’s historical behavior
- what similar visitors did in the past

### Important Lesson

Real-time customization is one of the strongest examples of making a business process change **right now**.

Amazon does not wait until later to adjust the experience. It responds immediately during the user’s session.

---

## Amazon’s System Design

Amazon’s system combines two major types of data:

### 1. Pre-Processed Data

This is data Amazon has already prepared before the user searches.

Examples include:

- product databases
- book records
- text indexes
- subject categories
- customer history
- historical buying behavior

### 2. Real-Time Data

This is data created while the user is actively using Amazon.

Examples include:

- search terms
- clicks
- page movements
- current browsing behavior

### Big Idea

Amazon combines prepared historical data with live user behavior to decide what to show each customer.

---

## Example: Amazon Book Search

The speaker gives an example of searching Amazon Books using the words:

**information theory learning**

In less than three seconds, Amazon shows a page with **12 books**.

The important question is:

**How did Amazon decide which 12 books to show first?**

---

## Amazon’s Book ID Database

Amazon has a very large book database.

Each book has:

- its own record
- a unique Book ID
- a specific location in the database

This makes it possible for Amazon to quickly retrieve and organize book information.

---

## Amazon’s Text Index

Amazon also maintains a text index.

A **text index** allows Amazon to search book records for specific words.

Amazon may index words from:

- book titles
- other text connected to the book
- possibly text inside the book

For the search **information theory learning**, Amazon finds more than **1,200 books** that contain at least one of those words.

---

## Why Random Search Results Would Be Bad

Amazon could randomly select 12 books from the 1,200 possible matches.

But this would likely show books that are not relevant.

If the results are not useful, the user might:

- look at one or two pages
- get frustrated
- stop browsing
- leave without buying anything

The speaker compares this to poor internet search from around 1995.

### Important Lesson

Bad search results lose sales.

---

## Amazon’s Dynamic Revenue Metrics

Instead of showing random books, Amazon ranks the results.

Amazon ranks books by predicted relevance to the user.

In simple terms, Amazon is trying to predict:

**Which books is this user most likely to buy during this visit?**

This is a dynamic revenue metric because it connects the search results directly to the probability of a purchase.

---

## Amazon’s Inferred Two-Step Ranking Process

The speaker says they do not have direct inside knowledge of Amazon’s system, but they infer that Amazon uses a two-step process.

---

## Step 1: Match Search Terms to Subject Categories

Amazon first studies the search phrase:

**information theory learning**

Then Amazon matches it to a predefined list of subject categories.

These subject categories are similar to the subject index used in old library card catalogs.

---

## Controlled Vocabulary Index

### What It Means

A **controlled vocabulary index** is a limited and organized list of subject terms.

It does not contain every possible word users might type.

Instead, it contains standardized subject categories.

### Why It Matters

People often do not know exactly how to describe what they want.

A controlled vocabulary index helps Amazon connect the user’s search words to broader subject areas.

---

## Synonym Matching

Amazon likely uses a large thesaurus to match the user’s search words to related subject categories.

This means Amazon does not only look for exact word matches.

It also looks for related meanings.

### Why This Is Useful

Synonym matching helps Amazon give users what they actually want, even if they did not know the exact terms to search for.

### Example

The user searches:

**information theory learning**

Amazon may connect this search to subject areas such as:

- artificial intelligence
- machine learning
- computer vision
- pattern recognition
- neural networks
- semantics

Even if some of those words were not included in the original query.

---

## Evidence of Synonym Matching

The speaker notices that Amazon shows subject areas in the upper-left corner of the first search results page.

These subject areas include the number of books in Amazon’s catalog that are listed under each subject.

The speaker points out that all ten subject areas are relevant, but only three of them contain even one of the original words typed into the search.

### Important Lesson

This suggests Amazon is not only matching exact words. It is matching the meaning of the search to related subject areas.

---

## Category Trees and Subcategories

Amazon’s subject index expands into subtopics.

For example, if the user clicks on **AI and Machine Learning**, Amazon may show subtopics such as:

- AI and machine learning
- computer vision
- pattern recognition
- intelligence and semantics
- neural networks
- machine theory

This creates a tree structure of:

- categories
- subcategories
- more specific topics

---

## Step 2: Identify Best-Selling Books Within Relevant Subcategories

After Amazon identifies the subject categories most relevant to the user’s search, it then looks for the best-selling books inside those subject subcategories.

Amazon defines best sellers based on how well books are selling compared only to other books in the same subject area or subcategory.

### Why This Matters

A specialized book may not be a top seller across all of Amazon, but it may be a top seller in its specific subject area.

That makes it more relevant to someone searching for that topic.

---

## Why Amazon Needs Subject Categories

If Amazon simply ranked all 1,200 matching books by total sales, general-interest best sellers would dominate the results.

This would hide specialized books that may be exactly what the user wants.

### Example

A specialized machine learning book may only interest a smaller group of people, but it could be highly relevant to the user’s search.

Without subject categories, that book might be buried under more general best sellers.

---

## Amazon’s Dynamic Top-Line Metrics

The speaker infers that Amazon is using these dynamic top-line metrics:

1. **Which subject area categories in the controlled vocabulary index are most relevant to this user’s exact typed query terms?**

2. **Within the subject subcategories that best match the query, which books are selling the most right now?**

These metrics help Amazon decide which books to display first.

---

## Why This Is a Dynamic Revenue Metric

Amazon’s search and ranking system is dynamic because it:

- responds immediately to the user’s current search
- uses real-time clickstream data
- uses historical customer behavior
- uses behavior from similar users
- ranks products based on predicted purchase probability
- changes the user experience during the session

### Important Lesson

Amazon’s system is designed to increase revenue by making the shopping experience more relevant in real time.

---

## Big Lesson

Amazon does not just wait for users to browse randomly.

It actively uses data to decide:

- what the user probably means
- what categories are most relevant
- what products are most likely to sell
- what should be displayed first

This creates a more effective online sales process.

---

## Key Takeaways

- Enterprise sales depend on personal meetings and one-on-one communication.
- Online retail depends on digital interfaces and data-driven customer experiences.
- Amazon is a strong example of dynamic revenue metrics.
- Clickstream data includes clicks, cursor movements, page movements, and search behavior.
- Amazon combines historical data with real-time user behavior.
- Real-time customization changes the customer experience while the user is still on the site.
- Amazon likely uses subject categories and synonym matching to understand what users really want.
- A controlled vocabulary index organizes products into standardized subject categories.
- Amazon does not only match exact words; it likely matches meaning and intent.
- Amazon ranks products based on predicted relevance and purchase probability.
- Best-seller rankings are more useful when calculated within relevant subcategories.
- Dynamic revenue metrics help online retailers improve customer experience and increase sales immediately.

---

## Extra Important Notes

- A user’s search terms may not perfectly describe what they actually want.
- Exact keyword matching is weaker than intent-based or category-based matching.
- Product ranking is a major business process in online retail.
- A well-designed search result page can directly affect revenue.
- Businesses outside retail can still learn from Amazon by studying website behavior and improving online user experience.

---

## Final Summary

This lesson explains how online retail uses dynamic revenue metrics differently from traditional enterprise sales. Enterprise sales depend on personal meetings and salespeople, while online retailers like Amazon use data and real-time customization to guide customers toward purchases. Amazon studies clickstream data, search terms, historical behavior, and product categories to decide what to show each user. In the book search example, Amazon likely uses a controlled vocabulary index, synonym matching, and best-seller rankings within relevant subject categories to display the books the user is most likely to buy. The main lesson is that dynamic revenue metrics help companies make immediate process changes that improve customer experience and increase sales.
