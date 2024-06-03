# Data Manipulation Language

Language used for selecting, deleting and updating data in a database.
It is used to retrieve and manipulate data in a relational database.

Three basic commands:
1) INSERT
2) UPDATE
3) DELETE

## INSERT STATEMENT

It allows users to insert values into the table based on the integrity constraints.
There are 2 ways to do this:

1) Specify both the column names and the values to be added

Syntax:

INSERT INTO -tablename-(-attribute_names-) VALUES (-add values)

2) Specify only the values if all the columns are being updated

INSERT INTO -tablename- VALUES (-add values)

Insert multiple values by adding the value sets one after another with a ',' separating them

## UPDATE STATEMENT

Used to update the data of an existing table in a database.

Syntax:

UPDATE -tablename-
SET -attributename- = -value', .....
WHERE -condition-

## DELETE STATEMENT

Used to delete some or whole of the data in a table

Syntax:

DELETE FROM -tablename- 
WHERE -Condition-

Note: If condition is not added, the entire table will be deleted