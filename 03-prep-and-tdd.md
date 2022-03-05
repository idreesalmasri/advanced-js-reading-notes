# Data Modeling Concepts.
create diagrams of the database tables and their relationships.  These may be done during the design process, as  your data modeling, or once the database is created, in order to document the tables’ dependencies.
* There are many types of modeling software you can use to create models, such as MySql Workbench.
### Data Modeling – Table Elements
* The Table Name, which is located at the top of the table.
* The Primary Keys.  Remember the primary keys uniquely identify each row in a table.  A table typically has one primary key, but can have more.  When the key has more than one column, it is called a compound key.
* Table Columns – There can be one or more table columns.  To keep the diagrams simple, I don’t show the data types.  I may introduce those later when we focus on more comprehensive modeling.
* Foreign Key – This is a column or set of columns which match a primary key in another table.
# SQL vs NoSQL Database Differences
## SQL
* SQL databases are primarily called as Relational Databases (RDBMS);
* SQL databases are table based databases ,This means that SQL databases represent data in form of tables which consists of n number of rows of data.
* SQL databases are vertically scalable, its scaled by increasing the horse-power of the hardware.
* use SQL ( structured query language ) for defining and manipulating the data.
* examples: MySql, Oracle, Sqlite, Postgres and MS-SQL.
* SQL databases are good fit for the complex query intensive environment.
* SQL databases are best fit for heavy duty transactional type applications, as it is more stable.
* QL databases emphasizes on ACID properties ( Atomicity, Consistency, Isolation and Durability).
## NoSQL
* NoSQL database are primarily called as non-relational or distributed database.
* NoSQL databases are document based, key-value pairs, graph databases or wide-column stores.which do not have standard schema definitions which it needs to adhered to, it have dynamic schema for unstructured data.
*  NoSQL databases are horizontally scalable, its scaled by increasing the databases servers in the pool of resources to reduce the load.
* Unstructured Query Language .
* examples: MongoDB, BigTable, Redis, RavenDb.
* NoSQL databases are not good fit for complex queries.
* NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data).
* NoSQL database follows the Brewers CAP theorem ( Consistency, Availability and Partition tolerance ).


# Review, Research, and Discussion
Name 3 advantages to Test Driven Development:
* THE SOFTWARE DESIGN BECOMES MODULAR
* THE CODE IS EASIER TO MAINTAIN
* CODE REFACTORING GOES MORE SMOOTHLY


What is one downside of Test Driven Development?
The tests are dependent on external dependencies. So they cannot maintain themselves.


What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
ES5 function constructors create objects along with inheritance property. 
ES6 class constructors creates objects by adding function to their prototypes (Blueprint).

[Home](./README.md)<br>