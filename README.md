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
