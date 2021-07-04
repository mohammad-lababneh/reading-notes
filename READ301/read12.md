# Mongo and Mongoose
![](https://miro.medium.com/max/594/1*vK4MHL_jpKKmUFGjE5H9jw.png)
#### Things I want to know more about

#### SQL vs NoSQL
(MySQL, Oracle, or other SQL databases)
SQL
- SQL databases are primarily called as Relational Databases (RDBMS)
- SQL databases are table based databases
- SQL databases have predefined schema 
- SQL databases are vertically scalable 
- SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful.
- SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL.
- For the type of data to be stored: SQL databases are not best fit for hierarchical data storage.
#### **NoSQL**
-  NoSQL database are primarily called as non-relational or distributed database.
-  NoSQL databases are document based, key-value pairs, graph databases or wide-column stores.
- NoSQL databases have dynamic schema for unstructured data.
- NoSQL databases are horizontally scalable.
- n NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.
- NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb
- NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set
#### MySQL Community Edition
MySQL database is very popular open-source database. It is generally been stacked with apache and PHP, although it can be also stacked with nginx and server side javascripting using Node js. The following are some of MySQL benefits and strengths.
####  MS-SQL Server Express Edition
It is a powerful and user friendly database which has good stability, reliability and scalability with support from Microsoft. The following are some of MS-SQL benefits and strengths:
- Integrated Development Environment: Microsoft visual studio, Sql Server Management Studio and Visual Developer tools provide a very helpful way for development and increase the developers productivity.
- Disaster Recovery: It has good disaster recovery mechanism including database mirroring, fail over clustering and RAID partitioning.
- Cloud back-up: Microsoft also provides cloud storage when you perform a cloud-backup of your database.
#### 3. Oracle Express Edition
It is a limited edition of Oracle Enterprise Edition server with certain limitations. This database is free for development and deployment. 
#### NoSQL Database Examples
  #### MongoDB
Mongodb is one of the most popular document based NoSQL database as it stores data in JSON like documents. 
  #### CouchDB
CouchDB is also a document based NoSQL database. It stores data in form of JSON documents. 
  #### Redis
Redis is another Open Source NoSQL database which is mainly used because of its lightening speed. It is written in ANSI C language.
#### Model( )
**Parameters**
- doc «Object» values for initial set
- optional «[fields]» object containing the fields that were selected in the query which returned this document. 
- [ skipId=false] «Boolean» optional boolean. 
## Model.aggregate()
**Parameters**
- [ pipeline] «Array» aggregation pipeline as an array of objects
- [ callback] «Function»
#### What does SQL stand for?
Stands for Structured Query Language.
#### What is a realational database?
A  relational database is a type of database that stores and provides access to data points that are related to one another. 
## What type of structure does a relational database work with?
The relational model means that the logical data structures—the data tables, views, and indexes—are separate from the physical storage structures.
#### What is a ‘schema’? 
![](https://i.ytimg.com/vi/E8BCcrM9DDI/maxresdefault.jpg)
We define SQL Schema as a logical collection of database objects. 
#### What is a NoSQL database?
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTOGZUDQiU8RQuLsxK0VNyAjLzpMxffTMIZLA&usqp=CAU)
NoSQL is a type of database that stores and retrieves data without needing to define its structure first - an alternative to the more rigid relational databases
## What is inside of a Mongo database?
MongoDB stores data records as documents (specifically BSON documents) which are gathered together in collections. A database stores one or more collections of 

#### Which is more flexible - SQL or MongoDB? and why?
 MongoDB is more flexible and ensures high and diverse data availability, a SQL Database operates with the ACID (Atomicity, Consistency, Isolation, and Durability) properties and ensures greater reliability of transactions
 #### What is the disadvantage of a NoSQL database?
 ![](https://www.researchgate.net/profile/Msandeep-Kumar/publication/324016909/figure/tbl1/AS:631574211092538@1527590434898/ADVANTAGES-AND-DISADVANTAGES-OVER-NOSQL-DATABASE.png)
 NoSQL databases don't have the reliability functions which Relational Databases have (basically don't support ACID). This also means that NoSQL databases offer consistency in performance and scalability