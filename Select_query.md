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

