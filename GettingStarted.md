# Getting Started (Installation/First Code
  ## Installation
  There are many resources to help set up SQL. I used MyWebSQL, a website specifically used for students to learn SQL. It gives a broader range of SQL than an extension like SQLLite would. For this, check with your technology or CS department if they have this set up for students. If so, have a meeting with an instructor to set up your account and allow you access to the databases.  If not, Microsoft has a few extensions you can download onto VSCodium (or another programming environment) for you to code on. **You need to make sure you have both a place to code and a database to draw from.** 

  ## A Simple Start
  You run programs in MyWebSQL by selecting one of the databases your institution or workplace has provided for you. Then, we'll start by creating a table and putting some values into it. The way to write comments is to either #comment or /* comment */. You run the program by pressing 'run query'. My server is MariaDB, so the syntax is a little different from others. The file has 4 queries that creates a table and adds 3 rows of information. Run the queries separately.

  ### The Actual Code

  #My server is MariaDB, so the syntax may differ from another. This file has 4 queries that you can run separately from each other.

#creating a table with the title and year established
CREATE TABLE Musicals(
  title text,
  year_est int
);

#adding some data into the table
INSERT INTO Musicals (title, year_est)
  VALUES ("Annie", 1977);

INSERT INTO Musicals (title, year_est)
  VALUES ("Chicago", 1975);

INSERT INTO Musicals (title, year_est)
  VALUES ("Hamilton", 2015);
