# Amazon’s Dynamic Revenue Metrics: Co-Occurrence Data and Recommendations

## Main Idea

This lesson continues the Amazon example and explains how Amazon uses detailed data about customer behavior to increase sales.

Amazon does not only track what users search for. It also tracks:

- what books people buy together
- what books people view but do not buy
- what books are bought after viewing another book
- which recommendations increase sales the most

This helps Amazon personalize the shopping experience and choose which products to recommend.

---

## What We Already Know About Amazon’s Database

From the previous lesson, we know Amazon likely stores several important pieces of information for every book.

For every unique **Book ID**, Amazon stores:

- the book’s unique database record
- the subject area categories the book belongs to
- the subcategories and subtopics the book belongs to
- how the book ranks in recent sales within each category and subcategory
- how relevant the book is to a user’s search

This allows Amazon to quickly decide which books to show when someone searches.

---

## Example Book: David MacKay Textbook

In the example, the top book Amazon shows from the search results is:

**Information Theory, Inference, and Learning Algorithms** by **David MacKay**

This book appears as the top result out of more than **1,200 possible books** Amazon retrieved.

The speaker mentions that this is one of their favorite books and is used in a Duke Master of Engineering Management Data Mining course.

---

## Clicking on the Book Page

When the user clicks on the MacKay book, Amazon shows a new page with more information.

One important section on this page is:

**Frequently Bought Together**

This section suggests another book:

**Elements of Information Theory** by **Cover and Thomas**

---

## Frequently Bought Together

## What it means

The **Frequently Bought Together** section recommends products that customers often buy together in the same shopping session.

In this case, Amazon suggests that people who buy the MacKay book may also want to buy the Cover and Thomas book.

## Subtle selling suggestion

Amazon is indirectly suggesting that learning information theory in relation to machine learning may require more than one book.

This is a sales technique because it encourages the customer to buy more than one item.

---

## No Discount Offered

The speaker notices that Amazon does **not** offer a discount for buying both books together.

This is important because it suggests Amazon has probably tested this.

Amazon may have found that offering a discount does not increase sales enough to justify the lower price.

### Important lesson

Amazon likely uses data to decide not only what to recommend, but also whether discounts are worth offering.

---

## Co-Occurrence Data

## What is co-occurrence data?

**Co-occurrence data** tracks things that happen together.

In Amazon’s case, this means tracking books that are:

- bought together in the same session
- viewed together in the same session
- viewed before another book is purchased

## Example

If many customers buy the MacKay book and the Cover and Thomas book together, Amazon records that these two books frequently co-occur in purchases.

---

## Co-Occurrence Matrix

Co-occurrence data can be represented in a **co-occurrence matrix**.

A co-occurrence matrix shows relationships between items based on how often they appear together.

For Amazon, this could mean a matrix that tracks:

- Book A bought with Book B
- Book A viewed with Book B
- Book A viewed before Book B was bought

The speaker says this topic will be explored more later.

---

## Amazon Tracks More Than Purchases

Amazon is not only tracking what people buy.

It also tracks what users click on and view while browsing.

This means Amazon keeps detailed clickstream data about:

- books people looked at
- books people did not buy
- books people bought after looking at other books

### Important lesson

Amazon learns from both purchases and non-purchases.

Even when a user does not buy something, that behavior still provides useful data.

---

## Top 100 Frequently Bought Together Books

Amazon offers viewers a list of the top **100 books** that people frequently bought at the same time as the MacKay book.

This means Amazon is maintaining an up-to-date database of:

- each book
- other books purchased in the same session
- how often those purchases happen together

---

## Question About Ranking

The speaker raises an important question:

Does Amazon list the top 100 co-occurring books in exact order from highest co-occurrence to lowest?

The speaker does not know the answer.

This matters because the book shown in the **Frequently Bought Together** slot may not necessarily be the single most frequently purchased book with MacKay.

---

## Possible Explanation 1: Simple Co-Occurrence Ranking

One possibility is that Amazon ranks books simply by how often they are bought together.

If that is true, then the book most frequently bought with MacKay might actually be:

**Pattern Recognition and Machine Learning** by **Christopher Bishop**

This would mean Cover and Thomas is not necessarily the most frequently bought together book, even though Amazon suggests it in the main recommendation slot.

---

## Possible Explanation 2: A/B Testing for Best Upsell

Another possibility is that Amazon uses **A/B testing** to decide which book to place in the main **Frequently Bought Together** recommendation.

Amazon may have tested different recommendations and found that showing Cover and Thomas with MacKay increases:

- sales
- profits
- total order value

more than showing Bishop or other books.

In this case, Amazon is not simply choosing the book with the highest co-occurrence. It is choosing the book with the best **upsell revenue potential**.

---

## What Is Upsell Revenue Potential?

**Upsell revenue potential** means the chance that recommending an additional product will increase the value of the sale.

Amazon wants to know:

- which recommendation makes customers more likely to buy more
- which recommendation increases profit the most
- which product placement works best

### Important lesson

The best recommendation is not always the most obvious one. It is the one that creates the best business result.

---

## Possible Explanation 3: Avoid Showing the Same Offer Again

Another possibility is that Amazon already showed the user Cover and Thomas in the main **Frequently Bought Together** area.

If the user did not accept that offer, Amazon may slightly change the order of the top 100 list.

Amazon might then show the second-most popular related book first in another section to avoid repeating the same offer.

### Important lesson

Amazon may adjust recommendations based on what it already showed the user and how the user responded.

---

## Amazon Optimizes Recommendation Placement

The speaker concludes that the exact ranking is uncertain, but one thing is likely:

Amazon optimizes the placement of recommendations through A/B testing.

This includes:

- the Frequently Bought Together display
- the top 100 frequently bought together display
- the order of recommendations
- which products appear in the most visible slots

The goal is to maximize sales and profits.

---

## Viewed But Not Bought Data

Amazon also tracks books that users viewed but did not buy.

This is another important type of clickstream data.

At the bottom of the MacKay book page, Amazon shows another list based on:

- people who viewed the MacKay book
- did not buy it
- but bought other books during the same session

This shows that Amazon tracks what customers buy after considering but rejecting a product.

---

## Why Viewed-But-Not-Bought Data Matters

This type of data helps Amazon understand alternatives.

If many users view Book A but then buy Book B, Amazon can infer that:

- Book B may be a better match for some users
- Book B may be more appealing
- Book A may attract attention but not always close the sale
- Book B may be a strong recommendation for users who hesitate on Book A

### Important lesson

A product a customer does not buy can still tell Amazon what the customer might want instead.

---

## Amazon’s Co-Occurrence Matrix

The speaker explains that Amazon likely maintains a co-occurrence matrix for every visit that results in at least one book sale.

This matrix includes at least two major types of records.

---

## Record Type 1: Books Bought Together

When **Book 1** is bought, Amazon records:

- all other books bought in the same session
- how often those books are bought together
- the relationship between the purchased books

This supports the **Frequently Bought Together** feature.

---

## Record Type 2: Books Viewed Before Purchase

When **Book 1** is bought, Amazon also records:

- all other books viewed during that same session
- books the user looked at but did not buy
- what the user ultimately purchased instead

This supports recommendation lists based on browsing behavior.

---

## Amazon’s Three Recommendation Metrics

The lesson identifies three important recommendation metrics Amazon uses.

---

## 1. Profit-Maximizing Frequently Bought Together Metric

Amazon’s first line of promotion is the **Frequently Bought Together** recommendation.

This is likely optimized to maximize profit, not just show the most common pairing.

It answers the question:

**Which additional product should we recommend with this book to increase sales or profit the most?**

---

## 2. Recommendation Based on Products Bought Together

The second metric recommends books that are likely to be bought if the user buys the first book.

It is based on the assumption:

**If this user buys the MacKay book, what else are they likely to buy?**

This supports recommendations based on completed purchases.

---

## 3. Recommendation Based on Viewed But Not Bought Behavior

The third metric recommends books based on what people bought after viewing but not buying the first book.

It answers the question:

**What did people buy after looking at this book but choosing not to buy it?**

This helps Amazon recommend alternatives.

---

## Why This Is Important for Dynamic Revenue Metrics

Amazon uses these metrics dynamically because the recommendations can change based on:

- current user behavior
- past buying behavior
- what similar users bought
- what users viewed but rejected
- A/B testing results
- current sales performance

This allows Amazon to improve sales during the user’s current visit.

---

## Big Lesson

Amazon’s recommendation system is not random.

It is based on detailed tracking of:

- product relationships
- customer sessions
- browsing behavior
- purchase behavior
- co-occurrence patterns
- testing results

Amazon uses this data to decide what to show customers in order to increase the chance of a sale.

---

## Key Takeaways

- Amazon tracks dynamic revenue metrics for every book.
- Each book has a unique Book ID and belongs to subject categories and subcategories.
- Amazon tracks how books rank in sales within their subject areas.
- Amazon tracks which books are bought together.
- Amazon tracks which books are viewed but not bought.
- Co-occurrence data shows which products appear together in customer behavior.
- Co-occurrence data can be stored in a co-occurrence matrix.
- The Frequently Bought Together feature is based on co-occurring purchase behavior.
- Amazon may use A/B testing to decide which product recommendation creates the most sales or profit.
- Amazon also recommends products based on what people bought after viewing but not buying a specific product.
- Viewed-but-not-bought data is valuable because it reveals customer alternatives.
- Amazon’s recommendations are designed to maximize sales and profits.

---

## Extra Important Notes

- A recommendation does not have to be the most frequently co-occurring product to be the most profitable recommendation.
- A/B testing helps Amazon determine which recommendation placement works best.
- Amazon learns from both successful purchases and abandoned product views.
- Product recommendation systems are a major example of dynamic revenue optimization.
- Any business with an online store or website can learn from this approach by tracking what users view, click, ignore, and buy.

---

## Final Summary

This lesson explains how Amazon uses co-occurrence data and clickstream behavior to create powerful dynamic revenue metrics. Amazon tracks not only which books people buy together, but also which books they view without buying and what they purchase afterward. This information can be organized in a co-occurrence matrix and used to power recommendation systems like Frequently Bought Together. Amazon likely uses A/B testing to decide which recommendations and placements increase sales or profits the most. The key lesson is that Amazon’s personalized recommendations are based on detailed data about customer behavior, and this data helps the company optimize revenue during each customer visit.
