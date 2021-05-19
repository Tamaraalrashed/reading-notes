# Data Modeling

## Three advantages to Test Driven Development

1. Better program design and higher code quality.
2. Detailed project documentation.
3. TDD reduces the time required for project development.

## what case would you need to use beforeEach() and afterEach() in a test suite?
While testing a logger middleware.

## one downside of Test Driven Development

- Big time investment.

## The primary difference between ES6 Classes and Constructor/Prototype Classes

The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.<br>

A child of an ES6 class is another type definition which extends the parent with new properties and methods, which in turn can be instantiated at runtime. A child of a prototype is another object instance which delegates to the parent any properties that aren’t implemented on the child.<br>

## Why REST

- REST is Easy to Understand and Implement.
- REST Makes your Application More Scalable.
- Caching is Easier with REST.
- REST is Flexibile.
- 
<br>

## SQL vs NOSQL

In the last several years, NoSQL database is getting widely adopted to solve various business problems. <br>


High-Level Differences:<br>
- SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.<br>

- SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to..<br>

- SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.<br>

- SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load. <br>

- SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database. <br>

- SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb. <br>

## NOSQL Data Modeling Techniques

- Key-Value storage is a very simplistic, but very powerful model. Many techniques that are described below are perfectly applicable to this model.<br> 


- One of the most significant shortcomings of the Key-Value model is a poor applicability to cases that require processing of key ranges. Ordered Key-Value model overcomes this limitation and significantly improves aggregation capabilities.
Ordered Key-Value model is very powerful, but it does not provide any framework for value modeling. In general, value modeling can be done by an application, but BigTable-style databases go further and model values as a map-of-maps-of-maps, namely, column families, columns, and timestamped versions.<br>

- Document databases advance the BigTable model offering two significant improvements. The first one is values with schemes of arbitrary complexity, not just a map-of-maps. The second one is database-managed indexes, at least in some implementations. Full Text Search Engines can be considered a related species in the sense that they also offer flexible schema and automatic indexes. <br>
  
- Graph data models can be considered as a side branch of evolution that origins from the Ordered Key-Value models. <br>


## General Notes on NoSQL Data Modeling

- NoSQL data modeling often starts from the application-specific queries as opposed to relational modeling:
   - Relational modeling is typically driven by the structure of available data. The main design theme is  “What answers do I have?” 
   - NoSQL data modeling is typically driven by application-specific access patterns, i.e. the types of queries to be supported. The main design theme is “What questions do I have?” .
- NoSQL data modeling often requires a deeper understanding of data structures and algorithms than relational database modeling does. <br>
- Data duplication and denormalization are first-class citizens. <br>
- Relational databases are not very convenient for hierarchical or graph-like data modeling and processing. Graph databases are obviously a perfect solution for this area, but actually most of NoSQL solutions are surprisingly strong for such problems. <br>

## Conceptual Techniques

 - Denormalization.
 - Aggregates.
 - Application Side Joins.
 - Atomic Aggregates.
 - Enumerable Keys.
 - Dimensionality Reduction.
