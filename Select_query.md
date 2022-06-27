# simple query to fetch all records from the table with all column .

```
select * from customers;
```

# fetch only selected column like first_name and last_name of customer.
```
select first_name , last_name from customers;
```

# use of where clause to filter out record on the basis of condition

```
select * from customers where first_name = 'anil';
```

here it will fetch all record whose first name is anil.

# WHERE clause  with AND

```
select * from products 
where origin= 'american' 
and price <= '3.00';
```

# WHERE clause  with OR

```
select * from products 
where origin= 'american' 
and price <= '3.00';
```
# fetch records Where column has null value

```
select * from customers where phone_num is null;
```

# fetch records where column has not null values

```
select * from customers where phone_num is not null;
```

# where clause and Between

```
select * from orders
where order_time 
between '2022-06-17' and '2022-06-25';
```

# where clause and like
```
select * from customers where 
first_name 
like 'a%';
```
![image](https://user-images.githubusercontent.com/44174633/175936550-e77c4fbe-e2ba-4ef9-aa42-3bb857cf0483.png)

```
select * from customers 
where first_name 
like '%l';
```
![image](https://user-images.githubusercontent.com/44174633/175936633-b8d22e1f-d776-4cce-a96f-f2a4d5e050b8.png)

```
select * from customers 
where first_name 
like '%ni%';
```
![image](https://user-images.githubusercontent.com/44174633/175936681-8b32a5ee-24b5-44bf-b6a1-74c8b56bdd8a.png)

```
select * from customers 
where first_name 
like 'anil';
```
![image](https://user-images.githubusercontent.com/44174633/175936767-2e5737f0-49e5-4fc5-8192-869672982a8c.png)

# Order by , sort resultset in Ascending order
```
select * from orders 
order by order_time ASC;
```
![image](https://user-images.githubusercontent.com/44174633/175937871-1700ad04-a227-4318-9ea0-dca0747b6a48.png)

# Order by , sort resultset in Descending order
```
select * from orders
order by order_time DESC;
```
![image](https://user-images.githubusercontent.com/44174633/175938043-11bbc8cd-2c9e-416c-903d-a69184018a22.png)

# where clause and Order by 
```
select * from orders 
where product_id = 2 
order by order_time DESC;
```
# Distinct
```
select distinct customer_id from orders where product_id = 2 ;
```
![image](https://user-images.githubusercontent.com/44174633/175939552-b35fd784-283c-4256-bd21-20e161b47be9.png)

# Limit (fetch first two record) , for fetching number of rows.
```
select * from products limit 2;
```
![image](https://user-images.githubusercontent.com/44174633/175941606-93bd0685-7746-4b11-939a-78664d30b008.png)

# Limit with Offset(does not rreturn first 3 records)
```
select * from products limit 2 offset 3;
```
![image](https://user-images.githubusercontent.com/44174633/175941342-45660535-1586-4846-98c3-60c6ebbaa7f7.png)
