# SQL-Datawarehouse-Analytics
This Project is from Baraa on SQL . I have followed the video and executed it to learn the basics of Analytics using SQL

Phase 1 - Exploring the Database
-- To  check what tables are in the database/n
     Select * from INFORMATION_SCHEMA.TABLES
     
--To  check what tables are in the database/n
      Select * from INFORMATION_SCHEMA.COLUMNS/n
	    Where TABLE_NAME = 'dim_customers'
      
-- Explore countries of customers
	Select DISTINCT country FROM gold.dim_customers

-- Explore countries of products, divisions
	Select DISTINCT category,subcategory,product_name FROM gold.dim_products
	order by 1,2,3
