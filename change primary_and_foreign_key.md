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

# add unique constraint
```
alter table customers
add constraint phone_number_unique unique (phone_number);
```

# drop unique constraint
```
alter table customers
drop index phone_number_unique (name of constraint refering unique key);
```

# change column name
```
alter table customers
change phone_number(old_column_name) phone_num(new_column_name) varchar(10)(data type);
 ```
 
 # change data type
``` 
 alter table customers
 modify phone_num varchar(11);
```
