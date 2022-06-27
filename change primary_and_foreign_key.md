```
alter table orders
drop primary key , MODIFY   order_id int;

alter table orders
add primary key (order_id), modify order_id int auto_increment;

alter table orders
add primary key (order_time);

alter table orders
drop primary key;

```

## Alter forrign key 
# drop foreign key 
```
alter table orders
drop foreign key orders_ibfk_1(name of constraint refering foreign key);
```
 
# add foregin key 
```
alter table orders
add constraint orders_ibfk_1
foreign key (product_id) references products (product_id);
```
