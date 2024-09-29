# Data-Analysis
Supply Chain Data Analysis 

1. Project Description:
The project offers a real-world dataset focused on supply chain analytics. Helps in resolving significant shipment and inventory management concerns, analyzing supply chain inefficiencies, and developing meaningful dashboards to notify business stakeholders about potential issues and propose fundamental business improvements.

2. Methodology:

**Business demand analysis**

Requirements: A Dashboard to analyze the business problem and improve the supply chain’s efficiency

Method: descriptive, exploratory and diagnostic analysis

Tool: Python (Data preprocessing, data cleaning, EDA, inventory segmentation); 
      Power BI (Dashboard)

Sales Manager: Overview and keep track of customer’s demand and product sales

Inventory Manager: Control the inventory flow including order fulfillment, storing and distribution 

Shipping Manager: Overseeing daily shipping and distribution operations to customers

3. Data Preprocessing:

Customer:
General information about customers including identifiers and addresses

Order:
Information about the order including date of order, product and quantity ordered, order value

Shipment:
Shipping information including shipping date, shipping mode

Product:
Specific information about the ordered item including product name, product category, product department

Warehouse Inventory:
Information on inventory management for each product name including monthly inventory, warehouse location, storage costs, order fulfillment

**Data cleaning**

1. Dropping unnecessary columns (Order Item ID, Order Time)

2. Fixing the datatype of the columns

3. Removing special characters in Customer Country column

4. Checking for missing value

5. Checking for duplicate value

6. Inconsistency of Product Name between order and inventory table
   
7. Negative and unusual large shipping time

**Feature creation**

1. Creating Date time feature from day, month, year feature
   
2. Creating Shipment feature to show which order is late or on time

  Shipping Time = Shipment Date - Order Date

  Delay Shipment = Late if Shipment Day - Schedule Shipping Time and vice versa

  Late Shipment Rate = Total of late order / Total number of order

3. Create Business performance feature

  Net Sales = Gross sales - Discount * Gross sales

  Unit Price = Gross sales / Order Quantity

  Profit margin = Total Profit / Total Net sales 

  Storage cost = Inventory cost per unit * Warehouse inventory 
