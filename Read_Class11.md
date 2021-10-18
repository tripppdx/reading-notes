# Readings: Mongo and Mongoose

## Reading: nosql vs sql

https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool

### 1. Fill in the chart below with five differences between SQL and NoSQL databases:

| SQL | NoSQL |
| ----- | -----|
| vertically scalable | horizontally scalable |
| table based | document based key values |
| predefined schema | dynamic schema |
| called as RDMBS | called as non-relational/distributed |
| Atomicity, Consistency, Isolation and Durability (ACID)| Consistency, Availability and Partition tolerance (CAP)|

### 2. What kind of data is a good fit for an SQL database?

Structured data.

### 3. Give a real world example.

MySQL.

### 4. What kind of data is a good fit a NoSQL database?

Unstructured data.

### 5. Give a real world example.

MongoDB.

### 6. Which type of database is best for hierarchical data storage?

NoSQL.

### 7. Which type of database is best for scalability?

vertically (by increasing the CPU, RAM, SSD, etc, on a single server): SQL
horizontally (by adding more servers): NoSQL.


## Video: sql vs nosql

https://www.youtube.com/watch?v=ZS_kXvOeQ5Y

### 1. What does SQL stand for?

Structured Query Language

### 2. What is a realational database?

A collection of data points or sets organized into tables. These tables are further structured into rows and columns. Each row is identified by a unique key. The columns are organized by attributes. Relational refers to the inter-relation bewteen tables.

### 3. What type of structure does a relational database work with?

Tables.

### 4. What is a ‘schema’?

A schema is the architectural organization of the database. The structure of the columns of attributes (data fields) represent a basic schema. All records (rows) have to adhere to the schema.

### 5. What is a NoSQL database?

A NoSQL (non SQL/ not only SQL) database, is a database that does not store data in relational tables. 

### 6. How does it work?

The databases have flexible schema and allow devs to store large collections of unstructured data. There are four main types, Document, key-value, wide-column stores, and graphh databases. Document databases store their data in JSON-like objects called documents. 

[reference](https://www.mongodb.com/nosql-explained)

### 7. What is inside of a Mongo database?

Mongo is a document-based database. 

### 8. Which is more flexible - SQL or MongoDB? and why.

MongoDB is more flexible because they most easily scale across servers. They also lack strict schema and can therefore be easily updated/ expanded to contain both structured and unstructured data. Performance can be increased by spreading the data across multiple servers (horizontal scaling).

### 9. What is the disadvantage of a NoSQL database?

The main disadvantage of a NoSQL database is that it can contain duplicate data.  The relative lack of relations is fine for reading data, but writes may require changes to multiple collections of documents, impacting performance.

## Additional Resources

mongoose api: https://mongoosejs.com/docs/api.html#Model
React Router: https://reactrouter.com/web/api/BrowserRouter

## Things I want to know more about
