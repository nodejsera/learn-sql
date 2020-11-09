# learn-sql
Learning Mysql from scratch daily


1. Type "mysql" on terminal to start using mysql
2. If you were not able to login, you can use the following command   
     mysql -u me -p

     where me is username. And It will ask for password. Enter the user specific password to start.

3. SHOW DATABASES : To list All databases.

    for example: 
    mysql> SHOW DATABASES;

    +--------------------+
    | Database           |
    +--------------------+
    | classicmodels      |
    | information_schema |
    | mysql              |
    | performance_schema |
    | sys                |
    +--------------------+


    
4. USE <DATABASE_NAME>: Used to switch to a specific database.
    for example:

    USE classicmodels;

    Database changed
    

5. SHOW <TABLE_NAME>: This command is used to list tables of the current db.

    mysql> SHOW TABLES;

    |-------------------------+
    | Tables_in_classicmodels |
    |-------------------------+
    | customers               |
    | employees               |
    | offices                 |
    | orderdetails            |
    | orders                  |
    | payments                |
    | productlines            |
    | products                |
    |-------------------------+

    8 rows in set (0.00 sec)

6. SELECT: The SELECT statement allows you to read data from one or more tables.
    Syntax is: 

    SELECT select_list
    FROM table_name;

    Some examples are:
    + To list a specific field:

        SELECT firstName FROM employees;
    + To list multiple fields:

        SELECT firstName, lastName, email FROM employees;
    + To list all fields:

        SELECT * FROM employees;
