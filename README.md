# SQL Query HW

[Questions and Requirements](https://github.com/Filipe-p/sql-queries-excercise/blob/master/sql_exercises_homework.md)

### How many orders in NWDB?
```
SELECT COUNT(*) AS 'Number of Orders' FROM Orders;
```
Answer = 830

### How many orders where the ShipCity is Rio de Janeiro?
```
SELECT COUNT(*) AS 'Number of Orders shipping to Rio de Janeiro' FROM Orders
WHERE ShipCity = 'Rio de Janeiro';
```
Answer = 34

### Orders where the ShipCity is Rio de Janeiro or Reims
```
SELECT * AS FROM Orders
WHERE ShipCity IN ('Rio de Janeiro', 'Reims');
```
Answer = 39 (if using ``COUNT(*)``)

### All entries where company name has z or Z in table of customers
```
SELECT * FROM Customers
WHERE CompanyName LIKE '%z%';
```
Answer = 6 (if using ``COUNT(*)``)


