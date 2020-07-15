
# Learning PostgreSQL: Checklist

Level 1: Beginner
=================

1.1 Business Case for relational databases
------------------------------------------

-   Describe a few situations in which organisations use a relational
    database
-   Enumerate a few relational database technologies
-   Name a few features that a relational database needs to have
-   Distinguish SQL and NoSQL databases
-   Enumerate advantages of SQL over NoSQL and vice versa

1.2 Getting Started with PostgreSQL
-----------------------------------

-   Draw a diagram explaining how a PostgreSQL server is structured
-   Install PostgreSQL
-   Create a database superuser
-   Create a database
-   Log into psql

1.3 CRUD
--------

-   Run a SQL query in psql
-   Create a table
-   Insert a new row into a table
-   Retrieve all rows from a table
-   Update the values in a specific row
-   Delete a row
-   Use the built-in help function to display the syntax of commands

1.4 Creating Tables
-------------------

-   Enumerate 7 data types you can use in PostgreSQL
-   Use the following constraints when creating a table:

    -   IF NOT EXISTS
    -   PRIMARY KEY
    -   UNIQUE
    -   NOT NULL
    -   DEFAULT
    -   CHECK

-   List all tables in a database

1.5 Writing Select Statements
-----------------------------

-   Write a SELECT statement using the following keywords:

    -   FROM
    -   WHERE
    -   GROUP BY
    -   ORDER BY
    -   HAVING
    -   LIMIT

-   Describe the aggregation functions *count(), sum(), avg(), stddev()*

1.6 JOINs
---------

-   Write a query that connects information from two tables
-   Distinguish INNER JOIN, LEFT JOIN, RIGHT JOIN and CROSS JOIN
-   Explain whether JOIN needs a primary key or not
-   JOIN a table with itself

Level 2: Intermediate
=====================

2.1 Database Clients
--------------------

-   Enumerate programs that connect to PostgreSQL
-   Name the 5 parts of a database connection
-   Connect to a remote database
-   Access your database from your favourite programming language
-   Host a PostgreSQL database on a public server

2.2 Data Modeling
-----------------

-   Add FOREIGN KEY constraint to a table
-   Create a PRIMARY KEY over two columns
-   Explain three different cardinalities two tables can have
-   Draw an ER-diagram for your database
-   Explain why database normalization is important
-   Explain the First to Fourth Normal form and BCNF

2.3 Data Import/Export
----------------------

-   Use COPY to load a table from a CSV file
-   Use COPY to write a table to a CSV file
-   Dump an entire database to a text file
-   Dump a database schema without ownership information or data
-   Restore a database to a text file
-   Use SQLAlchemy to read/write tables to pandas DataFrames

2.4 Basic Administration
------------------------

-   List all your local databases
-   Add a column to an existing table
-   Create an index on a column
-   Delete a database
-   Delete a user
-   Change your password
-   Display/save the psql history

2.5 Advanced SQL Queries
------------------------

-   Use aliases for tables in a SELECT statement
-   Use the DISTINCT keyword
-   Request query results with a specific offset (paging)
-   Perform arithmetical operations in a SELECT statement (e.g. to
    normalize your data)
-   Enumerate functions you can use in a SELECT statement
-   Use a generator function to create data from scratch
-   Concatenate tables with UNION
-   Write query with a CASE statement
-   Write a query containing one or more Sub-SELECTs
-   Write a query prefixed by a WITH clause
-   Create a view from a SELECT statement

2.6 Trivia
----------

-   know who Slonik is
-   know how old PostgreSQL is
-   watch a few conference talks/videos on PostgreSQL

Level 3: Advanced
=================

3.1 Data Cleaning
-----------------

-   replace Null values in a column
-   factorize a column
-   calculate substrings of a column
-   create a pivot table

3.2 More advanced queries
-------------------------

-   Define transactions with COMMIT/ROLLBACK
-   Use a cursor object
-   Use set operations
-   Use a temporary table
-   Use hash functions

3.3. Full Text Search
---------------------

-   Run a Regex query on a text column
-   Run a full text search with tokenization on a text column
-   Create an inverted index (gin)
-   Run an FTS query with a Levenshtein distance of 2
-   Run a trigram search and Metaphones

3.4 Special Data Types
----------------------

-   Run a proximity query based on geographical coordinates
-   Store JSON documents and run queries on multiple nested fields
-   Store parameters of a ML model in an array/cube object
-   Write a ORM class in SQLAlchemy

3.5 Query Performance
---------------------

-   Measure the performance of queries
-   Distinguish btree, gin, gist and hash indexes
-   Interpret the statistics PostgreSQL calculates on columns
-   Calculate and explain a query plan
-   know what VACUUM FULL ANALYZE does

3.6 Administration
------------------

-   Manage multiple users
-   Alter read/write privileges of users
-   Know what a tablespace is
-   Set up an automated backup mechanism
-   Set up a distributed database

3.7 Architecture
----------------

-   Group tables into multiple schemas
-   Define a Trigger function
-   Store schema migrations using a migration tool
-   Use an ETL tool (e.g. Airflow) to continuously update one DB from
    another
-   Understand how Streaming (with Kafka or Apache Flink) relates to a
    relational Database
-   Enumerate a few scenarios where using a different database than
    PostgreSQL is a good idea
