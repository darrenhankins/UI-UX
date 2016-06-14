Tuesday, June 14, 2016
### An Object-Oriented Approach to Programming Logic and Design
#### Programming Logic and Design
###### Lesson 6
###### Understanding Databases

##### Understanding Relational Database Concepts
- Data Anomalies
  - Insert anomaly
  - Delete anomaly
  - Update anomaly

##### Understanding Databases Query Methods

##### Understanding Database Connection Methods


`NOTE: Make sure to understand 'Data Normalization'`

`Data normalization`
  - `First Normal form` - none of columns should have multiple values in the cell
  - `Second Normal form` - first meet req. of first normal form, all non-key columns are functionally dependent on the entire primary key (pk)
    - primary key (pk)
    - foreign key (fk)
  - `Third Normal form` - meet the req. of the second normal form, requires that there is no functional dependency between non-key attributes

`Data de-normalization`
  - used in Data warehousing


  Structured Query Language (SQL)
  - used by most database systems to manage the information in their Databases
  - SQL is `declarative` in nature - you tell the database what needs to be done, and its the database's job to figure out how to do it
  - 2 ways to submit T-SQL and SQL Server:
    - Ad-hoc SQL statements (`SELECT`, `INSERT`, `UPDATE`, `DELETE`)
    - Stored procedures


  - Running SQL Queries
    - Visual Studio
    - C# application
    - SQL Query Analyzer
    - osql command prompt utility

Select statement is used to retrieve data from one or more database tables

```
SELECT ... (list_of_fields)
FROM ...  (list_of_tables)
WHERE ... (where_clause)
GROUP BY ... (group_by_clause)
HAVING ...  (having_clause)
ORDERBY ... (order_by_clause)
```

- Stored procedures
  - is a set of SQL statements that is stored in a database
  - benefits:
    - save complex sql statements for future execution
    - run faster than ad hoc queries

- Working a Flat file
  - Plain text or binary
  - StreamReader and StreamWriter classes allows you to manipulate text fields
  - Binary Reader and BinaryWriter to manipulate binary files

- XML is text based format for representing structured data
  - XmlReader, XmlWriter, XmlDocument

Working with DataSet
  - in-memory representation of relational data
