**Dimension vs Fact Table**
* Dimension tables provide the context and descriptive attributes for analyzing quantitative measures stored in fact tables. Dimension tables contain the "who," "what," "where," and "when" of the data, while fact tables contain the "how much" or "how many." Together, dimension tables and fact tables form the foundation of dimensional modeling, which is widely used in data warehousing and business intelligence to support analytical reporting and decision-making.
**Fact Table**
* Fact table contains the measuring of the attributes of a dimension table.
* In fact table, There is less attributes than dimension table.
* In fact table, There is more records than dimension table.
* Fact table forms a vertical table.
* The attribute format of fact table is in numerical format and text format.
* It comes after dimension table.
* The number of fact table is less than dimension table in a schema
* It is used for analysis purpose and decision making.
**Dimension Table**
* Dimension table contains the attributes on that truth table calculates the metric.
* While in dimension table, There is more attributes than fact table.
* While in dimension table, There is less records than fact table.
* While dimension table forms a horizontal table.
* While the attribute format of dimension table is in text format.
* While it comes before fact table.
* While the number of dimension is more than fact table in a schema.
* While the main task of dimension table is to store the information about a business and its process

**Types of Dimensions**

**Slowly Changing Dimensions–** Dimension attributes that change slowly over a period of time rather than changing regularly is grouped as SCDs.  Attributes like name, address can change but not too often.

These attributes can change over a period of time and that will get combined as a slowly changing dimension. Consider an example where a person is changing from one city to another. Now there are 3 ways to change the address;

Type 1  is to over write the old value, Type 2 is to add a new row and Type 3 is to create a new column.

**Type 1**
The advantage of type 1 is that it is very easy to follow and it results  in huge space savings and hence cost savings. The disadvantage is that no history is maintained.

**Type 2**
The advantage of type 2 is that the complete history is maintained. The only disadvantage lies in the huge space allocation because the entire history right from the start has to be maintained.

**Type 3**
The best approach could be to add a new column where you add two new columns. In this case keeping a tracking of the history becomes very easy.











