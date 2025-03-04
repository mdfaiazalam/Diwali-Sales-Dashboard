# Dynamic Dashboard for Diwali Sales
## Overview
This project involves creating an interactive and insightful dashboard using Microsoft Excel to analyze a Diwali sales dataset. The dashboard provides key metrics and visualizations that enable users to explore the dataset dynamically through slicers, charts, and pivot tables.


## Dataset Overview
* User_ID: Unique identifier for each customer.
* Cust_name: Name of the customer.
* Product_ID: Unique identifier for each product.
* Gender: Gender of the customer.
* Age Group: The age range of the customer.
* Age: Exact age of the customer.
* Marital_Status: Marital status (0 = Single, 1 = Married).
* State: State where the customer resides.
* Zone: Zone of the customer (e.g., Western, Southern, Central, etc.).
* Occupation: Profession of the customer.
* Product_Category: Category of the purchased product.
* Orders: Number of orders placed by the customer.
* Amount: Total amount spent by the customer.

## Key Metrics Displayed

Total Sales: Sum of the "Amount" column.

Average Order Value: Calculated as Total Amount / Total Orders.

Top Customers: Customers ranked by total amount spent.

Regional Sales: Sales grouped by zones or states.

Customer Demographics:

Sales by Gender.

Sales by Age Group.

Sales by Marital Status.

Product Analysis:

Total sales by Product Category.

Orders categorized into "Low Orders (1-2)", "Medium Orders (3-4)", and "High Orders (5+)".

### The dashboard includes slicers for:

Gender
* Age Group
* Zone
* State
* Marital Status
* Product Category
* These slicers allow users to dynamically filter data and view specific subsets of the dataset.

##Steps to Create the Dashboard

### 1. Data Preparation

Remove Duplicates: Ensured no duplicate entries exist in the dataset.

Add Calculated Columns:

Average Spending per Order: Amount / Orders

Order Category: Categorized orders into:

=IF(Orders <= 2, "Low Orders", IF(Orders <= 4, "Medium Orders", "High Orders"))

### 2. Pivot Tables

Created pivot tables for:

Total Sales by Zone: Zones as rows, total "Amount" as values.

Sales by Gender: Gender as rows, total "Amount" as values.

Top Customers: Customer names as rows, total "Amount" as values.

Sales by Age Group: Age groups as rows, total "Amount" as values.

Sales by Occupation: Occupation as rows, total "Amount" as values.

### 3. Visualizations

Added dynamic charts linked to the pivot tables:

Bar Chart: Total Sales by Zone.

Pie Chart: Sales distribution by Gender.

Line Chart: Daily sales trend (if Date column is added).

Map Chart: Sales by State (requires properly formatted state names).

### 4. Interactive Filters

Inserted slicers for Gender, Zone, Age Group, Marital Status, Product Category, and Order Category.

Connected slicers to all relevant pivot tables.

### 5. Dashboard Layout

Top Row: Key metrics (Total Sales, Average Order Value, Total Orders).

Middle Section: Charts (e.g., Bar Chart for Regional Sales, Pie Chart for Gender Distribution).

Bottom Section: Pivot tables for detailed insights (e.g., Top Customers, Sales by Occupation).

Side Section: Slicers for dynamic filtering.
