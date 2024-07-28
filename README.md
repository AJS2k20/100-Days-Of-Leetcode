# 100-Days-Of-Leetcode
100 Days of Problem Solving on Leetcode

This document contains a brief description of what the code does

### Day 1 
#### 584. Find Customer Referee
selects the names of customers from the customer table where the referee_id is not 2 or is null (indicating no referee). This ensures that only those customers who either do not have a referee or have a referee other than customer with id 2 are retrieved.
_______________________________________________________

### Day 2 
#### 595. Big Countries
The SQL query retrieves the names, populations, and areas of countries from the World table where the area is at least 3,000,000 square kilometers or the population is at least 25,000,000.
_______________________________________________________

### Day 3 
#### 1683. Invalid Tweets
SELECT tweet_id: This selects the tweet_id column from the table.
FROM Tweets: This specifies the Tweets table as the source of the data.
WHERE LENGTH(content) > 15: This condition filters the rows to include only those tweets where the length of the content exceeds 15 characters.
_______________________________________________________

### Day 4 
#### 1757. Recyclable and Low Fat Products
The query selects product_id from the Products table where both low_fats and recyclable are 'Y'. The result can be returned in any order.
_______________________________________________________

### Day 5 
#### 1378. Replace Employee ID With The Unique Identifier
1. FROM Employees e: <br />
★ The primary table Employees is aliased as e. <br />

2. LEFT JOIN EmployeeUNI en on e.id = en.id: <br />
★ A LEFT JOIN combines Employees (e) with EmployeeUNI (en) based on matching id values. <br />
★ Ensures all employees from Employees are included, with null for unique_id if no match is found in EmployeeUNI. <br />

3. SELECT en.unique_id as unique_id, e.name as name: <br />
★ Selects unique_id from EmployeeUNI and name from Employees. <br />
★ Displays null for unique_id if the employee doesn't have one in EmployeeUNI. <br />
_______________________________________________________

### Day 6 
#### 1068. Product Sales Analysis I
SELECT Product.product_name, Sales.year, Sales.price: <br />
  ★ Specifies the columns to be retrieved.<br />
  
FROM Sales: <br />
  ★ The main table from which data is being selected. <br />

INNER JOIN Product ON Sales.product_id = Product.product_id: <br />
  ★ Combines rows from Sales and Product where the product_id matches in both tables. <br />
_______________________________________________________

### Day 7 
#### 197. Rising Temperature
★ The Weather table is aliased as w1 for the main query and as w2 for the subquery. <br />
★ The main query selects id from w1 where the temperature on that date is greater than the temperature on the previous day. This <br /> comparison is made using a subquery. <br />
★ The subquery retrieves the temperature from w2 where w2.recordDate is one day before w1.recordDate. <br />
This is done using the DATE_SUB function which subtracts one day from w1.recordDate. <br />
★ The main query filters the dates where the temperature is higher than the previous day and returns the corresponding id values.
_______________________________________________________
