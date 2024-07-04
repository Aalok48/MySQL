# MySQL
mysql learning
mysql is not case sensitive but it is recommended to use uppercase

# Create database

CREATE DATABASE db_name   # this command to create a new database

# drop or delete a database

DROP DATABASE db_name     # this command to delete a database


# this command is used to make mysql understand to run queries on the particular database db_name

use db_name 


# this command to create the table

create table table_name(
    column1 datatype,       # here after datatype constraint is passed
    column2 datatype,       # primary key should be unique
    column3 datatype
);

# this command to insert values into the table
INSERT INTO table_name values(column1_value, column2_value, column3_value)

# this command to print the table 
select * from student;

# check if the database is present of not before creating and deleting

create database if not exists db_name;    # if already a db exits it gives a warning

drop database if exists db_name; 

# to show the databases and tables

show databases;
show table;


# select keyword in mysql

select * from table_name;    
select distinct col_name from table_name;    (gives distinct values from table only)

# where clause in mysql (more like a condition)

select city from city_column where city = 'pokhara'

# to turn off safe mode in sql

set sql_safe_updates = 0

# to update table

update table_name set col1 = val1, col2 = val2 where condition;

# Alter the table (to change schema)

# to add column

alter table table_name add column column_name datatype constraint ;

# to drop column

alter table table_name drop column column_name;

# to rename table

alter table table_name rename to new_table_name;

# to rename a column

alter table table_name change column old_name new_name new_datatype new_constraint;

# to modify a column

alter table table_name modify column_name new_datatype new_constraint;

# drop deletes the whole table whereas truncate deletes the table data

truncate table table_name;