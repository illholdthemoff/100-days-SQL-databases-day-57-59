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

When linking to another table, the common naming convention is to use the name of that table (not plural) then underscore and whatever it is youre linking, for example, grabbing ids from the addresses table would be address_id. The datatype should be the same. Also related but not necessarily needed is the foreign keys tab, right underneath.
Foreign Key = a field (column) that references a field in another table, like address_id

Soemthing to note regarding datatypes in SQL. When for example you create an INT type column with the intent of storing a number between 1-10 or somehting like that, you would handle taht in the backend JS code, which would filter numbers accordingly.

Another notable datatype is TEXT. This doesn't require you to enter a max char limit though you can. Typically this is used for things like storing blog posts and other long form things that would go over 255 chars, although I guess you could use it for othe rthings too if you dont want to be efficient

Also to note is DATETIME. This of courese is reserved for the date and time, and in the Default/Expression, you can place CURRENT_TIMESTAMP to timestamp automatically whenever you add a new record

INNER JOIN - important keyword(s), allows you to combine data from mulitple tables, after you type it you specify which tables you want to join, and the fields that you wish too with the ON keyword.

![alt text](SQL-join.jpg "Title")
An example of using the INNER JOIN and ON keywords to combine data from mutpliepl tables

IMPORTANT!!!!! remember to double clikc the active schema you're woprking on on the side (makes it bold) so that it sets it as the active one, or else you'll have to prefix everything with the schema.whatver.id etc etc

![alt text](SQL-join-multi.jpg "Title")
An example of a multi line joining with multiple tables involved. Note the AS, that means that when you add that particular one in, it will be labeled AS whatever you name it, this is useful because otherwise you could get multiple different fields with the same name.

![alt text](SQL-join-where.jpg "Title")
An example of a multi line join that uses everything we learned so far

And finally, one more infograph of how SQL databases work and their various relationships

![alt text](SQL-layout-2.jpg "Title")
