# Joins allow you to retrive data from multiple tables in a single select statement
# To join two tables there need to be a related column between them.

#Inner join
# inner join  will retrine data only where there is matching values in both tables.

```
select cu.first_name, cu.last_name , ord.order_time from orders as ord
inner join  customers as cu 
on ord.customer_id=cu.customer_id 
where cu.first_name = 'anil'
order by ord.order_time desc;
```
![image](https://user-images.githubusercontent.com/44174633/175957760-c7081088-d491-4d7c-aea6-c4b3c3cc9a95.png)

# left join will retive data from left table and matching rows from the right table.
```
select cu.first_name, cu.last_name , ord.order_time from orders as ord
Left join  customers as cu 
on ord.customer_id=cu.customer_id 
where cu.first_name = 'anil'
order by ord.order_time desc;
```



# Right Join will retrive all data from right table and matching rows from the left tables.
```
select cu.first_name, cu.last_name , ord.order_time from orders as ord
Right join  customers as cu 
on ord.customer_id=cu.customer_id 
where cu.first_name = 'anil'
order by ord.order_time desc;

```

# Join multiple table

```
select  p.name ,p.price,c.first_name,c.last_name,o.order_time from orders as o
 join products as p on o.product_id = p.product_id 
 join customers as c on o.customer_id = c.customer_id;

```
