# Iceberg Data Storage

Apache Iceberg is an open table format for huge analytic datasets. Iceberg adds tables to Presto and Spark that use a high-performance format that works just like a SQL table.
Iceberg is essentially a table format standard designed for massive analysis, which can provide high-performance reading, writing and metadata management capabilities for mainstream computing engines such as Presto and spark. Iceberg does not pay attention to the underlying storage (such as HDFS) and table structure (business definition). It provides an abstraction layer between the two and organizes data and metadata. 



![image](https://user-images.githubusercontent.com/95130613/153721376-48c5228d-41e9-4561-8a8f-13fd2729c999.png)


### General information

Creation year : Apple and Netflix started the Iceberg project around 2018.

Website : https://iceberg.apache.org/

Github repo : https://github.com/apache/iceberg

Community channel : https://apache-iceberg.slack.com/

Founders : Ryan Blue, ingénieur principal chez Netflix et président PMC du projet Apache Iceberg.
  

### Main capabilities  

Iceberg currently supports three file formats: Parquet, Avro, and ORC. files in HDFS and in S3 can be stored inline or column, which we will discuss in detail later. The features of Iceberg itself are summarized as follows. These capabilities are essential for building a real-time data warehouse with Iceberg.


![image](https://user-images.githubusercontent.com/95130613/153721472-40c469e4-69d6-4663-ba22-46421fd938cb.png)


•	Snapshot-based read-write separation and backfill

•	Stream-batch unified write and read

•	No forcing binding between the computing and storage engines

•	Multi-version ACID semantics and data

•	Table, schema, and partition change


### Available connectors / integrations  

Apache Iceberg is an open table format for huge analytic datasets. Iceberg adds tables to compute engines including Spark, Trino, PrestoDB, Flink and Hive using a high-performance table format that works just like a SQL table.


![image](https://user-images.githubusercontent.com/95130613/153721609-90188b35-22d3-4809-929c-e0db2955360e.png)


 #### Integrations:
 
 ##### •	AWS
 
 Iceberg provides integration with different AWS services through the iceberg-aws module. 
 
 ##### •	Nessie
 
Iceberg provides integration with Nessie through the iceberg-nessie module. This section describes how to use Iceberg with Nessie. Nessie provides several key features on top of Iceberg:
•	multi-table transactions
•	git-like operations (eg branches, tags, commits)
•	hive-like metastore capabilities

 ##### •	JDBC
 
 Iceberg supports using a table in a relational database to manage Iceberg tables through JDBC. The database that JDBC connects to must support atomic transaction to allow the JDBC catalog implementation to properly support atomic Iceberg table commits and read serializable isolation.
 
### Ways to deploy it :

##### Iceberg on Kubernetes

Kubernetes is responsible for application automation deployment and resource management scheduling, shielding the complexity of the underlying environment for the upper layer. Iceberg + hive Metastore + HDFS implements a real-time data Lake based on Hadoop ecology to provide data access and storage for big data applications. Spark, Flink and other computing engines run in kubernetes cluster in a native way, and resources are available and used immediately. After mixing with online business, it can greatly improve the utilization of cluster resources.

#### Architecture diagram

![image](https://user-images.githubusercontent.com/95130613/153721780-fbf7d57e-b71c-4d3c-912b-560239e2ed4f.png)


•	Resource layer: kubernetes provides resource management and control capabilities
•	Data layer: Iceberg provides access to data sets such as acid and table
•	Storage layer: HDFS provides data storage capability, hive Metastore manages iceberg table metadata, and PostgreSQL serves as the storage backend of hive Metastore
•	Computing layer: Spark native on kubernetes, which provides flow batch computing capability


### Reviews

#### 1.	Support to in place file formats

As we have already discussed Iceberg is not a file format but it’s a table format.
Having to use the Iceberg, doesn’t require you to change the file format if you are using ORC, Avro or Parquet.
It integrates well with the current file format and it adds a layer on top of these file formats.
Plus the Iceberg is built in a way where it can run on top of the current execution engines like Hive, Spark or Presto.

#### 2.	Schema evolutions

Iceberg does supports ADD, DROP, RENAME, UPDATE or REORDER of a column.
The schema evolution or changes would only effect the metadata. It means you are not required to change or rewrite the whole data again.

Note that map keys do not support adding or dropping struct fields that would change equality.

#### 3.	Atomic Operations

All the writes will always work at isolation without impacting the current read or the current schema in the metadata.
Readers will never be able to read the partially committed data.
Once the operation is fully succeeded the atomic operation will be committed and will be visible to the readers.

#### 4.	To get rid of directory and file listing

The traditional file format requires you to read the list of directories in case of partitioning and list all the files within the partition and based on the footer exclude the files which are not in the filter clause.
Though we are not in need of most of the partitions and fields within those partitions we end up listing the each and every-time for every query.
It’s a lot of listing.
Iceberg doesn't require a listing of the files. It maintains the data in the manifests.
We shall talk about it more in the architecture.

#### 5.	Altering the partitioning columns

The architecture we have defines years back will not be able to support all my future use cases.
Similarly in case of partitioning the data, the data distribution based on the column we have defined would need a change as the time progresses.
For eg. we may want to change the partitioning column from Month to date without having to rewrite the whole data.
Iceberg does support the different level of partitioning at the same schema.
  
 
 ![image](https://user-images.githubusercontent.com/95130613/153721877-a731c8f8-e5c1-4f5c-a23e-f4accdffab93.png)

#### 6.	Isolation between read and write

Iceberg maintains the snapshots of the files which changed as time progresses. This will support the READ and WRITE to occur parallel but in isolation.
Unless the new write is committed, this snapshot will not be available for read.
This will make sure your data and schema will not break or read the partial data.

#### 7.	Implicit partitioning

Defining the partitioning shouldn't be mandatory. As m requirement will change with the time. Having to know the partitioning at the run time will improve your query performance exponentially.
Iceberg just does that. Implicitly the partitioning column will be fetched and read.

#### 8.	Time travel

As e have already discussed the Iceberg supports the versioning. This makes the time travel possible if you are required to go back to a previous version as per your requirement.


### Roadmap



![image](https://user-images.githubusercontent.com/95130613/153721912-63f9e028-774f-48e8-80c3-0f9963556902.png)


The picture above shows Iceberg's Roadmap. It can be seen that Iceberg only released one version in 2019, but directly released three versions in 2020, and became the top project in version 0.9.0.


![image](https://user-images.githubusercontent.com/95130613/153721931-65f0a5ba-fb48-4f8e-a134-ab99148de137.png)

The above picture shows the Roadmap of Flink and Iceberg, which can be divided into 4 stages.

1)	The first stage is to establish a connection between Flink and Iceberg.
2)	The second stage is the scene where Iceberg replaces Hive. In this scenario, many companies have already started to go online to implement their own scenarios.
3)	The third stage is to solve more complex technical problems through Flink and Iceberg.
4)	The fourth stage is to change this set from a purely technical solution to a more complete product solution perspective.

### Reference

https://iceberg.apache.org/

https://www.datanami.com/2021/02/08/apache-iceberg-the-hub-of-an-emerging-data-service-ecosystem/#:~:text=Engineers%20at%20Apple%20and%20Netflix,and%20query%20massive%20data%20sets.

https://www.alibabacloud.com/blog/flink-%2B-iceberg-how-to-construct-a-whole-scenario-real-time-data-warehouse_597824

https://segmentfault.com/a/1190000040253675/en

https://developpaper.com/use-iceberg-on-kubernetes-to-build-a-new-generation-of-cloud-native-data-lake/


