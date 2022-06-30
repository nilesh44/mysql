Refer this for practice
https://www.w3resource.com/sql-exercises/sql-aggregate-functions.php#SQLEDITOR

![image](https://user-images.githubusercontent.com/44174633/176608163-0efdeb24-6699-43c5-bbe8-e6a646ff5a06.png)

```
select city ,max(grade) from customer 
group by city 
order by max(grade) Desc;
```

![image](https://user-images.githubusercontent.com/44174633/176608292-45568e24-f805-4ef2-9b8e-f08ceead4566.png)

```
SELECT customer_id,ord_date,MAX(purch_amt) 
FROM orders 
GROUP BY customer_id,ord_date;
```
![image](https://user-images.githubusercontent.com/44174633/176610795-e30214a0-dbe8-4768-8597-a023b4d23345.png)

```
SELECT salesman_id,MAX(purch_amt) 
FROM orders 
WHERE ord_date = '2012-08-17' 
GROUP BY salesman_id;

```

![image](https://user-images.githubusercontent.com/44174633/176612696-236ba8ab-ff2b-4fd5-a225-0a9426b17934.png)

```
SELECT customer_id,ord_date,MAX(purch_amt) 
FROM orders 
GROUP BY customer_id,ord_date 
HAVING MAX(purch_amt)>2000.00;

```
![image](https://user-images.githubusercontent.com/44174633/176613507-43d5c9a5-6d1e-4be5-a34b-b0935fde0b6c.png)

```
SELECT cust_country,COUNT(grade) 
FROM customer 
GROUP BY cust_country 
HAVING COUNT(grade)>2; 

```
![image](https://user-images.githubusercontent.com/44174633/176616967-f649683f-f47c-434c-a203-18d2f3a3207f.png)

![image](https://user-images.githubusercontent.com/44174633/176617130-7dc4e1e8-23ab-4ed4-95c1-d14d34efbe8c.png)





