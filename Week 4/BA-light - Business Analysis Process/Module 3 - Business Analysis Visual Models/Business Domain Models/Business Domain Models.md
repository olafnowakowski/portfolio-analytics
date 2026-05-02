# Business Domain Models: Classes, Associations, and Attributes

## Main Idea

A **business domain model** is a visual model that shows how different parts of a business relate to each other.

It helps a Business Analyst understand the high-level structure of the business before going deeper into specific processes.

---

# What Is a Business Domain Model?

A **business domain model** shows the relationships between important business elements.

These elements might include:

- customers
- orders
- products
- marketing
- fulfillment
- payments
- suppliers
- software actions
- business systems

The goal is to show how these elements connect.

---

# Business Domain Model vs Process Flow Diagram

## Process Flow Diagram

A **process flow diagram** shows the step-by-step flow of a specific process.

It explains:

- what happens first
- what happens next
- where decisions happen
- how the process ends

### Example

A process flow diagram might show how a customer places an order from start to finish.

---

## Business Domain Model

A **business domain model** shows how business elements relate to each other.

It does not have to show one specific process from start to finish.

### Example

A business domain model might show that:

- a customer places an order
- an order includes products
- products are connected to customers through orders

---

# Simple Comparison

| Model | What It Shows | Main Purpose |
|---|---|---|
| **Process Flow Diagram** | Step-by-step actions in a process | Shows how a process is carried out |
| **Business Domain Model** | Relationships between business elements | Shows how parts of the business connect |

---

# Classes

## What Are Classes?

In a business domain model, the main parts of the business are called **classes**.

A class is an important business object, concept, or category.

Examples of classes:

- Customer
- Order
- Product

---

## Classes in Boxes

Classes are usually shown inside boxes.

The class name appears at the top of the box.

At first, the box may only contain the class name.

Later, as the model becomes more detailed, the box can be filled with more information.

---

# Example Classes: Customer, Order, and Product
<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/e8b8d701-895b-448c-8379-cc461ee0bf2f" />

For a company that sells physical products, a simple business domain model might start with three classes:

1. **Customer**
2. **Order**
3. **Product**

These three classes form the basic structure of many customer ordering systems.

---

## Customer

A **Customer** is the person or organization that buys from the company.

Possible customer information may include:

- customer ID
- name
- email address
- phone number
- shipping address
- billing address

---

## Order

An **Order** represents a purchase made by a customer.

Possible order information may include:

- order number
- order date
- order status
- payment status
- shipping status
- total price

---

## Product

A **Product** is something the company sells.

Possible product information may include:

- product ID
- product name
- product description
- price
- inventory quantity
- product category

---

# Associations

## What Are Associations?

**Associations** show how classes are connected to each other.

After identifying the classes, the analyst determines how those classes relate.

In a domain model, associations are often shown with lines connecting the class boxes.

---

## Example Association
<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/63c90f0b-47c4-4594-a833-77ecca48c4c9" />

In a customer ordering system:

- a customer places an order
- an order includes a product
- the customer receives the product

This means the **Order** connects the **Customer** and the **Product**.

---

# Customer, Order, and Product Relationship

The relationship can be understood like this:

1. A **Customer** places an **Order**.
2. The **Order** contains one or more **Products**.
3. The **Customer** receives the **Product**.

### Important Lesson

The connection between the customer and the product is often the order.

---

# Associations May Not Always Have Direction

Associations do not always have a strict direction like a process flow diagram.

A process flow diagram usually shows a sequence:

- first this happens
- then this happens
- then this happens

A domain model shows relationships, even if they are not always linear.

---

## Example: Order and Product

A customer order may trigger a product shipment.

That is directional because the order causes the shipment.

However, after shipment, the order and product remain connected.

For example:

- if the customer returns the product
- if the product arrives damaged
- if the business needs to replace the item

The company can use the order number to locate the product and handle the issue.

### Important Lesson

A domain model shows business relationships, not just process steps.

---

# Granular Classes

As the analyst learns more about the business, the domain model may become more detailed.

Initial classes may split into smaller, more specific classes.

For example, the class **Order** might later become:

- Online Order
- In-Store Order
- Return Order
- Shipping Order
- Payment Record

This happens because the analyst’s understanding of the business becomes clearer over time.

---

# Attributes

## What Are Attributes?

**Attributes** are the pieces of information that describe a class.

They are added inside the class box.

Attributes help explain what data the business has or needs about each class.

---

## Example Attributes
<img width="402" height="256" alt="image" src="https://github.com/user-attachments/assets/7d306a52-43e9-44b6-9197-153e37d70f12" />

### Customer Attributes

- customer ID
- name
- email
- phone number
- address

### Order Attributes

- order ID
- order date
- total amount
- order status
- payment status

### Product Attributes

- product ID
- product name
- price
- inventory quantity
- category

---

# Why Attributes Matter

Attributes help the analyst understand what information is connected to each business element.

They help answer questions like:

- What data do we store about customers?
- What data is needed to process an order?
- What product information is important?
- What data might be missing?
- What information should be included in the analysis?

---

# Domain Models Can Become Large

For simple business processes, a domain model may only have a few classes.

For larger businesses, domain models can become very large and complex.

They may look like a web of connected boxes.

This is normal because large businesses have many connected systems, departments, and processes.

---

# Why Business Domain Models Are Helpful

Business domain models help analysts see the company at a high level.

Instead of starting deep inside one specific process, the analyst can first understand how different parts of the business connect.

This helps the analyst:

- understand the company landscape
- identify important business elements
- see relationships between business areas
- discover relevant areas that may have been missed
- communicate high-level business structure to stakeholders
- decide where to focus deeper analysis

---

# When to Use a Business Domain Model

A domain model is especially useful when first trying to understand the business.

It helps answer:

- What are the main parts of the business?
- How are those parts connected?
- What business areas might affect the problem?
- Which processes may need deeper analysis?

---

# When to Move Away From a Domain Model

Business domain models are useful early in analysis, but they are not always the final tool.

Once the analyst identifies the most relevant process, they will often move from the domain model to more detailed process maps.

## Why?

Because process maps are better for analyzing:

- step-by-step workflows
- process inefficiencies
- bottlenecks
- handoffs
- decision points
- improvement opportunities

---

# Big Lesson

A business domain model gives a high-level view of business relationships.

A process map gives a detailed step-by-step view of a specific process.

Both are useful, but they serve different purposes.

---

# Key Takeaways

- A business domain model shows how business elements relate to each other.
- It is useful for understanding high-level business connections.
- A process flow diagram shows the steps of a specific process.
- A domain model is not necessarily tied to one process.
- The main parts of a domain model are called classes.
- Classes are usually shown in boxes.
- Examples of classes include Customer, Order, and Product.
- Associations show how classes connect.
- The order often connects the customer to the product.
- Associations may not always be directional.
- Attributes are pieces of information that describe each class.
- Domain models can become large and complex as the business becomes more detailed.
- Domain models help analysts understand the company landscape before focusing on specific processes.
- After identifying the most relevant process, analysts may use process maps for deeper analysis.

---

# Extra Important Notes

- A domain model helps prevent analysts from missing important business areas.
- It is useful when the analyst needs a broad understanding of the organization.
- Classes can represent physical things, such as products, or abstract things, such as software actions.
- Associations help show business relationships that may not appear clearly in text.
- Attributes help define what data belongs to each class.
- Domain models and process maps often work together in business analysis.

---

# Final Summary

A business domain model is a visual representation of how different parts of a business relate to each other. It is different from a process flow diagram because it focuses on relationships between business elements rather than step-by-step process flow. The main elements in a domain model are called classes, such as Customer, Order, and Product. Associations show how these classes connect, and attributes describe the data connected to each class. Domain models are especially helpful early in analysis because they show the company at a high level and help analysts discover important business areas they might otherwise miss. Once the most relevant process is identified, the analyst may move from the domain model to detailed process maps.
