# Code 401 - Class 04 - Data Modeling

## [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

### What type of database is the best fit for the complex query intensive environment?

- SQL databases are better for this

### What type of database is the best fit for hierarchical data storage?

- NoSQL database

### Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend

- A SQL database usually runs on a single server, so it can be scaled by increasing the power of the hardware it's running on. But a NOSQL database is usually shared across several servers, so it can be scaled by increasing the number of servers sharing it

## [sql modeling techniques](https://www.essentialsql.com/get-ready-to-learn-sql-7-simplified-data-modeling/)

### Among data tables, what is a one-to-many relationship and how do we “relate” them?

- This relationship occurs when an entry in one table can be related to more than one entry in another

### Prior to designing your relational database, it might be useful to `create a diagram` of the database tables and their relationships

### Explain the difference between a primary and foreign key

- A **primary key** uniquely identifies each row in a table, and a table usually only has one of these

- A **foreign key** is a column (or set of columns) which match a primary key in another table

## [sql vs nosql](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

### How do we treat keywords and parameters differently in SQL syntax?

- Looks like uppercase for Keywords and lowercase for Parameters, maybe

### Define normalization within the context of schemas and data

- When data is brought into a table, it must be formatted to fit the exact schema before it can be added to the table. This is called *normalization*

### Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter

- **One-to-One:** When one item in a table corresponds to one item in another table
- **One-to-Many:** When an item in a table might be connected to several different items in another table (or tables)
- **Many-to-Many:** When multiple items in a table might be connected to several different items in other tables

[Back to Home](../README.md)
