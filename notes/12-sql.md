# SQL

MySQL

select * from (tableName) returns all of the table data options
SELECT * FROM bananaSandwich

where is a match search
WHERE color = 'yellow'                only gets back bananaSandwich that are yellow 

to make an id 
id INT AUTO_INCREMENT PRIMARY_KEY

primary keys cant be edited

DELETE FROM bananaSandwich WHERE id = (id of delete)

mySQLtutorial.org

NOT NULL    makes it required

can have reusable variables 


after setting up auth & database, execute dbSetup.sql
default charset utf8mb4 COMMENT '';           allows you to have emojis

in sql extension open query (looks like a page)

creator id VARCHAR must match what it is set to in the account table

if you tie two tables together they have to have the same character set 

ON DELETE CASCADE     cascades the delete

JOIN connects two tables so you can get back information from both   
just joining it will combine all data with every possibility, so every user will have a copy of every post. So you have to be more specific with you join tables
JOIN accounts ON album.creatorId = accounts.id;

MySQL is not sequential

tables can't hold objects or arrays

when you are asking for information you usually just change the WHERE.
we have an image of what the data should look like, which wont change, we are just searching it differently with WHERE

VIEW is a saved select statement 
can't have duplicate columns in a VIEW

you can where a VIEW, but you have to make changes to the SELECT because it cant have duplicate columns

