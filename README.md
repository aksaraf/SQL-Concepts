# SQL-Concepts

> A well organized and good code is not the one computers can understand, it is the one humans can understand.

SQL (Structured Query Language) is a programming language specifically designed for working with databases. It allows us to create, share, manipulate data especially from Relational Database Management Systems

Query is a piece of code inducing a computer to execute a certain operation that will deliver the desired output. The latter process is called querying the database.

SQL is a declarative language because while coding we are not interested in how the job is done but interested in what result we want to obtain.

### Components of SQL's Syntax
1. **Data Definition Language (DDL):**  A set of statements that allows the user to define or modify data structures and objects, such as tables.
    1. CREATE: used for creating entrire database and database objects like tables.
       ```SQL
       CREATE TABLE table_name
       (
       column_1 datatype,
       column_2 datatype,
       ....
       );
       ```
    2. ALTER: used for altering exisiting objects like adding, removing or renaming exisiting column in a table.
       ```SQL
       ALTER TABLE table_name
       ADD COLUMN column_name datatype;
       ```
    3. DROP: used for deleting a database object.
       ```SQL
       DROP object_type object_name;
       ```
    4. RENAME: used for renaming a database object.
       ```SQL
       RENAME object_type object_name TO new_object_name;
       ```
    5. TRUNCATE: instead of deleting the entire table using DROP, we can just delete records from the table using TRUNCATE.
       ```SQL
       TRUNCATE object_type object_name;
       ```

### Date Functions (MySQL)
1. CURDATE(), CURRENT_DATE, CURRENT_DATE(): Returns current date in YYYY-MM-DD format as a text.
   ```SQL
   SELECT CURDATE(), CURRENT_DATE, CURRENT_DATE();
   ```
2. NOW(): Returns both current date and time.
   ```SQL
   SELECT NOW();
   ```
3. CURRENT_TIME(), CURRENT_TIME, CURTIME(): Returns current time as a string in the hh:mm:ss format.
   ```SQL
   SELECT CURRENT_TIME(), CURRENT_TIME, CURTIME();
   ```
