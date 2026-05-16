### Fill in the blank: Data professionals use data _____ to control their company’s data and make sure data assets are formally managed.
- governance

---

### Which of the following is the best example of metadata for a column named order_quantity in a sales database table?
- The definition stating that order_quantity represents 'The number of units ordered' and its data type is 'Integer'.

---

### Which of the following statements accurately describe primary and foreign keys in a relational database? Select all that apply.
- A table can have multiple foreign keys.
- Primary keys are unique identifiers for each row in a table.
- Primary keys cannot contain null or blank values.

---

### A data analyst runs the following query. What do they want to retrieve from the database?
```SELECT *
`FROM` VideoGames 
`WHERE` Creator = 'Maddox';
```
- All fields of the video games created by Maddox

---

### What are some benefits of using external data for an analysis project? Select all that apply.
- External data, when validated and trusted, provides more data points and helps analysts identify broad insights.
- External data provides industry-level perspectives.

---

### A data professional at a local zoo is sending an email to all donors who give at least $25 to the zoo each year. What spreadsheet tool will enable them to display only donors who meet that condition? 
- Filter the data to show only donors who have given more than $25 each year

---

### A junior data analyst at a dental care provider uses a tool to explore the data in its patient database. They’re creating a report on the number of times patients floss their teeth each week. This information is stored in the floss_per_week field of the CustomerSurvey table. What query should they write to return only this column of information?  
<img width="450" height="350" alt="image" src="https://github.com/user-attachments/assets/46b8026b-edfc-49b9-b4f3-a536dc159726" />

```
SELECT floss_per_week
FROM CustomerSurvey;
```

---

### Which SQL statement will return only elementary school students from the Grade column of the Students database table?
<img width="450" height="350" alt="image" src="https://github.com/user-attachments/assets/7254d239-e04d-4e38-ad75-bef5d5cd30a2" />

```
SELECT *
FROM Students
WHERE Grade = 'elementary';
```

---

### What are the benefits of open data for the public? Select all that apply.
- Increased public participation and improved decision making.
- Improved understanding of government spending and opportunities to contribute to public planning.

---

### You are a database administrator for a hair salon that specializes in hair treatments and styling. The company is growing, and the number of customers the company needs to keep track of has increased. The limitations of the current database design have become more noticeable. There is a lot more repeated data, such as customer names, phone numbers, and email addresses. This redundancy is causing issues with data integrity and making queries slow. In the tables below what are the primary keys? 
<img width="426" height="350" alt="image" src="https://github.com/user-attachments/assets/c7d5c680-1c69-4e3e-bc58-412dfa1d44a3" />

- customer_id and services_id



