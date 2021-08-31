# Room

* The advantage of apps that are handling non-trivial amounts of structured data is that user can continue using the app while it is offline, because data is locally stored.
* There is a Room persistence library that we can use to access data in SQLite.
* The advantages of using Rooms
    1. Clear comments or annotations to prevent and reduce errors.
    2. Compile-time verification of SQL queries.
    3. Simple database paths.

## Primary Components For Room

* The database class: it is a class that holds all database and serves.
* Data Entities that represent tables in database class.
* Data access objects (DAOs) that holds the methods that are related to database and its statements.

## Database

* The class that hold the database must has
    1. Annotated with a @Database.
    2. Be an abstract class that extends RoomDatabase.
    3. Define an abstract method that has zero arguments and returns an instance of the DAO class.

## Defining data using Room entities

* Using Room library, you can define entities that is related to what you want to store.
* Room entities can be used to define database schema without writing any SQL code.
* Each Room entity must be declared as a class that is annotated with @Entity, to includes the fields for each column in the entity.
* Room uses the class name as the database table name, but it can be changed if you set the tableName property of the @Entity annotation an @ColumnInfo annotation to set the name of the column.
* Each table has a primary key that can be set using @PrimaryKey annotation.
* You can use @Ignore annotation to ignore fields.
* You can use full-text search to search for details in your database's tables.
* @AutoValue annotation can be used if there are two instances of an entity are equal.

## Define relationships between objects

* Room doesn't allow object references, but you can create embedded objects.
* Use @Embedded annotation to represent an object that you'd like to divide into its subfields within a table.
* @Relation annotation, parentColumn and entityColumn to set the relation between entities.

## Accessing data using Room DAOs

* DAO is used to ease the test of your app while you mock database.
* DAO can be an interface or abstract class, and you must use @Dao annotation.
* There are two types of DAO methods that define database interactions:
  * Convenience methods: insert, update, and delete
  * Query methods: write your own SQL query
