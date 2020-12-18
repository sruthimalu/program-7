# program-7
7Implementation of Build in functions in RDBMS

a.	Create a table store. Fields are order no, code, item, quantity, price, discount, mrp

b.	Insert values into the table

c.	Display the table

d.	Write an SQL query to display the reminder, if the amount of an each item in store is divided by 9.

e.	Write SQL query to display the amount in store and its square

f.	Write SQL query to divide the amount in stock of each item by 7 in store table and display the result round to the nearest integer.



create table store(order_no int(5), code  varchar(10), item varchar(20), quantity int(2), price int(5), discount int(2), MRP int(5),primary key(order_no));

insert into store values(90001,'AX5432','SSHH',2,649,30,879);

insert into store values(90002,'BY3471','TTAA',1,559,25,720);

insert into store values(90003,'CZ6312','WWCC',2,432,50,832);

insert into store values(90004,'DL7481','HHEE',4,1345,60,1675);

insert into store values(90005,'EQ4954','MMAA',3,800,30,1255);

select * from store;

select mod(price,9) from store;

select price,power(price,2) from store;

select round(quantity div 7) from store;


