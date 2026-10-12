# Data Types and Naming Conventions
## Declaring Basic Data Types
For data types in SQL, it is a strong tradition to use snake case where the variable starts with a lower case letter with an underscore if it has more than a word. Ex: variable_name
### Examples
DECLARE @age INT;   //For integers, 1st line declared the variable
SELECT @age = 35;  //assigned value to the variable
SELECT @age years_old  //displays the value

DECLARE @flour_in_grams FLOAT;  //for floats
DECLARE @first_name VARCHAR;   //for strings
DECLARE @question BIT;
SET @question = 1;   //for Booleans. True is 1 and False is 0

SQL does not have inherent dictionary or array data types because it's basically a lot of tables.
However, SQL does have some interesting data types like date/time, xml, and geography!
DECLARE @portland GEOGRAPHY;
SET @portland = geography("45 31 12 N 122 40 55 W");
SELECT @portland
