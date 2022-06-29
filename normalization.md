# normalization is the process of efficiently organizing data in a database.
why to do this ?
* To eliminate redundant data.
* to only store related data in table

# benifits
* reduce storage space
* reduce Insert,update,deletion anomalies
* improve performance.e

# Levels of normalization
* 1st Normal Form (1NF)
* 2nd Normal Form (2NF)
* 3rd Normal Form (3NF)
* Boyce and Codd Normal Form (BCNF)


# 1st Normal Form (1NF)
* No repeted rows of data
* column only contain single value
* The table has a primary key (one column or more then on column which uniquely identified rows of data)

# 2nd Normal Form (2NF)
* tables are in 2NF if
* they conform to 1NF
* every column that is not a primary key of the table is dependent on whole of primary key(because wothout primary key remaining column does not make sense)

# 3rd Normal Form (3NF)

* tables are in 2NF if
* they conform to 1NF
* every column that is not a primary key of the table is dependent on whole of primary key(because wothout primary key remaining column does not make sense)


