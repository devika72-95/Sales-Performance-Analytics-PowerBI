# 📐 DAX Measures & KPI Calculations

## 1. Overview

DAX (Data Analysis Expressions) was used in Power BI to calculate key performance indicators and support sales performance analysis.

The dashboard focuses on five major business metrics:

- Total Sales
- Total Orders
- Total Quantity
- Average Price
- Average Order Value

## 2. DAX Measures

### 💰 1. Total Sales

Calculates the overall sales revenue generated from retail transactions.

```dax
Total Sales =
SUM(retail_store_sales[Total Spent])
```

**Dashboard Result:** 1.55M

### 🧾 2. Total Orders

Calculates the total number of transaction records.

```dax
Total orders =
COUNTROWS(retail_store_sales)
```

**Dashboard Result:** 13K

### 📦 3. Total Quantity

Calculates the total quantity of products sold.

```dax
Total Quantity =
SUM(retail_store_sales[Quantity])
```

**Dashboard Result:** 66K

### 🏷️ 4. Average Price

Calculates the average price per unit.

```dax
Average price =
AVERAGE(retail_store_sales[Price Per Unit])
```

**Dashboard Result:** 23.37

### 🛍️ 5. Average Order Value

Calculates average sales per transaction record.

```dax
Average order Value =
DIVIDE([Total Sales], [Total orders])
```

**Dashboard Result:** 123.43

## 3. Business Applications of DAX

These calculations help businesses:

- Monitor overall revenue performance.
- Track transaction volume.
- Understand product sales quantities.
- Evaluate average product pricing.
- Monitor average transaction value.
- Analyze performance dynamically using dashboard filters.

## 4. Conclusion

DAX measures provide the foundation for KPI reporting and interactive sales analysis.

By combining DAX calculations with Power BI visualizations, the dashboard converts raw retail transaction data into meaningful business performance indicators.

## 5. Tools Used

- Microsoft Power BI
- DAX
- Power Query
- Retail Store Sales Dataset
