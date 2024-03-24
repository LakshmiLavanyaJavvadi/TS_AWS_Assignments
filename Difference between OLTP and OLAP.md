**OLTP**
* OLTP is characterized by many short on-line transactions (INSERT, UPDATE, DELETE).
These transactions involve inserting, updating, or deleting small amounts of data in real-time. OLTP systems are optimized for fast response times and are crucial for day-to-day operational tasks.
* OLTP queries are simple and easy to understand. These queries typically involve basic CRUD operations (Create, Read, Update, Delete) and are optimized for fast transaction processing.
* OLTP is widely used for small transaction.
* OLTP is highly normalized.
* OLTP is used for Backup religiously.
* OLTP usually uses schema used to store transnational databases is the entity model (usually 3NF).
* Performance of OLTP is comparably fast as compared to OLAP.

**OLAP** 
* OLAP is characterized by relatively low volume of transactions. OLAP systems focus on querying and analyzing large volumes of historical data to extract insights and support decision-making.
* OLAP Queries are often very complex and involve aggregations. Queries tend to be more complex and involve aggregating, grouping, filtering, and analyzing large datasets. Users often perform ad-hoc analysis and drill down into data to explore relationships and trends across multiple dimensions.
* OLAP applications are widely used by Data Mining techniques.
* OLAP is typically de-normalized.
* OLAP is used for regular backup.
* OLAP uses star model to store the data.
* Performance of OLAP is comparably low as compared to OLTP.
