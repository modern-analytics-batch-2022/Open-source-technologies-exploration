# CASSANDRA

## Brief description

Apache Cassandra is a massively scalable open source NoSQL database. Cassandra is perfect for managing large amounts of structured, semi-structured, and unstructured data across multiple datacenters and the cloud. Cassandra delivers continuous availability, linear scalability, and operational simplicity across many commodity servers with no single point of failure, along with a powerful dynamic data model designed for maximum flexibility and fast response times.
The latest version of Apache Cassandra is 2.2.15.

## General information
* Creation year : 2008
* Website : "https://cassandra.apache.org/"
* Github repo :"gitbox.apache.org/repos/asf/cassandra.git"
* Community size : a minimal production server requires at least 2 cores, and at least 8GB of RAM. Typical production servers have 8 or more cores and at least 32GB of RAM.
* Founders : Avinash Lakshman and Prashant Malik.

## Main capabilities
- Distributed: Each node in the cluster has has same role. There's no question of failure & the data set is distributed across the cluster but one issue is there that is the master isn't present in each node to support request for service.
- Supports replication & Multi data center replication: Replication factor comes with best configurations in cassandra. Cassandra is designed to have a distributed system, for the deployment of large number of nodes for across multiple data centers and other key features too.
- Scalability: It is designed to r/w throughput, Increase gradually as new machines are added without interrupting other applications.
- Fault-tolerance: Data is automatically stored & replicated for fault-tolerance. If a node Fails, then it is replaced within no time.
- MapReduce Support: It supports Hadoop integration with MapReduce support.Apache Hive & Apache Pig is also supported.
- Query Language: Cassandra has introduced the CQL (Cassandra Query Language). Its a simple interface for accessing the Cassandra.

## Available connectors / integrations

Apache Drill
* Cassandra Storage Plugin: Drill's Cassandra storage plugin allows you to execute SQL queries against Cassandra tables.

Apache Flink
* Flink Sink Connector: This connector provides sinks that writes data into a Apache Cassandra database.

Apache Kafka
* Confluent Connect Cassandra: The Confluent Cassandra Sink Connector is used to move messages from Kafka into Apache Cassandra.

* DataStax Sink Connector:: The DataStax Apache Kafka Connector automatically takes records from Kafka topics and writes them to a DataStax Enterprise or Apache Cassandra database. This sink connector is deployed in the Kafka Connect framework and removes the need to build a custom solution to move data between these two systems.

* Lenses Sink Connector: The Cassandra Sink allows you to write events from Kafka to Cassandra. The connector converts the value from the Kafka Connect SinkRecords to JSON and uses Cassandra's JSON insert functionality to insert the rows. The task expects pre-created tables in Cassandra.

* Lenses Source Connector: Kafka Connect Cassandra is a Source Connector for reading data from Cassandra and writing to Kafka.

* Stream-Reactor: Lenses offers SQL (for data browsing and Kafka Streams), Kafka Connect connector management, cluster monitoring, and more.

Apache Pulsar
* Pulsar Sink Connector Cassandra Connector: The Pulsar Cassandra Sink connector is used to write messages to a Cassandra Cluster.

Apache Spark
* DataStax Spark Cassandra Connector: This library lets you expose Cassandra tables as Spark RDDs and Datasets/DataFrames, write Spark RDDs and Datasets/DataFrames to Cassandra tables, and execute arbitrary CQL queries in your Spark applications.

Presto
* Presto: The Cassandra connector allows querying data stored in Cassandra.

## Ways to deploy it :

The following are some key resources and information related to deploying Cassandra in the cloud or within your own private data center.
Cassandra and Multi-Data Center Clusters
One of the strongest features of Cassandra is its native support for the concept of multiple logical data centers within a cluster. Multi-data center clusters allow Cassandra to support several different scenarios. While at a high level, creating additional data centers in Cassandra is fairly straightforward, but in cross-region and cross-provider scenarios, you would need to dig deeper. Our CPO, Ben Slater,  helps you to learn how Instaclustr has made Multi-Data center clusters easy.
We conducted benchmarking for multi-data center Apache Spark and Apache Cassandra. The aim of this benchmark study was to compare performances between one-data-center settings where Spark and Cassandra are collocated, versus two-data-center settings where Spark is running on the second data center.

## Reviews
### Good reviews
- It's open-source
- It follows peer-to-peer architecture rather than master-slave architecture, so there isn't a single point of failure
- Cassandra can be easily scaled down or up
- It features data replication, so it's fault-tolerant and has high availability
- It's a high-performance database manager that easily handles massive amounts of data
- It's schema-free (or, schema-optional), so you can create your columns within the rows, and there is no need to show all the columns required to run the application
- It supports hybrid cloud environments since Cassandra was designed as a distributed system to deploy many nodes across many data centers

### Bad reviews
- It doesn't support ACID and relational data properties, because it handles large amounts of data and many requests, transactions slow down, meaning you get latency issues
- Data is modeled around queries and not structure, resulting in the same information stored multiple times
- Since Cassandra stores vast amounts of data, you may experience JVM memory management issues
- It offers no join or subquery support
- Cassandra doesn't support aggregates
- Cassandra was optimized from the start for fast writes, reading got the short end of the stick, so it tends to be slower
- Finally, it lacks official documentation from Apache, so you need to look for it among third-party companies

## Roadmap 4.0
CASSANDRA-9425: make node-local schema fully immutable.
CASSANDRA-12229: move streaming to non-blocking IO and netty.
CASSANDRA-9143: fix consistency of incrementally repaired data across replicas.
CASSANDRA-14556: fatser streaming of SSTables using ZeroCopy APIs.
CASSANDRA-7396: support for selecting map values and set elements.
CASSANDRA-7461: add support for arithmetic operators.
CASSANDRA-11936: add support for + and - operations on dates(CASSANDRA-11873 add duration type).
CASSANDRA-7622: virtual tables.
CASSANDRA-13289: ideal consistency level.
CASSANDRA-14404: Transient replica & Cheap Quorum.


