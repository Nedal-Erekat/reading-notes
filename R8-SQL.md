# SQL
#### SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.
> SQLite, MySQL, Postgres, Oracle and Microsoft SQL Server. All of them support the common SQL language standard
##### A relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.
* To retrieve data from a SQL database, we need to write `SELECT` statements
> Select query for a specific columns
```
SELECT column, another_column, …
FROM mytable;
```
> Select query for all columns
```
SELECT * 
FROM mytable;
```
* to filter certain results from being returned, we need to use a `WHERE` clause in the query. 
> Select query with constraints
```
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```

- `=, !=, < <=, >, >=`	Standard numerical operators
- `BETWEEN … AND …`	Number is within range of two values (inclusive)
- `NOT BETWEEN … AND …`	Number is not within range of two values (inclusive)
- `IN (…)`	Number exists in a list	
- `NOT IN (…)`	Number does not exist in a list
- LIKE	Case insensitive exact string comparison
- NOT LIKE	Case insensitive exact string inequality comparison	
- %	Used anywhere in a string to match a sequence of zero or more characters (only with LIKE or NOT LIKE)	
```
SELECT title, director FROM movies 
WHERE title LIKE "Toy Story%";
```

* `DISTINCT` keyword will blindly remove duplicate rows
* QL provides a way to sort your results by a given column in ascending or descending order using the `ORDER BY` clause.