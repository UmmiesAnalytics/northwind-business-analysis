Northwind Data Model and Relationships 
1.	Overview 
The Northwind data model was developed in Power BI Desktop to connect the database tables and support interactive sales analysis. The relationships allow information from orders, customers, products, employees, and geographical tables to work together across the dashboard. 
The complete relationship diagram is provided in data-model.png. 
2.	Main Tables 
The project uses the following tables for analysis: 
	Table 	Purpose 
Orders 	Contains order-level information, including order dates, customer references, shipping details, and employee references. 
Order Details 	Contains individual product lines within orders, including quantities, unit prices, and discounts. 
Products 	Provides product information, including product names, category references, and supplier references. 
Categories 	Groups products into categories for category-level performance analysis. 
Customers 	Provides customer information for customer-related analysis. 
Employees 	Contains employee information associated with order processing. 
Shippers 	Provides information about shipping companies. 
Suppliers 	Contains information about product suppliers. 
Territories 	Supports geographical territory analysis. 
Regions 	Groups territories into broader geographical regions. 
EmployeeTerritories 	Connects employees with the territories assigned to them. 
The database also contains additional tables that support the wider Northwind dataset. 
3.	Key Relationships 
The model includes relationships between the main transactional tables and their supporting tables. 
Orders and Order Details 
The Orders table represents an order, while Order Details represents the individual product lines within that order. This structure supports analysis of sales at the order and product-line levels. 
Products and Categories 
The Products table connects to Categories so that product performance can be analysed by category. 
Customers and Orders 
The relationship between Customers and Orders supports analysis of orders and sales by customer. 
Employees and Orders 
The relationship between Employees and Orders supports employee-related order analysis. 
Suppliers and Products 
The relationship between Suppliers and Products supports analysis of the suppliers associated with the product catalogue. 
Shippers and Orders 
The relationship between Shippers and Orders supports analysis of shipping activity by shipping company. 
Regions, Territories, and Employees 
The Regions and Territories tables support geographical analysis. EmployeeTerritories acts as a bridge between Employees and Territories, representing the assignment of employees to territories. 
4.	Data Modelling Considerations 
The model was designed to allow related tables to work together while maintaining the distinction between orders and their individual line items. 
Important considerations include: 
●	Identifying the appropriate keys used to connect tables. ● Reviewing relationship cardinality and filter direction. 
●	Avoiding unnecessary or ambiguous relationship paths. 
●	Preserving the distinction between order-level and order-detail-level analysis. 
●	Ensuring that report filters produce meaningful results. 
5.	Business Value 
The relationships support analysis of sales performance across several dimensions, including time, product category, customer, geography, employee, and shipping activity. 
This allows dashboard users to move beyond overall sales totals and investigate the factors contributing to business performance. 
6.	Relationship Diagram 
The file data-model.png provides a screenshot of the complete Power BI Model View, showing the tables and their configured relationships. 
7.	Tools Used 
●	SQLite: source database. 
●	Power BI Desktop: data modelling, relationship configuration, DAX measures, and dashboard development. 
Note: The final documentation should reflect the relationships actually configured in the Power BI model. Confirm relationship cardinalities and filter directions in Model View before documenting their exact settings. 
 
