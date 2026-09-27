# Veda-Technology-Task-20
# Customer Order Count — Task 20

**Data Analytics Track | VEDA Technology Internship | Level 1 · Day 20 of 45**

##  Overview

This task analyzes customer purchase behavior using the **Online Retail dataset**, counting distinct orders placed by each customer and identifying the top frequent buyers.

##  Objective

Understand simple customer behavior by counting orders per customer and identifying which customers are frequent (repeat) buyers versus one-time buyers.

##  Dataset

- **Name:** Online Retail
- **Rows:** 1,670 order lines
- **Customers:** 120
- **Columns:** `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

##  Tools Used

- Microsoft Excel (formulas: `SUMPRODUCT`, `SUMIFS`, `INDEX`, `MATCH`, `RANK`, `COUNTIF`)
- SQL (for querying and aggregating order data)

##  Methodology

1. Added a helper column (`IsFirstInvoiceLine`) to flag the first line of every invoice, so multi-line orders are **not double-counted**.
2. Built a **Customer Order Table** with, for every customer:
   - Distinct **Order Count**
   - **Total Quantity** purchased
   - **Total Spend**
3. Used `RANK` + `INDEX`/`MATCH` to extract the **Top 10 frequent buyers** into a separate sheet.

##  Deliverables

| File | Description |
|---|---|
| `Online_Retail_Dataset.xlsx` | Raw dataset + Customer Order Table + Top Customers sheets (formula-driven) |
| `Task20_Customer_Order_Count_Report.pdf` | Summary report with methodology, key figures, chart, and conclusion |

##  Key Results

- **120** customers placed a combined **390** distinct orders across **1,670** order lines
- **41** customers were repeat buyers; **79** ordered only once
- Total customer spend: **£35,242.07**
- Top customer (by order count): **Customer 12443** with 21 distinct orders

##  Conclusion

Distinct orders, quantity, and spend were calculated per customer using formulas that auto-update if the source data changes. The top 10 frequent buyers were identified, helping highlight the most valuable, repeat customers worth prioritizing for retention and loyalty efforts.
---
