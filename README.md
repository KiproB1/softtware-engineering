# softtware-engineering
Database design
Database:

A database is a structured collection of data organized and stored electronically in a way that allows for efficient retrieval, management, and manipulation of data. It serves as a repository for storing and managing various types of information, such as customer data, product information, financial records, and more.
Table:

A table is a fundamental structure in a relational database that represents a collection of related data organized in rows and columns. Each column in a table represents a specific attribute or field, while each row represents a single record or entry containing values corresponding to each attribute.
Record:

A record, also known as a row or tuple, is a single instance or entry within a database table that contains a complete set of related data values. Each record represents a unique entity or item within the database, such as a customer, product, transaction, or employee.
Field:

A field, also known as a column or attribute, is a specific piece of data within a database table that represents a particular characteristic or property of the entities described by the table. Each field corresponds to a specific data type, such as text, number, date, or boolean, and holds values related to that attribute for each record in the table.
Primary Key:

A primary key is a unique identifier or attribute within a database table that uniquely identifies each record or row in the table. It serves as a unique reference point for accessing and retrieving specific records within the table and ensures data integrity by enforcing entity uniqueness and preventing duplicate entries.
SQL (Structured Query Language):

SQL is a standardized programming language used for managing and manipulating relational databases. It provides a set of commands, statements, and syntax rules for performing various operations on databases, such as querying data, inserting, updating, and deleting records, creating and modifying database structures (e.g., tables, indexes), and defining access controls and permissions.
Query:

A query is a request or command written in SQL that is used to retrieve, manipulate, or perform operations on data stored in a database. Queries are used to extract specific information from one or more database tables based on specified criteria or conditions, such as filtering, sorting, grouping, joining, or aggregating data.
Index:

An index is a data structure used in a database to improve the speed and efficiency of data retrieval operations, such as searching, sorting, and accessing records. It provides a quick lookup mechanism by organizing and storing key values from one or more database columns in a structured format, allowing for faster access to data based on specific criteria.
Normalization:

Normalization is the process of organizing and structuring data within a relational database to minimize redundancy, dependency, and anomalies, and to ensure data integrity and efficiency. It involves decomposing larger tables into smaller, more manageable tables and establishing relationships between them through the use of keys (e.g., primary keys, foreign keys) to reduce data duplication and improve database performance.
Database Management System (DBMS):

A Database Management System (DBMS) is a software application or system that facilitates the creation, management, organization, storage, retrieval, and manipulation of data within a database environment. It provides a set of tools, utilities, and interfaces for users and applications to interact with databases, perform database operations, and ensure data consistency, security, and integrity. Popular examples of DBMS include MySQL, PostgreSQL, Oracle Database, Microsoft SQL Server, and MongoDB.
2.1.1. Purpose of a Primary Key:

The primary key in a database table serves the fundamental purpose of uniquely identifying each record or row within the table. It ensures that each row has a unique identifier, which distinguishes it from all other rows in the table. The primary key enforces entity integrity and guarantees the uniqueness and accuracy of data within the table.

Example:
Consider a database table named "Employees" with columns such as "EmployeeID," "FirstName," "LastName," and "Email." In this table, the "EmployeeID" column can serve as the primary key. Each employee record will have a distinct EmployeeID value, ensuring that no two employees share the same identifier. For example:

EmployeeID	FirstName	LastName	Email
1	John	Smith	john@example.com
2	Emily	Johnson	emily@example.com
3	Michael	Williams	michael@example.com
In this example, the EmployeeID column uniquely identifies each employee record in the Employees table.

2.1.2. Difference between a DBMS and a Database:

Database:
A database refers to a structured collection of data organized and stored electronically in a way that facilitates efficient retrieval, management, and manipulation of data. It consists of tables, records, and fields containing related information. A database can be a physical or logical entity that stores data in a structured format.
Database Management System (DBMS):
A Database Management System (DBMS) is software that provides a set of tools, utilities, and interfaces for creating, managing, organizing, storing, retrieving, and manipulating data within a database environment. It acts as an intermediary between users or applications and the database, facilitating database operations and ensuring data consistency, security, and integrity. DBMS manages the storage, retrieval, and manipulation of data in the database, and it includes features such as data definition, data manipulation, data administration, and transaction management.
In essence, a database is the repository of data, while a DBMS is the software system used to manage and interact with the database.

2.1.3. Importance of Normalization in Database Design:

Normalization is essential in database design as it helps organize data efficiently, reduces redundancy, dependency, and anomalies, and ensures data integrity and consistency. By breaking down larger tables into smaller, more manageable tables and establishing relationships between them, normalization optimizes database structure and performance.

Example:
Consider a database for a library with two tables: "Books" and "Authors." Each book can have multiple authors, and each author can write multiple books. Instead of storing all book details in a single table, normalization allows us to divide the data into separate tables and establish relationships between them.

Books Table: (Primary key: BookID)
BookID	Title	ISBN	AuthorID
1	Database Design	1234567890	1
2	Python Programming	0987654321	2
Authors Table: (Primary key: AuthorID)
AuthorID	FirstName	LastName
1	John	Smith
2	Emily	Johnson
In this example, normalization separates book and author details into two tables and establishes a relationship between them using the AuthorID column. This approach minimizes redundancy and dependency, ensures data integrity, and allows for easier data maintenance and updates.
