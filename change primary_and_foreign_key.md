alter table orders
drop primary key , MODIFY   order_id int;

alter table orders
add primary key (order_id), modify order_id int auto_increment;

alter table orders
add primary key (order_time);

alter table orders
drop primary key;
