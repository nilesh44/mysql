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
phone_number varchar(11)

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