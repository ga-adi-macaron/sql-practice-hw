---
title: SQL Practice
type: Homework
duration: "1:00"
creator:
    name: Drew Mahrt
    city: NYC
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) SQL Practice

## Exercise

Go to the [W3Schools SQL Practice website](http://www.w3schools.com/sql/trysql.asp?filename=trysql_delete). Click the **Customers** table on the right side to show the data it contains.

In the requirements section below, you will find tasks to complete on the **Customers** table. Work through as many as you can. Copy each SQL command into a text file as you complete them.

#### Requirements

- Find all of the names of the customers who are from London.

  ```SQL
  SELECT CustomerName FROM Customers WHERE City = "London";
  ```

- Find all of the names of the customers who have a 0 in their postal code

  ```SQL
  SELECT CustomerName FROM Customers WHERE PostalCode LIKE "%0%";
  ```

- Find all of the city names that are in France

  ```SQL
  SELECT City FROM Customers WHERE Country = "France";
  ```

- Update all of the cities in the UK to be London

  ```SQL
  UPDATE Customers SET City = "London" WHERE Country = "UK";
  ```

- Find the Customer Names and Contact Names for customers who are in North America

  ```SQL
  SELECT CustomerName, ContactName FROM Customers WHERE Country IN ("Canada", "Mexico", "USA");
  ```

- Find all of the customers whose CustomerName's start with a B and ends with an s.

  ```SQL
  SELECT * FROM Customers WHERE CustomerName LIKE "B%s";
  ```

- Find all customers who have a postal code with exactly 4 digits.

  ```SQL
  SELECT * FROM Customers WHERE LENGTH(PostalCode) = 4;
  ```

- Delete all customers whose ContactNames start with an M

  ```SQL
  DELETE FROM Customers WHERE ContactName LIKE "M%";
  ```

- Add the following information to the table:
  - id: 110
  - CustomerName: Best Bagels
  - ContactName: John Smith
  - Address: 234 Example St.
  - City: Anytown
  - PostalCode: 12345
  - Country: USA

  ```SQL
  INSERT INTO Customers VALUES (110, "Best Bagels", "John Smith", "234 Example St.", "Anytown", "12345", "USA");
  ```

- Delete all Customers whose CustomerNames start with an A, or whose ContactNames start with an L

  ```SQL
  DELETE FROM Customers WHERE CustomerName LIKE "A%" OR ContactName LIKE "L%";
  ```

#### Deliverable

A text file containing each of the SQL commands.  Submit a pull request!

## Additional Resources

- [SQL Syntax](http://www.w3schools.com/sql/sql_syntax.asp)

---

## Licensing
1. All content is licensed under a CC­BY­NC­SA 4.0 license.
2. All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact [legal@ga.co](mailto:legal@ga.co).
