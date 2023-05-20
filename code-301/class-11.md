# Class 11 Reading Notes

Fill in the chart below with five differences between SQL and NoSQL databases:

SQL vs NoSQL

- SQL = *relational databases* / NoSQL =  *non-relational or distritbuted database*

- SQL = table based / NoSQL = document based, key value pairs, graph databases/wide-column stores

- SQL = vertically scalable (increasing horse power of the hardware) / NoSQL = horizontally scalable (increasing databases servers in the pool of resources to reduce the load)

- SQL best fit for heavy duty transactional type applications, more stable and promises atomicity/integrity of data. NoSQL is not comparable in high load transactional apps

- SQL excellent support, NoSQL rely on community support

1. What kind of data is a good fit for an SQL database?

- structured data or heavy duty complex transactions

2. Give a real world example.

- creating a record or updating a record of data

3. What kind of data is a good fit a NoSQL database?

- hiearchical data storage

4. Give a real world example.

- JSON file. craigslist

5. Which type of database is best for hierarchical data storage?

-  - managing a library card catalogue <a href="https://www.spiceworks.com/tech/artificial-intelligence/articles/what-is-nosql/#:~:text=Such%20databases%20are%20mainly%20used,Cassandra%2C%20HBase%2C%20and%20Hypertable.">source</a>

6. Which type of database is best for scalability?

- NoSQL

## Video

1. What does SQL stand for?

- Structured Query Language

2. What is a relational database?

- stores/provides access to data points that are related to one another, supports sq label

3. What type of structure does a relational database work with?

- tables, rows, columsn

4. What is a ‘schema’?

- all records in a table have to adhere to a schema, however fetching data and bring into a format needs to fit into a table

5. What is a NoSQL database?

- houses data instead of in a table structure it is in one data structure like a JSON file, does not require schema

6. How does it work?

- have databases with no tables, but have collections with documents (basically the rows in a table), can add new data or fetch new user data and store them in same collection

7. What is inside of a MongoDB database?

- a non relational document database that provides support for JSON data storage, are flexible so you can use unstructured data

8. Which is more flexible - SQL or MongoDB? and why.

- mongoDB is more flexible. It ensures higher data availability while SQL ensjures greater reliability of transactions.

9. What is the disadvantage of a NoSQL database?

- don't support transactions across multiple documents
