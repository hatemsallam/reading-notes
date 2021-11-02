## Defining data using Room entities:

>define each Room entity as a class that is annotated with @Entity. A Room entity includes fields for each column in the corresponding table in the database, including one or more columns that comprise the primary key. `@Entity444`

>each Room entity must define a primary key that uniquely identifies each row in the corresponding database table. `@PrimaryKey`.

> By default, Room creates a column for each field that's defined in the entity. If an entity has fields that you don't want to persist, you can annotate them using @Ignore.`n cases where an entity inherits fields from a parent entity, it's usually easier to use the ignoredColumns property of the @Entity attribute`


> Support full-text search (FTS).

## Save data in a local database using Room :

Apps that handle non-trivial amounts of structured data can benefit greatly from persisting that data locally. The most common use case is to cache relevant pieces of data so that when the device cannot access the network, the user can still browse that content while they are offline.

The Room persistence library provides an abstraction layer over SQLite to allow fluent database access while harnessing the full power of SQLite. In particular, Room provides the following benefits:

-  Compile-time verification of SQL queries.
-  Convenience annotations that minimize repetitive and error-prone boilerplate code.
-  Streamlined database migration paths.


> Primary components: 

- The database class that holds the database and serves as the main access point for the underlying connection to your app's persisted data.

- Data entities that represent tables in your app's database.

- Data access objects (DAOs) that provide methods that your app can use to query, update, insert, and delete data in the database.