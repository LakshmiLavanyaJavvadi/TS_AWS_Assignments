**Star Schema:** Star schema is the type of multidimensional model which is used for data warehouse. In star schema, The fact tables and the dimension tables are contained. In this schema fewer foreign-key join is used. This schema forms a star with fact table and dimension tables. 
* In a star schema, the fact table is at the center, surrounded by multiple dimension tables. Each dimension table is directly connected to the fact table through foreign key relationships.
* Star schemas are relatively simple and easy to understand. They have a denormalized structure, with dimension tables containing all relevant attributes for analysis.
* Star schemas typically offer better query performance, as they involve fewer joins compared to snowflake schemas. Queries can be executed more efficiently due to the simplified structure.
  
**Example:** A typical example of a star schema is a sales database, where the fact table contains sales transactions and dimension tables include products, customers, time, and locations.

**Snowflake Schema:** Snowflake Schema is also the type of multidimensional model which is used for data warehouse. In snowflake schema, The fact tables, dimension tables as well as sub dimension tables are contained. This schema forms a snowflake with fact tables, dimension tables as well as sub-dimension tables.
* In a snowflake schema, dimension tables are normalized into multiple related tables, forming a hierarchical or tree-like structure. Each dimension table may have one or more related tables representing sub-dimensions.
* Snowflake schemas are more normalized compared to star schemas, as they separate repeating groups of attributes into their own tables. This reduces data redundancy but increases the complexity of the schema.
* Snowflake schemas are more complex and require more joins to retrieve data compared to star schemas. Querying data from a snowflake schema may involve traversing multiple tables, which can impact query performance.

**Example:** An example of a snowflake schema might be a product hierarchy, where the product dimension is normalized into multiple tables representing product categories, subcategories, and individual products.
