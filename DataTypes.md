# Data Types and Naming Conventions
## Declaring Basic Data Types
For data types in SQL, it is a strong tradition to use snake case where the variable starts with a lower case letter with an underscore if it has more than a word. Ex: variable_name
### Examples
DECLARE @age INT;   #For integers, 1st line declared the variable
SELECT @age = 35;  #assigned value to the variable
SELECT @age years_old  #displays the value

DECLARE @flour_in_grams FLOAT;  #for floats 

DECLARE @first_name VARCHAR;   #for strings

DECLARE @question BIT;
SET @question = 1;   #for Booleans. True is 1 and False is 0

SQL does not have inherent dictionary or array data types because it's basically a lot of tables.
However, SQL does have some interesting data types like date/time, xml, and geography!

DECLARE @portland GEOGRAPHY;
SET @portland = geography("45 31 12 N 122 40 55 W");
SELECT @portland

## Language Details
SQL has around 79 common reserved words. These include ADD (adds a column in an existing table) ALTER (adds, deletes, or modifies columns in a table, or changes the data type of a column in a table) and INDEX (creates or deletes an index in a table).

Again, variables cannot have spaces in them, and it is a strong tradition in the community to use snake_case (although camelCase or PascalCase is alright). You should be consistent with your naming conventions because the variables need to be read by other people accessing the database. The variables you enter are mutuable, so other people can alter them.

Since SQL is a declarative query language, the way it's typed mostly depends on the application you're using.  If you're writing it statically, the variables are fixed at compile time. If you're writing it dynamically, the variables are fixed at run time. SQL can be explicitly or implicitly typed. An example for explicitly type: the CAST and COVERT functions to convert a value from 1 data type to another. An example for implicitly typed is comparing a smallint to an int.

It's a weakly typed language; which means that it can crash if you enter code in wrong. However, if you do want to mix type operations, you can do so with parentheses and logical operators (ex: ALL, AND, ANY, BETWEEN, EXISTS, NOT, etc). SQL can also use arithmetic, comparision, compound, and bitwise operators.

A limitation with SQL may be differentiating between all the different data types. It's ok to look up what you want your specific data type to be. You can use [https://www.geeksforgeeks.org/sql/sql-data-types/](url) as a resource.

Some of the more complex data types are in a special category because they have specific data to enter. For example, if you want to enter in data in a Euclidean coordinate system, use the GEOMETRY data type.
