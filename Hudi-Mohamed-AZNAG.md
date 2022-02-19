<p align="center">
    <img width="800" height="300" src="https://user-images.githubusercontent.com/98332222/154753446-17c82ddd-7014-4dd6-a6d7-5931a1933df2.png">
</p>

## Brief Description:<br>
Apache Hudi, which stands for Hadoop Upserts Deletes Incrementals, is an open-source framework developed by Uber in 2016 that manages the storage of large datasets on distributed file systems, such as cloud stores, HDFS, or any other Hadoop FileSystem compatible storage. It enables atomicity, consistency, isolation, and durability (ACID) transactions in a data lake.
<p align="center">
    <img width="800" height="300" src="https://user-images.githubusercontent.com/98332222/154754502-57282974-83d4-4c00-894a-678e4b981321.jpg">
</p>

## :bookmark: General informations:
**:hourglass_flowing_sand:creation year** :2016<br>
**:earth_africa:The website:** https://hudi.incubator.apache.org/<br>
**:octocat:Github repo:** https://github.com/apache/hudi<br>
**:email:Community channel:** 
https://app.slack.com/client/T4D7BR6T1<br>
**:floppy_disk:Communiy size:** 
1599<br>
:hammer_and_pick:**Founders:**<br>
a group of engineers including **Vinoth Chandar**<br>
## :zap:Main capabilities
:star: Upserts, Deletes with fast, pluggable indexing.<br>
:star: Transactions, Rollbacks, Concurrency Control.<br>
:star: Automatic file sizing, data clustering, compactions, cleaning.<br>
:star: Built-in metadata tracking for scalable storage access.<br>
:star: Incremental queries, Record level change streams.<br>
:star: SQL Read/Writes from Spark, Presto, Trino, Hive & more.<br>
:star: Streaming ingestion, Built-in CDC sources & tools.<br>
:star: Backwards compatible schema evolution and enforcement.<br>

## :electric_plug: Available connectors / integrations:
- Hudi interacts with lake storage using the Hadoop FileSystem API.
- Hudi interacts with Amazon EMR with Spark Data Source API.
- Hudi Flink SQL source/sink connectors, providing ability to define record keys, pick out the write operation, specify how to merge records, enable/disable asynchronous compaction or choosing query type to read.
- The AWS Glue Connector for Apache Hudi simplifies the process to create and update Apache Hudi tables from AWS Glue. This connector can be used for both Copy on Write (COW) and Merge on Read (MOR) storage types.

Apache Hudi integrates with:
- Alluxio
- Amazon Athena
- Amazon Redshift
- Apache Cassandra
- Apache Hive
- Apache Kafka
- Apache Spark
- Azure Data Lake
- Apache Flink
- Hadoop
- MySQL
- PostgreSQL
- Presto. 

## :hammer_and_wrench:Ways to deploy it :
### System Requirements : SaaS
All in all, Hudi deploys with no long running servers or additional infrastructure cost to your data lake. In fact, Hudi pioneered this model of building a transactional distributed storage layer using existing infrastructure and its heartening to see other systems adopting similar approaches as well. Hudi writing is done via Spark jobs (DeltaStreamer or custom Spark datasource jobs), deployed per standard Apache Spark recommendations. Querying Hudi tables happens via libraries installed into Apache Hive, Apache Spark or PrestoDB and hence no additional infrastructure is necessary.

A typical Hudi data ingestion can be achieved in 2 modes. In a single run mode, Hudi ingestion reads next batch of data, ingest them to Hudi table and exits. In continuous mode, Hudi ingestion runs as a long-running service executing ingestion in a loop.
With Merge_On_Read Table, Hudi ingestion needs to also take care of compacting delta files. Again, compaction can be performed in an asynchronous-mode by letting compaction run concurrently with ingestion or in a serial fashion with one after another.

## :pushpin:Reviews
:+1:**Good reviews:**<br>
- Apache Hudi works with these users and organization types: Mid Size Business, Small Business, Enterprise, Freelance, Nonprofit, and Government.
- Apache Hudi supports these languages: English.
- Apache Hudi offers support via online.

:thumbsdown:**Bad reviews:**
<br>

since it is a new technology in the market, there is no bad review.
## :clock1: Roadmap 

### This Roadmap include: 
Hudi community strives to deliver major releases every 2-3 months, while offering minor releases every month! 
### H1 2022 Releases
Next minor release : 0.10.1 (Jan 2022) Next major release : 0.11.0 (Feb 2022)

- in Feb 2022: release 0.11.0
- in apr 2022: release 0.12.0
- in Summer 2022: release 1.0.0

### Transactions/Database Layer

  ![3](https://user-images.githubusercontent.com/98332222/154760963-5f56f662-f53d-4bda-afed-459652c3a1a4.png)


### Execution Engine Integration

![4](https://user-images.githubusercontent.com/98332222/154761458-fcb035b6-5bd8-4dec-8b6a-2b1cfafbe0e7.png)

### Platform Services

![5](https://user-images.githubusercontent.com/98332222/154761955-10efd8c4-b19b-4976-b166-cf51fb358c8d.png)

## REFERENCES:
- https://hudi.apache.org/docs/0.10.0/overview/
- https://medium.com/slalom-build/data-lakehouse-building-the-next-generation-of-data-lakes-using-apache-hudi-41550f62f5f
- https://hudi.apache.org/docs/deployment/
