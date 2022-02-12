 
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
