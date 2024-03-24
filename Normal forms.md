**Normalization**
* Redundancy in a relation or collection of relations is minimized through the process of normalization. Anomalies related to insertion, deletion, and updates may result from relation redundancy. Thus, it aids in reducing relationship redundancy. In database tables, normal forms are used to decrease or eliminate redundancy.
* The normalization process follows a series of rules known as normal forms. There are several normal forms, each building upon the previous one, with the ultimate goal of improving data integrity and reducing anomalies during data manipulation.

**First Normal Form (1NF):**
* The first normal form requires that each column in a table contains atomic values, meaning values cannot be further divided into smaller pieces.
* Each attribute must have a single value for each row. There should be no repeating groups or arrays of values within a single attribute or cell.

<ins>**Example:**</ins> If you have a table for customer orders, each order should have its own row, and each attribute such as order ID, customer ID, product ID, and quantity should contain only atomic values.

**Second Normal Form (2NF):**
* 2NF eliminates redundant data by requiring that each non-key attribute be dependent on the primary key. This means that each column should be directly related to the primary key, and not to other columns.

<ins>**Example:**</ins> If you have a table with a composite primary key (e.g., Order ID and Product ID), attributes like Product Name and Product Price should depend on both Order ID and Product ID, not just one of them.

**Third Normal Form (3NF):**
* 3NF builds on 2NF by requiring that all non-key attributes are independent of each other. This means that each column should be directly related to the primary key, and not to any other columns in the same table.

<ins>**Example:**</ins>If you have a table with attributes like Employee ID, Department ID, and Department Name, where Department Name depends only on Department ID, you need to remove Department Name from this table and create a separate table where Department ID is the primary key, and Department Name is the dependent attribute.

**Boyce-Codd Normal Form (BCNF):**
* BCNF is a stricter form of 3NF that ensures that each determinant in a table is a candidate key. In other words, BCNF ensures that each non-key attribute is dependent only on the candidate key.

**Fourth Normal Form (4NF):**
* 4NF is a further refinement of BCNF that ensures that a table does not contain any multi-valued dependencies.

<ins>**Example:**</ins> If you have a table representing courses and instructors, where an instructor can teach multiple courses and a course can have multiple instructors, you need to break this into two separate tables to achieve 4NF.

**Fifth Normal Form (5NF):**
* 5NF is the highest level of normalization and involves decomposing a table into smaller tables to remove data redundancy and improve data integrity.

<ins>**Example:**</ins> In a table with multiple candidate keys, attributes that depend on the combination of these keys rather than just the primary key need to be separated into their own table to achieve 5NF.
