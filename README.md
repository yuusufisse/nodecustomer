# Nodecustomer

Create database and table for the customers

### Connect to database
Connect to the postgres database using postgres user
<img src="/images/image 1.png" alt="Connect to postfres" title="Connect to postfres">

### Create a new database
Create a new database called customer
```SQL
CREATE DATABASE customer;
```
<img src="/images/image 2.png" alt="Create a new database" title="Create a new database">

### Create customers table
Create customers table to the customer database
```SQL
CREATE TABLE customers (
  id serial PRIMARY KEY,
  firstname VARCHAR (250) NOT NULL,
  lastname VARCHAR (250) NOT NULL,
  email VARCHAR (250) NOT NULL,
  phone VARCHAR (250) NOT NULL
);
```
<img src="/images/image 3.png" alt="Create a new table" title="Create a new table">

### Verify that customers table exists
Type \d command in the SQL Shell to verify that customers table exists
```SQL
\d
```
<img src="/images/image 4.png" alt="Verify table exists" title="Verify table exists">

### Insert some demo data
Connect to customer database by typing \c customer command
```SQL
INSERT INTO customers (firstname, lastname, email, phone) VALUES ('John', 'Johnson', 'john@johnson.com', '8233243');
INSERT INTO customers (firstname, lastname, email, phone) VALUES ('Mary', 'Smith', 'mary@smith.com', '6654113');
INSERT INTO customers (firstname, lastname, email, phone) VALUES ('Peter', 'North', 'peter@north.com', '901176');
```
<img src="/images/image 5.png" alt="Insert data" title="Insert data">

### Check the customers table
Check that customers are added to the customers table
```SQL
SELECT * FROM customers;
```
<img src="/images/image 6.png" alt="Check table" title="Check table">




