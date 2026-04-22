# Job Applications Spreadsheet Activity — Important Notes

## Goal
Summarize 2023 job application data to answer:

- total applications each month
- total applications for the year
- lowest and highest application months
- average applications per month

---

## Important Setup

- Rename spreadsheet to something clear like `data_analyst_jobs_2023`
- Rename first sheet to `raw data`
- Add a second sheet named `summary data`
- Sort the raw data by **Date** in **ascending order**

---

## Most Important Functions Used

### 1. Convert dates to month names
In `raw data!G2`:

`=TEXT(B2,"mmmm")`

**Purpose:** Converts the date into the full month name, such as January.

---

### 2. Count applications by month
In `summary data!B2`:

`=COUNTIF('raw data'!G:G,A2)`

**Purpose:** Counts how many times the month in `A2` appears in column `G` of the raw data sheet.

**Question 1 answer:** `COUNTIF`

---

### 3. Total applications
In `B14`:

`=SUM(B2:B13)`

**Result:** `32596`

---

### 4. Lowest monthly applications
In `B16`:

`=MIN(B2:B13)`

**Result:** `2312`

**Lowest month:** `February`

---

### 5. Highest monthly applications
In `B17`:

`=MAX(B2:B13)`

**Result:** `3138`

**Highest month:** `July`

---

### 6. Average monthly applications
In `B18`:

`=AVERAGE(B2:B13)`

**Result:** `2716.33`

---

## Monthly Application Totals

| Month | Applications |
|---|---:|
| January | 2387 |
| February | 2312 |
| March | 2536 |
| April | 2544 |
| May | 2954 |
| June | 2990 |
| July | 3138 |
| August | 2969 |
| September | 2865 |
| October | 2751 |
| November | 2508 |
| December | 2642 |

---

## Main Insight

- **February** was the slowest month
- **July** was the busiest month

### Business meaning
The agency could spend more advertising and outreach budget in slower months like **February** and less in peak months like **July**.

---

## Reflection Notes

### How functions help with large data
Functions help analyze large datasets quickly because they automate counting, totaling, and averaging instead of requiring manual work. This saves time, reduces errors, and makes it much easier to find patterns and trends in the data.

### How a data table helps
A data table organizes the results in one clear place, which makes the information easier to read and compare. It also helps communicate key findings, such as monthly trends, totals, and averages, to stakeholders more effectively.

---

## Key Takeaways

- Use `TEXT()` to turn dates into month names
- Use `COUNTIF()` to count applications by month
- Use `SUM()` for yearly total
- Use `MIN()` and `MAX()` to find lowest and highest months
- Use `AVERAGE()` for monthly average
- A summary table makes the results easier to understand and present
