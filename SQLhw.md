SQL Homework

#### Requirements ####

- Find all of the names of the customers who are from London
SELECT * FROM [Customers] WHERE City = 'London';

- Find all of the names of the customers who have a 0 in their postal code
SELECT customerName FROM [Customers] WHERE PostalCode LIKE '%0%';

- Find all of the city names that are in France
SELECT City FROM [Customers] WHERE Country = 'France';	

- Update all of the cities in the UK to be London
UPDATE Customers SET City= 'London' WHERE Country='UK';

- Find the Customer Names and Contact Names for customers who are in North America
SELECT CustomerName, ContactName FROM [Customers] WHERE Country = 'USA';
SELECT CustomerName, ContactName FROM [Customers] WHERE Country = 'Canada';
SELECT CustomerName, ContactName FROM [Customers] WHERE Country = 'Mexico';

- Find all of the customers whose CustomerName's start with a B and ends with an s.
SELECT CustomerName FROM [Customers] WHERE CustomerName like'B%S';

- Find all customers who have a postal code with exactly 4 digits.

- Delete all customers whose ContactNames start with an M
DELETE FROM [Customers] WHERE CustomerName LIKE 'M%';

- Add the following information to the table:
  - id: 110
  - CustomerName: Best Bagels
  - ContactName: John Smith
  - Address: 234 Example St.
  - City: Anytown
  - PostalCode: 12345
  - Country: USA
    
INSERT INTO [Customers] (CustomerID, CustomerName, ContactName, Address, City, PostalCode, Country) VALUES (110, 'Best Bagels', 'John Smith', '234 Example St.', 'Anytown', 12345, 'USA');

- Delete all Customers whose CustomerNames start with an A, or whose ContactNames start with an L
DELETE from [Customers] WHERE CustomerName LIKE A%';
DELETE from [Customers] WHERE ContactName LIKE 'L%';

