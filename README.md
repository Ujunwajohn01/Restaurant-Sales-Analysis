# Restaurant-Sales-Analysis
### INTRODUCTION
An Excel-based data analytics project using restaurant order data to extract key business
insights and operational strategies.

**Table of Contents**

- Project Overview

- Project Scope

- Project Objectives

- Expected Outcome

- Document Purpose

- Use Case

- Data Source

- Data Cleaning and Processing

- Data Analysis

- Data Visualization

- Recommendations

- Conclusion

**Project Overview**

This project provides a comprehensive analysis of a year's worth of restaurant sales data.
Using Microsoft Excel, the goal is to extract actionable insights from customer orders, sales
patterns, and menu performance to drive strategic business decisions and operational
optimization.

**Project Scope**

The project spans all aspects of the restaurant's sales data, including:
- Order details (date, time, item, quantity)
- Menu items (name, category, price)
- Sales trends by day, hour, and month
- Revenue contributions by category and item
- Identification of bestsellers and underperformers

**Project Objectives**
- **Customer Flow:** Determine daily and hourly customer patterns
- **Order Behavior:** Calculate the average number of items per order
- **Menu Performance:** Identify top and bottom performing items and categories
- **Revenue Analysis:** Evaluate total revenue and detect seasonality
- **Strategic Insights:** Provide operational and promotional recommendations

**Expected Outcome**

This project aims to deliver:
- Clear insights into customer habits
- Visualizations of peak periods and sales performance
- A prioritized menu strategy
- Actionable suggestions to increase sales and improve efficiency

**Document Purpose**

This document is intended to:
- Summarize the analysis process and results
- Serve as a portfolio piece demonstrating Excel-based data analytics
- Inform restaurant managers on data-backed decisions

**Use Case**

**1. Business Owners & Management:** to understand which products drive revenue and make
informed decisions on staffing and stock

**2. Marketing Teams:** to plan promotions around peak times and popular items and rebrand
or remove low-performing menu options

**3. Operations Teams:** to schedule staff based on high-traffic days/hours and optimize supply
chain management

**Data Source**

- **Source:** [Maven Analytics website](https://mavenanalytics.io/data-playground?order=date_added%2Cdesc&search=restaurant%20) designed for practice purposes. This dataset consists of a quarter's worth of orders from a fictitious restaurant serving international cuisine, including the date and time of each order, the items ordered, and additional details on the type, name and price of the items.

- **Tools Used:** Excel 

- **Sheets Used:**
   - **Order_Details:** contains order IDs, dates, times, item IDs, and pricing

  - **Menu Items:** includes item names, categories, and prices
    
- **Total Records:** 12,235 orders covering a full calendar year
  
- **Columns include:** Order_id, Order_Date, Order_Time, Item_Name, Category, Price, Hour, etc.

### Data Dictionary
- **menu_item_id:**	Unique ID of a menu item
- **item_name:**	Name of a menu item
- **category:**	Category or type of cuisine of the menu item
- **price:**	Price of the menu item (US Dollars $)
- **order_details_id:**	Unique ID of an item in an order
- **order_id:**	ID of an order
- **order_date:**	Date an order was put in (MM/DD/YY)
- **order_time**:	Time an order was put in (HH:MM:SS AM/PM)
- **item_id:**	Matches the menu_item_id in the menu_items table


### KEY DATA ANALYSIS

**1. Total Customer Order per Week**

**Objective:** To analyze customer traffic across the week to identify which days are busiest or
slowest for the restaurant.

**Methodology:** Using a pivot table in Excel:
- Day was placed in the Rows section.
- Order_ID was placed in the Values section (set to Count).
A line graph was used to visualize the number of customers (orders) per day.

![](https://github.com/Ujunwajohn01/Restaurant-Sales-Analysis/blob/main/Total%20Custom%20Orders%20per%20Week.png)

**Findings:**
- Friday and Monday have the highest number of orders, indicating peak customer
engagement at the start and end of the workweek.
- Saturday records the lowest order volume.

**Interpretation:**
- Customers tend to treat themselves on Fridays and seek convenience on Mondays.
- Saturdays might be slower due to traditional home-cooked meals or rest routines.

**Implications:**
- Allocate more staff on Fridays and Mondays.
- Consider special Saturday promotions to increase sales.


**2. Highest Spending Orders**

**Objective:** To identify which individual orders generated the most revenue.

**Methodology:**
- Created a pivot table with Order_ID in Rows and total Revenue in Values.
- Sorted descending to find the highest values.

![](https://github.com/Ujunwajohn01/Restaurant-Sales-Analysis/blob/main/Highest%20Spending%20Orders.png)

**Findings:**
- Top 5 highest spending orders ranged from $185 to $192.
- These orders typically contained multiple items across categories.
  
**Implications:**
- Indicates potential for bundled meal promotions.
- Target group orders for special offers.


**3. Is there a peak hour for orders?**

**Objective:** To determine which hours of the day experience peak or low order volumes for
better scheduling and inventory planning.

**Methodology:**
- Created a pivot table with Hour in the Rows section.
- Order_ID in Values as Count.
- A bar chart is used to visualize the hourly distribution of customer orders.

![](https://github.com/Ujunwajohn01/Restaurant-Sales-Analysis/blob/main/Time%20of%20the%20Day%20with%20Higest%20Sales.png)

**Findings:**
- 12 PM is the busiest with 1,659 orders.
- 1 PM follows closely with 1,558 orders, reflecting an extended lunch rush.
- High volume during lunch and dinner is consistent with typical fast-food behavior.
- A secondary peak occurs around 5–6 PM.
- 10 AM and 11 PM had the lowest order volumes (5 and 11 respectively).
- Early morning and late-night hours see minimal traffic.

**Implications:**
- Schedule staff breaks during off-peak hours.
- Consider off-peak deals or breakfast specials pre-noon.


**4. Best-selling and underperforming items?**

**Objective:** To rank menu items by quantity sold, identifying popular and unpopular dishes.

**Methodology:**
- Created pivot tables grouping by Item Name.
- Counted item frequency.
- Visualized with bar charts (Top 5 and Bottom 5).

![](https://github.com/Ujunwajohn01/Restaurant-Sales-Analysis/blob/main/Most%20Ordered%20Item.png)

![](https://github.com/Ujunwajohn01/Restaurant-Sales-Analysis/blob/main/Least%20Ordered%20Item.png)

**Findings:**
- Most ordered item: Hamburger (American category)
- Least ordered item: Chicken Tacos (Mexican category)

**Implications:**
- Promote top sellers to increase sales volume.
- Remove or rework underperforming items.


**5. Monthly revenue trends & seasonality**

**Objective:** To track revenue trends across months for identifying seasonal demand patterns.

**Methodology:**
- Extracted Month from Order Date.
- Created pivot tables summing Revenue by month.
- Line graph visualized monthly revenue.

![](https://github.com/Ujunwajohn01/Restaurant-Sales-Analysis/blob/main/Month%20with%20the%20Highest%20Sales.png)

**Findings:**
- March had the highest revenue.

**Implications:**
- Run marketing campaigns before or during peak months.
- Prepare for dips with special discounts in off-seasons.


**6. Total Orders & Revenue contribution by category**

**Objective:** To evaluate which menu categories, contribute most to total orders & overall
revenue.

**Methodology:**
- Pivot table grouped by Category, summing total Revenue and counting total orders.
- Visualized using a stacked bar chart.

![](https://github.com/Ujunwajohn01/Restaurant-Sales-Analysis/blob/main/Revenue%20per%20Category.png)

**Findings:**
- Italian and Asian cuisines generated the most revenue.
- American food, while popular, had the lowest revenue per item.

**Implications:**
- Expand offerings in high-margin categories.
- Adjust pricing in lower-margin categories.

### DATA VISUALIZATION

![](https://github.com/Ujunwajohn01/Restaurant-Sales-Analysis/blob/main/Full%20Dasboard.png)

### RECOMMENDATIONS
**1. Staffing:** Increase staff on weekends and during lunch/dinner peak hours

**2. Inventory Management:** Prioritize stock for top-selling items

**3. Promotions:**

a. Offer Wednesday & Saturday specials to increase traffic

b. Promote underperforming items via bundle deals or remove if needed

**4. Marketing:** Advertise popular dishes (e.g., Korean Beef Bowl, Hamburger,
Cheeseburger, Fries etc.)

**5. Menu Review:** Streamline offerings by cutting consistently low sellers

### CONCLUSION
This project reveals crucial insights into the restaurant’s operations and customer behavior.
By leveraging Excel’s capabilities, it translates raw data into a decision-making tool for
management. With these insights, the restaurant can optimize efficiency, boost revenue, and
improve customer satisfaction.

**Contact:**
Obianujunwa V. John

Email: ujunwajohn01@gmail.com

Location: Lagos, Nigeria

**Role Target:** Data Analyst position in a data-driven organization focused on growth,
efficiency, and customer experience.

### THANK YOU

  
