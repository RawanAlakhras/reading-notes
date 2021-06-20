# Mongo and Mongoose

## SQL vs NoSQL Database

* SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.

* SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to.

* SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.

* SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.

* SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.

* SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb

* For complex queries: SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.

* For the type of data to be stored: SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data).

* For scalability: In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable.

## What kind of data is a good fit for an SQL database?

* If the data is numeric, favor SMALLINT, INTEGER, BIGINT, DECIMAL, character, or data types.

## Give a real world example

* MySQL database is very popular open-source database. It is generally been stacked with apache and PHP, although it can be also stacked with nginx and server side javascripting using Node js.

## What kind of data is a good fit a NoSQL database?

* highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.

## Give a real world example

* Mongodb is one of the most popular document based NoSQL database as it stores data in JSON like documents.

## Which type of database is best for hierarchical data storage?

* SQL

## Which type of database is best for scalability?

* SQL databases

## What does SQL stand for?

* Structured Query Language

## What is a realational database?

* is a type of database that stores and provides access to data points that are related to one another.

## What type of structure does a relational database work with?

* B-TREE ,collection of tables, each having a unique name. A row in a table represents a relationship among a set of values. Thus a table represents a collection of relationships. There is a direct correspondence between the concept of a table and the mathematical concept of a relation.

## What is a ‘schema’?

* Is a cognitive framework or concept that helps organize and interpret information, represents the logical configuration of all or part of a relational database.

## What is a NoSQL database?

* which stands for “not only SQL,” is an approach to database design that provides flexible schemas for the storage and retrieval of data beyond the traditional table structures found in relational database.

## What is inside of a Mongo database?

* MongoDB stores data records as documents which are gathered together in collections. A database stores one or more collections of documents.

## Which is more flexible - SQL or MongoDB? and why

* MongoDB, some research has shown that the speed of MongoDB could be 100x faster than a relational database, and it has easy setup.

## What is the disadvantage of a NoSQL database?

* don't have the reliability functions which Relational Databases have (basically don't support ACID).
