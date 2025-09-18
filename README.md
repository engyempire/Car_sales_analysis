# Car_sales_analysis
**This is my report for car sales**

## Car Sales Data Analysis Report

---

### Project Overview

This project analyzes car sales data to uncover insights on sales distribution by various attributes such as car color, region, and month. Using pivot tables, I explored metrics like total sales by color and region, average income of buyers, gender distribution, and overall revenue. This analysis helps to understand the key factors driving car sales in the USA and identifies patterns across different segments.

---

### Data Source: kaggle.com 

### Tools Used
1.	#### Excel Pivot Tables:  
     1. For summarizing
     2. exploring trends in car sales data.
     3. [View Visuals Here](https://ibb.co/HN9GT9X)
---      
2.	#### SQL: For querying the dataset to:
      1. calculate totals
      2. averages
      3. specific breakdowns
  ---       
4.	#### Power BI: .
       1. For creating interactive visualizations
       2. For Dashboard Creation [View Here](https://ibb.co/LgpcFV8)
       3. For visuals that present data insights in a user-friendly format
  ----

### Data Overview
The dataset includes the following columns:

-	CarID: Unique identifier for each car sold.
-	Color: Color of the car.
-	Region: Geographic location where the car was sold.
-	SaleDate: Date when the sale was completed.
-	Income: Income of the buyer.
-	Gender: Gender of the buyer.
-	Revenue: Revenue generated from each sale.

### Analysis Breakdown

1. #### Total Sales by Car Color
Using pivot tables, I summarized the total sales by car color to understand the popularity of each color among buyers. This breakdown helps in understanding customer preferences.

#### Key Insight:
Certain colors may appeal more to buyers, informing inventory decisions and marketing strategies.

2. ##### Sales Distribution by Region
I analyzed sales by region using pivot tables to identify areas with the highest and lowest sales.

### Queries
```sql
---Selecting Black cars sold---
SELECT * FROM car_sales
WHERE color = 'Black';
```

```sql
---Total sales Query sort by Model---
SELECT Model, COUNT(Car_id) AS TotalSales
FROM car_sales
GROUP BY Model
ORDER BY TotalSales DESC;
```

```sql
---Calculate Total Revenue by Dealer Region---
SELECT Dealer_Region, SUM(Price) AS TotalRevenue
FROM car_sales
GROUP BY Dealer_Region
ORDER BY TotalRevenue DESC;
```

### Data Visualization

![Screenshot (188)](https://github.com/user-attachments/assets/cc96052d-ab88-4646-9c0a-7697f0a6c1d5)

---

### Second Car Dashboard
![car_kelechi](https://github.com/user-attachments/assets/e4c0c9c2-a9a5-4c72-a0af-7b81b3263ff3)

---

### Visuals for Performance from January to December
![Screenshot (392)](https://github.com/user-attachments/assets/0843a10f-3602-4a45-9d24-748bd506c7af)
