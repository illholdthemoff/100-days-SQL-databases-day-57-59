SQL databases have clearly defined schema and layouts. Data and relations can be queried. This can of course be done across tables to conenct records

SQL is also used for data analysis tasks
![alt text](SQL-server-connection.jpg "Title")

MySQL is a software suite, not SQL itself. The server is what will of course hold our data
On this server we will create our databases

![alt text](SQL-layout.jpg "Title")

This is the general layout of a database

something to note when creating columns in MySQL
PK - Primary Key - this is the primary identifier for units within the table
NN - Not Null - this means that this entry is not allowed to be null
AI - Auto Increment - this means that rather than having to manually check and add the number each time, this will do it for you
UQ - Uniuque Index - normally this sounds like somehting you'd want to select for a field that should be used for the ID, but when you select something as a primary key, its already selected as a UQ as well.

some standard keywords to note
INSERT INTO - keywords that say you want to instert data into a cell
VALUES - the things you ad in
SELECT - run command to select data from table
WHERE - allows you to select a subset of data, usually by column
COUNT - returns the number of tables which meet your parameters (ie id, name, type etc)
UPDATE - lets you update via using SET to select which to be updated
DELETE - you get it, DELETE FROM table WHERE thing = value
![alt text](SQL-select.jpg "Title")

What is neat about this is that you can just go back to whatever tab it was that had your insert into, and edit things around and execute again, and so on

An example of various keywords used at once

![alt text](SQL-various.jpg "Title")

Something to note regarding SQL tables, you dont really wnat to have a nunch of complex data in a single cell. Often times people will link mulitple tables together through ids, creating references to information stored in other tables to keep things neat
![alt text](SQL-links.jpg "Title")
