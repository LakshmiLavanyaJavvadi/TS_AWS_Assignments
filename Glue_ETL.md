<ins>**Create IAM Role:**</ins>

* Navigate to the IAM (Identity and Access Management) console in the AWS Management Console.
* Click on "Roles" and then "Create role".
  
* <img width="956" alt="image" src="https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/4e2ef3e8-c914-4744-9c69-441049a09dd3">

* Choose the service that will use this role (e.g., AWS Glue,S3).
* Attach policies to the role that grant permissions for accessing S3 buckets, creating databases, running crawlers, etc.
  
* ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/8bb2dc0c-46ac-4127-8ff9-96ed9218371e)


<ins>**Create Policy:**</ins>

* Navigate to the IAM console and select "Policies".
* Click on "Create policy" and choose the JSON tab.
* Edit the JSON to specify the permissions needed, including the S3 ARN (Amazon Resource Name) for the buckets that will be accessed.
  
* ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/38588971-13cb-4a5d-a868-d6910e360793)

* Review and save the policy.

<ins>**Create Database:**</ins>

* In the AWS Glue console, click on "Databases" and then "Add database".
  
  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/5b0b8e3f-f89c-4f06-837c-5d4124a8736a)

* Enter a name for the database and configure settings as needed.
  
  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/f502d11b-8f74-4c72-8483-d7635f7d8adc)


<ins>**Create Crawler:**</ins>

* Navigate to the AWS Glue console.
* Click on "Crawlers" and then "Add crawler".
  
  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/1b907573-205c-4e55-ab31-deb1f3d08dd3)

* Specify the data store (e.g., S3 bucket) and provide access permissions
  
  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/db81bf06-43a2-4b2e-b1a3-e510f05d6757)

* Choose the database where the metadata will be stored.
  
  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/64cb19d1-d9b9-4046-b569-ea9e72c9b80d)

* Configure crawler schedule and output options.
  
  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/25cee4b2-2943-436f-a347-a0139dfe2b97)


<ins>**Run Crawler:**</ins>

* Go to the AWS Glue console and select the crawler you created.
* Click on "Run crawler" to start the crawling process.
  
  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/4d48638a-5cfd-4b86-8553-4de87d4f5274)

* The crawler will analyze the data in the specified data store and create metadata tables in the database.
  
  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/226979a2-0f15-47e8-a83e-d2f454220cce)


<ins>**Visual ETL:**</ins>

* Use the AWS Glue console to create a new job for Extract, Transform, Load (ETL) operations.
* Configure the job to read data from the crawled tables in the database.
* Use visual tools to design the ETL process, including joining data from multiple sources, applying transformations, and routing data conditionally.

  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/414e77e7-eb37-4855-b5fa-7a3c79c2374e)


<ins>**Run Visual ETL:**</ins>

* After designing the ETL job, run it to execute the defined transformations.

  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/b4912de4-caf0-4426-85f2-dda6b4a25e0f)

* The job will process the data according to the configured logic and generate output.

<ins>**Check Parquet Files:**</ins>

* Navigate to the S3 console to verify that the ETL job created the expected Parquet files.

  <img width="956" alt="image" src="https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/ab40a503-776c-4223-86b0-ba3e4bc002b9">

* These files contain the transformed data and are stored in the specified S3 buckets.

<ins>**Query Data in Data Catalog:**</ins>

* Access the AWS Glue Data Catalog or use tools like AWS Athena to query the metadata tables created by the crawler.
* Write SQL queries to retrieve and analyze the transformed data stored in the Data Catalog.

  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/8fcf554d-3748-4410-b352-37a941d2655e)


<ins>**Store Query Results in S3:**</ins>

* Use AWS Athena or another query service to execute SQL queries against the Data Catalog.

  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/075394f8-b556-452b-bc4c-95b082db3704)

* Configure the query to store the results in an S3 folder for further analysis or archival purposes.

  ![image](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/e4116045-3fbf-4c6c-aa80-a3205846d646)
