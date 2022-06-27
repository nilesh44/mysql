```
Show databases;

create database test;
use test;
show tables;
Drop database test;

create database coffee_store;

use coffee_store;

create table products(
product_id int auto_increment primary key,
name varchar(30),
price decimal(3,2)
);

show tables;

create table customers(
customer_id int auto_increment primary key,
first_name varchar(30),
last_name varchar(30),
gender Enum('M','F'),
phone_num varchar(11)

);
 create table orders(
 order_id int auto_increment primary key,
 product_id int,
 customer_id int,
 order_time datetime,
 foreign key(product_id) references products(product_id),
 foreign key(customer_id) references customers(customer_id)
 );
 
 Alter table products
 add column coffee_origin varchar(30);
 
 select * from products;
 
 Alter table products
 drop column coffee_origin;
 
 drop table orders;
 drop table products;
 drop table customers;
```

```
insert into customers(first_name,last_name,gender,phone_num) values('anil','singh','M','1234678765');
insert into customers(first_name,last_name,gender) values('raj','patel','M');
insert into customers(first_name,last_name,gender,phone_num) values('rahul','dube','M','1234678765');

insert into products (name,price,origin) values('Espresso',3.00,'american');
insert into products (name,price,origin) values('caspreso',3.00,'american');
insert into products (name,price,origin) values('Doppio',5.00,'itely');
insert into products (name,price,origin) values('indeno',7.00,'india');
insert into products (name,price,origin) values('franso',8.00,'france');

insert into orders(product_id,customer_id,order_time) values(1,2,'2022-06-27 17:20:55');
insert into orders(product_id,customer_id,order_time) values(2,3,'2022-06-28 17:20:55');
insert into orders(product_id,customer_id,order_time) values(2,3,'2022-06-29 17:20:55');
insert into orders(product_id,customer_id,order_time) values(2,4,'2022-06-30 17:20:55');
insert into orders(product_id,customer_id,order_time) values(3,4,'2022-06-26 17:20:55');
insert into orders(product_id,customer_id,order_time) values(3,5,'2022-06-25 17:20:55');
insert into orders(product_id,customer_id,order_time) values(4,5,'2022-06-24 17:20:55');
insert into orders(product_id,customer_id,order_time) values(4,2,'2022-06-23 17:20:55');
```
