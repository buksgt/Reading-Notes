# table of contents
## code 301 reading notes
## Class 11 reading notes
### Reading Class 0011, 8 APR

Chart Comparing SQL and NoSQL Databases:

Aspect	SQL	NoSQL
Data Storage	Relational tables with predefined schema	Non-relational, various formats like document, key-value
Schema	Fixed, structured schema	Dynamic, flexible for unstructured data
Scaling	Vertical scaling (enhancing hardware)	Horizontal scaling (across multiple servers)
Query Language	Uses Structured Query Language (SQL)	No standard; varies (e.g., JavaScript-based queries)
Consistency	ACID compliance (strong consistency)	Often prioritizes performance; eventual consistency
SQL Database - Good Fit:

Suitable for structured data with complex relationships.
Real World Example: Banking systems where transactions, customer data, and account information are closely related and require consistency.
NoSQL Database - Good Fit:

Ideal for unstructured or semi-structured data; high variability or changing needs.
Real World Example: Social media platforms managing diverse data types like text, images, and user interactions.
Hierarchical Data Storage:

NoSQL databases (especially document-based or graph databases) are better suited due to flexible schemas.
Scalability:

NoSQL databases are typically more scalable, especially in distributed environments.
 

Video:Links to an external site.

 

SQL: Stands for "Structured Query Language," a standard programming language specifically designed for managing and manipulating relational databases.

Relational Database: A type of database that stores and provides access to data points that are related to one another. It's based on a relational model of data.

Structure in Relational Databases: These databases work with a table-based structure, where data is stored in rows and columns, forming a table. Each row represents a record and each column represents an attribute of the data.

Schema: In database systems, a schema is the structure that defines the organization of data, including tables, fields, relationships, views, indexes, etc. It's like a blueprint for how the database is constructed.

NoSQL Database: A NoSQL database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases. They are often used for large sets of distributed data. They can be document-oriented, key-value pairs, wide-column stores, or graph databases.

Inside a MongoDB Database: MongoDB, a NoSQL database, typically contains collections of documents. These documents are JSON-like field and value pairs. Collections in MongoDB are analogous to tables in relational databases.

Flexibility - SQL vs. MongoDB: MongoDB is often considered more flexible than SQL because it can handle a wide variety of data types and structures without needing a predefined schema. This flexibility makes it easier to accommodate changes in data structures over time.

Disadvantage of NoSQL Database: A notable disadvantage is that they often lack the robust ACID (Atomicity, Consistency, Isolation, Durability) transactional properties that SQL databases provide. This can make them less suitable for complex transactional applications where data consistency is a critical factor.

# Things I want to know more about.