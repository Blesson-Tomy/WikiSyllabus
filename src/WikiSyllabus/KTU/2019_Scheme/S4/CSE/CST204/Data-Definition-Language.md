# Data Definition Language

Responsible for defining the way data is structured in a database. In SQL it allows us to manipulate a Database by:

1) Creating a Table
2) Altering a Table
3) Dropping a Table
4) Altering a Table
5) Truncate a Table
6) Renaming a Table

SQL data definition language allows the specification of information about relations, including:
1) Scheme for each relation
2) Domain of values associated with each atrribute
3) Integrity Constraints


## Domain Types
1) char(n)
2) varchar(n)
3) int
4) float(n)
5) smallint
6) real, double
7) numeric(p,d) where p=no of digits, d=digits after decimal point

## CREATE STATEMENTS

1) CREATING A DATABASE
Syntax: CREATE DATABASE -name of db-

Database is a structured set of data.

2) CREATING A TABLE
Syntax: CREATE TABLE -name of table- (
    -variable name- -domain type-
)

### Integrity constraints in CREATE
1) Domain Constraints
2) Integrity Constraints
3) Referential Integrity Constraints

- Primary Key
    - attribite has to be non null and unique
- Foreign Key
    - Value of attribute has to correspond to values of the primary key attributes of some tuple in a relation
- Not Null
    - Value cannot be null

## DROP/TRUNCATE STATEMENTS

Drop statements are used to delete an entire table or database including the structure. 
It destroys existing objects like an existing database table, view or index.
This command cannot be undone.

Syntax: 
DROP TABLE -name of table-
DROP DATABASE -name of db-

Truncate statement on the otherhand, only deletes the data in the table and preserves the structure.
This allows user to reuse the table's structure when necessary.
It is ultra-fast and can be undone.

TRUNCATE TABLE -name of table-
TRUNCATE DATABASE -name of db-

## ALTER STATEMENTS
Used to add, delete/drop or modify columns in the existing table.
Add and drop various constraints on the existing table.



### ADD
Add can be used to add columns into the existing table.

Syntax:

ALTER TABLE -table name-
ADD (-column name- -datatype-);

## DROP
Used to drop a column in a table

Syntax:
ALTER TABLE -tablename-
DROP COLUMN -columnname-;

## MODIFY
Used to drop a column in a table

Syntax:
ALTER TABLE -tablename-
MODIFY COLUMN -columnname- -columntype-;





