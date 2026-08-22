# Power Query Practice Questions (Orders Dataset)

## Basic Level

### Q1.
Import the **Orders.csv** file into **Power Query** and rename the query as **Orders_Data**.

### Q2.
Assign the correct data types to all columns. For example:
- Order Date → Date
- Ship Date → Date
- Sales → Decimal Number
- Quantity → Whole Number
- Discount → Decimal Number
- Profit → Decimal Number

### Q3.
Rename the following columns:
- Row ID → Order_No
- Customer Name → Customer
- Product Name → Product

### Q4.
Remove the **Postal Code** column from the dataset.

### Q5.
Filter the dataset to display only the orders belonging to the **Technology** category.

### Q6.
Sort the dataset by:
- Order Date (Oldest to Newest)
- Sales (Largest to Smallest)

### Q7.
Remove duplicate records based on **Order ID** and **Product ID**.

### Q8.
Replace all blank or null values in the **Postal Code** column with **"Unknown"** before removing the column.

---

# Intermediate Level

### Q9.
Split the **Customer Name** column into two columns:
- First Name
- Last Name

### Q10.
Create a custom column named **Profit Margin (%)** using the formula:

> (Profit / Sales) × 100

### Q11.
Create a **Conditional Column** named **Profit Status** using the following conditions:

| Condition | Result |
|-----------|--------|
| Profit > 100 | High Profit |
| Profit between 0 and 100 | Medium Profit |
| Profit ≤ 0 | Loss |

### Q12.
Extract the following fields from **Order Date**:
- Year
- Month Name
- Quarter

### Q13.
Merge the **City** and **State** columns into a new column named **Location** in the format:

```
City, State
```

### Q14.
Add an **Index Column** starting from **1001**.

### Q15.
Group the data by **Category** and calculate:
- Total Sales
- Total Profit
- Total Quantity

---

# Advanced Level

### Q16.
Create a **Conditional Column** named **Discount Category** using the following conditions:

| Discount | Category |
|----------|----------|
| 0 | No Discount |
| 0.01 – 0.20 | Low Discount |
| 0.21 – 0.50 | Medium Discount |
| Above 0.50 | High Discount |

### Q17.
Create a **Custom Column** named **Delivery Days** using the formula:

```
Ship Date - Order Date
```

### Q18.
Group the data by **Region** and **Segment**, then calculate:
- Total Sales
- Average Profit
- Number of Orders

### Q19.
Create a **Conditional Column** named **Sales Category** using the following conditions:

| Sales | Category |
|-------|----------|
| Less than 100 | Low |
| 100 to 500 | Medium |
| Above 500 | High |

### Q20.
Create a final transformed table that contains only the following columns:

- Order ID
- Order Date
- Customer
- Segment
- Category
- Sub-Category
- Product
- Sales
- Profit
- Profit Margin (%)
- Profit Status
- Delivery Days
- Sales Category

Ensure the final table has:
- Correct data types
- Meaningful column names
- No duplicate records
- No unnecessary columns
- Data ready for loading into Excel or Power BI