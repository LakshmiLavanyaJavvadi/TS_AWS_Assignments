# TS_AWS_Assignments **Write about OLTP and OLAP**
<ins>**OLTP (Online Transaction Processing):**</ins>
* OLTP databases function as a "single source of storage" and are designed to handle many tiny transactions.
* OLTP systems are commonly used in day-to-day operations of businesses such as retail sales, banking transactions, order processing, and inventory management.
* Examples of OLTP databases include Oracle Database, SQL Server, MySQL, PostgreSQL, and MongoDB.

<ins>**Example:**</ins> A website for online movie ticket sales is an example of an OLTP system. If two people wish to reserve the same seat for the same film at the same time, 
the ticket will be awarded to the person who completes the transaction first. It's important to remember that OLTP systems are built for transactional priority rather than analytical data.

**Benefits:**
1. The primary advantage of utilizing OLTP services is their ability to execute queries quickly, allowing them to react to user actions instantly.
2. The user can read, write, and delete data quickly with the use of OLTP services.
3. OLTP ensures the consistency of data, any changes made by one user will reflect for all other users.
4. OLTP provides high levels of security by implementing various security features such as authentication, authorization and encryption to ensure that only authorized users can acess the data.
5. It is scalable and can handle increased number of users and transactions.

**Drawbacks:**
1. OLTP services is not fail-safe. If there is hardware failures, then online transactions gets affected.
2. OLTP systems are not meant for sophisticated analysis or reporting; rather, they are meant to manage operational tasks. They are not able to quickly compile and evaluate vast volumes of data.
3.  With many users accessing and modifying data concurrently, OLTP systems may experience issues with data integrity, such as duplicate or inconsistent data.

<ins>**OLAP (Online Analytical Processing):**</ins>
*  OLAP databases are typically larger (they process more data) and better suited for analytics, data mining, and fewer queries.
*  Any Datawarehouse system can be referred to as an OLAP system.
*  Examples of OLAP databases and tools include Microsoft Analysis Services, IBM Cognos, Oracle OLAP, SAP BusinessObjects, and Tableau.
  
<ins>**Example:**</ins> In order to track their business, many companies compare their sales from one month to the next. Here, the business compares the sales and stores the outcome in a different database at a different location. This business employs OLAP databases.

**Benefits**
* Keeping track of consistency and calculations is the primary advantage of utilizing OLAP services.
* OLAP creates a single platform on which we can store company analytics budgeting, analysis, and planning.
* We may simply implement security constraints to secure data when using the OLAP as a service.
* The unified picture of data from various sources that OLAP systems offer facilitates data access and analysis for business analysts.
* Because OLAP services offer a multidimensional view of the data, customers can slice and dice the data in a variety of ways, making complicated searches and data analysis possible.

**Drawbacks**
* The main issue with OLAP services is that because OLAP tools necessitate a complex modeling process, data handling is always the responsibility of IT professionals.
* The implementation and upkeep of OLAP systems can be highly costly, particularly when dealing with enormous datasets.
* Data availability could be delayed since analysis requires data to be extracted, converted, and put into the OLAP system.
* Write operations may be slower or less effective with OLAP services since they are designed for workloads that are heavy on reading.
