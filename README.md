MySQL wasn't able to install on my system so it isn't included 

the code for MySQL is:
1. Creating the database
--CREATING THE DATABASE
CREATE DATABASE atm;



2. Selecting the database
--SELECTING THE DATABASE
USE atm;



3. Create a users table
--CREATE USERS TABLE
CREATE TABLE users(id int primary key auto_increment, card varchar(16), pin varchar(4), uname varchar(25), bal int);


4. Create a transaction table
--CREATE TRANSACTION TABLE
CREATE TABLE transactions(transid int primary key auto_increment, id int, amount int, stat varchar(3), bal int);


5. Create an admin user
--CREATING AN ADMIN USER
INSERT INTO users VALUES(1, "admin", "1234", "admin", 0);
