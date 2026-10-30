Data Preparation and Cleaning 
Overview 
The Northwind dataset was prepared in Power Query in Power BI Desktop before building the data model and dashboard. The preparation process focused on improving column names, correcting data types, reviewing missing values, and making the tables suitable for analysis. 
Data Preparation Steps 
1. Data Import 
The Northwind SQLite database was used as the original data source. The database tables were imported into Power BI for transformation, modelling, and analysis. 
2. Column Headers 
The Customers table initially contained generic column names, including Column1 and Column2. These were corrected to meaningful headers so that the fields could be interpreted and used appropriately in the report. 
3. Data Types 
Column data types were reviewed and corrected where necessary. Appropriate data types are important for accurate date filtering, numerical calculations, currency analysis, and relationships between tables. 
4. Orders Table 
The Orders table was reviewed for missing values and potential data-quality issues. 
●	CustomerID blanks and duplicate-related issues were reviewed and addressed during preparation. 
●	Empty values in ShipRegion and ShipPostalCode were reviewed. ● Three missing ShippedDate values were identified and reviewed. 
Missing shipment dates were not automatically treated as errors because an order may not yet have been shipped. Missing values must be interpreted in the context of the business process. 
5. Order Details Table 
The Order Details table was reviewed and cleaned as needed. Duplicate rows were not removed automatically, since order-detail records must be evaluated in context before deciding whether they represent genuine duplicates. 
6. Data Model Readiness 
The prepared tables were used to build relationships in Power BI. The model includes sales-related tables and supporting tables such as Customers, Products, Categories, Employees, Territories, and Regions. 
Data Quality Considerations 
Data preparation was performed with the aim of preserving valid business records while addressing issues that could affect analysis. 
Key considerations included: 
●	Using meaningful column names. 
●	Applying suitable data types. 
●	Reviewing missing values rather than deleting them indiscriminately. 
●	Avoiding automatic duplicate removal where it could remove legitimate transactions. 
●	Preparing tables for reliable relationships and report filtering. 
Tools Used 
●	SQLite: original database source. 
●	Power BI Desktop: data import, Power Query transformations, data modelling, DAX calculations, and dashboard development. 
Outcome 
The preparation process established a usable foundation for the Northwind sales analysis. The cleaned tables were subsequently used to develop the Power BI data model, calculate key performance indicators, and build interactive dashboard pages. 
Note: This document describes the preparation steps performed during the project. Specific transformation details should be updated if the Power Query steps are revised. 
 
