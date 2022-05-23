# Code 301 - Class 11 - Mongo and Mongoose

## [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

**Fill in the chart below with five differences between SQL and NoSQL databases:**

| SQL Databases                   | NoSQL Databases                 |
| ------------------------------- | ------------------------------- |
| Called as rational databases    | Called as non-rational          |
| Pre-defined schema              | Dynamic schema                  |
| Vertically scalable             | Horizontally scalable           |
| Not best for hierarchical data storage | Better for hierarchical data storage  |
| Better for transactional based apps  | Not best for transactional based apps  |

1. **What kind of data is a good fit for an SQL database?** Complex queries, high transactional based apps

2. **Give a real world example.** Microsoft uses SQL databases

3. **What kind of data is a good fit a NoSQL database?** Hierarchical data storage that needs to be easily managed by both developers and administrators

4. **Give a real world example.** NY Times and Craigslist use NoSQL databases

5. **Which type of database is best for hierarchical data storage?** NoSQL

6. **Which type of database is best for scalability?** NoSQL, because it is horizontally scalable. The workload can be reduced by increasing the number of servers, rather than improving the performance of one server

## [sql vs nosql (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

1. **What does SQL stand for?** Structured Query Language

2. **What is a relational database?** Database that works with certain assumptions, and supports the SQL language

3. **What type of structure does a relational database work with?** Tables

4. **What is a ‘schema’?** The specific requirements for data that gets stored in the database. All records in the database structure have to fit into that schema

5. **What is a NoSQL database?** It is a database that holds large collections of data rather than in a strict table format

6. **How does it work?** A NoSQL database allows you to put all info in one place - Key user data, key product data, etc. go into a collection that might be needed to render on a page. Less relation merging needed creates higher speed for accessing the data you need. Might result in duplicate data, but overall faster

7. **What is inside of a Mongo database?** A Mongo database is made up of collections, which are made up of documents

8. **Which is more flexible - SQL or MongoDB? and why.** MongoDB is much more flexible, because it doesn't require all data to follow the same schema

9. **What is the disadvantage of a NoSQL database?** Uncertainty if all data follows the same schema, potential for slower performance if very complex queries are required

[Back to Home](../README.md)
