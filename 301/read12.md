| SQL      |  NoSQL |
| ----------- | ----------- |
|    called as Relational Databases (RDBMS)    |   called as non-relational or distributed database   |
| table based databases  |   document based, key-value pairs, graph databases or wide-column stores    |
|  have predefined schema  |    have dynamic schema for unstructured data    |
|   vertically scalable  |   horizontally scalable    |
|  examples: MySql, Oracle, Sqlite, Postgres and MS-SQL |   examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb     |




## What kind of data is a good fit for an SQL database?

the complex query intensive environment.



## Give a real world example.

On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.



## What kind of data is a good fit a NoSQL database?

 hierarchical data storage



## Give a real world example.

it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.



## Which type of database is best for hierarchical data storage?

NoSQL database



## Which type of database is best for scalability?

SQL databases 





## What does SQL stand for?

Structured Query Language. SQL is used to communicate with a database. According to ANSI (American National Standards Institute), it is the standard language for relational database management systems.



## What is a relational database?

 A relational database is a type of database that stores and provides access to data points that are related to one another. Relational databases are based on the relational model, an intuitive, straightforward way of representing data in tables. In a relational database, each row in the table is a record with a unique ID called the key. The columns of the table hold attributes of the data, and each record usually has a value for each attribute, making it easy to establish the relationships among data points.


## What type of structure does a relational database work with?

The relational model means that the logical data structures—the data tables, views, and indexes—are separate from the physical storage structures. This separation means that database administrators can manage physical data storage without affecting access to that data as a logical structure. For example, renaming a database file does not rename the tables stored within it.


## What is a ‘schema’?

its structure described in a formal language supported by the database management system (DBMS). The term "schema" refers to the organization of data as a blueprint of how the database is constructed (divided into database tables in the case of relational databases). The formal definition of a database schema is a set of formulas (sentences) called integrity constraints imposed on a database.


## What is a NoSQL database?

NoSQL databases are purpose built for specific data models and have flexible schemas for building modern applications. NoSQL databases are widely recognized for their ease of development, functionality, and performance at scale. This page includes resources to help you better understand NoSQL databases and to get started.


## How does it work?
NoSQL databases use a variety of data models for accessing and managing data. These types of databases are optimized specifically for applications that require large data volume, low latency, and flexible data models, which are achieved by relaxing some of the data consistency restrictions of other databases.



## What is inside of a Mongo database?

MongoDB stores data records as documents (specifically BSON documents) which are gathered together in collections. A database stores one or more collections of documents.



## Which is more flexible - SQL or MongoDB? and why.

While MongoDB is more flexible and ensures high and diverse data availability, a SQL Database operates with the ACID (Atomicity, Consistency, Isolation, and Durability) properties and ensures greater reliability of transactions






## What is the disadvantage of a NoSQL database?


don't have the reliability functions which Relational Databases have (basically don't support ACID). This also means that NoSQL databases offer consistency in performance and scalability.