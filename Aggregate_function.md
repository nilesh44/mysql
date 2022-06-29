# What is an Aggregate Function in SQL?
# An aggregate function in SQL returns one value after calculating multiple values of a column. We often use aggregate functions with the GROUP BY and HAVING clauses of the SELECT statement.
* Perform a calculations on Data within a column and returns one result row.
* can use GROUP BY clause to group the result by one or more columns.
* can use a HAVING clause in similar way to a Where clause in select statement to filter the resultset.
* 
# Various types of SQL aggregate functions are:

* Count()
* Sum()
* Avg()
* Min()
* Max()
```
SELECT count(customerId) as customerIds , customerId FROM Orders 
group by customerId  
order By count(customerId) desc;
```
![image](https://user-images.githubusercontent.com/44174633/176415867-0dd86802-e102-42df-a10c-31cf80ce1b00.png)
