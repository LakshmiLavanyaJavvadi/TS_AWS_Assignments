![Blank diagram (1)](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/d5a3d4cf-08a4-466d-8e50-95406a27af57)

<ins>**Data Ingestion Process:**</ins>

**Local Machine / Source:**
* Data originates from the local machine or source system.

**Amazon S3:**

* Files are uploaded from the local machine to an Amazon S3 bucket.
* S3 serves as the storage for the data to be ingested.

**IAM Service Role:**
* An IAM service role is created with the necessary permissions for AWS Glue to access the S3 bucket.
* The IAM service role is configured with an access policy granting Glue the necessary permissions to read data from the S3 bucket.

**Glue Crawler:**

* A Glue crawler is created to access the S3 bucket and crawl the files to infer the schema and metadata.
* The Glue crawler automatically identifies the data format, structure, and schema.
* It creates metadata tables in the Glue Data Catalog based on the crawled data.

**AWS Glue:**

* AWS Glue is a fully managed extract, transform, and load (ETL) service that simplifies the process of preparing and loading data for analysis.
* Glue utilizes the metadata tables created by the Glue crawler to facilitate data transformation and processing.
* Glue jobs can be created to perform ETL operations on the ingested data, such as data cleansing, transformation, and loading into other data stores or analytics platforms.
  
