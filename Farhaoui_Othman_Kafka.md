<p align="center">
    <img width="800" height="300" src="https://user-images.githubusercontent.com/78746917/154452425-d2806bb8-3965-41c9-8566-06b0867bdcfc.png"> 
</p>

## :clipboard: Description:
Apache Kafka is an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications. 
<p align="center">
    <img width="800" height="300" src="https://user-images.githubusercontent.com/78746917/154455255-70d8f43f-72ac-4b60-b8d0-90c7f10efe25.png"> 
</p>

## :bookmark: General informations:

**:hourglass_flowing_sand:creation year** : January 2011<br>
**:earth_africa:The website:** https://kafka.apache.org/<br>
**:octocat:Github repo:** https://github.com/confluentinc<br>
**:email:Community channel:** <br>
<ul>
  <li>:computer_mouse: google Group : https://groups.google.com/g/confluent-platform <br></li>
  <li> :computer_mouse:Docker Hub : https://hub.docker.com/u/confluentinc/<br></li>
  <li>:computer_mouse: LinkedIn: https://www.linkedin.com/products/the-apache-software-foundation-apache-kafka/<br></li>
  <li>:computer_mouse: Twitter @confluentinc :https://www.linkedin.com/company/confluent/<br></li>
  <li>:computer_mouse: Instagram : https://www.instagram.com/confluent_inc/<br></li>
  <li>:computer_mouse: Youtube channel: https://www.youtube.com/channel/UCmZz-Gj3caLLzEWBtbYUXaA<br></li>
</ul>
  
:technologist:**Community size:**
 More than 80% of all Fortune 100 companies trust, and use Kafka.
  <p align="center">
    <img width="600" height="100" src="https://user-images.githubusercontent.com/78746917/154460110-59182679-e1b3-4f5f-9728-719da8da4881.jpg"> 
</p>

:hammer_and_pick:**Founders:**<br>
<b> Jay Kreps, Neha Narkhede, Jun Rao</b> and the team at<b> Confluent</b> are responsible for one of the most important trends in technology today.
<p align="center">
    <img width="800" height="400" src="https://user-images.githubusercontent.com/78746917/154461903-1f8083fa-4dc7-472a-b7e0-018d29e45c44.jpg"> 
</p>

## :zap:Main capabilities

:point_right:Scalability:
Apache Kafka can handle scalability in all the four dimensions, i.e. event producers, event processors, event consumers and event connectors. In other words, Kafka scales easily without downtime.<br>
:point_right:High-Volume:
Kafka can work with the huge volume of data streams, easily.<br>
:point_right:Data Transformations:
Kafka offers provision for deriving new data streams using the data streams from producers.<br>
:point_right:Reliability:
Since Kafka is distributed, partitioned, replicated and fault tolerant, it is very Reliable.<br>
:point_right:Durability:
It is durable because Kafka uses Distributed commit log, that means messages persists on disk as fast as possible.<br>
:point_right:Performance:
For both publishing and subscribing messages, Kafka has high throughput. Even if many TB of messages is stored, it maintains stable performance.<br>
:point_right:Zero data loss:
Kafka is very fast and guarantees zero data loss.<br>
:point_right:Extensibility:
There are as many ways by which applications can plug in and make use of  Kafka. In addition, offers ways by which to write new connectors as needed.<br>
![cap](https://user-images.githubusercontent.com/78746917/154520848-979a13c3-0564-4aff-ad55-6b8e6fcdc86b.jpg)

## :electric_plug: Available connectors / integrations:
 <p align="center">
    <img width="600" height="400" src="https://user-images.githubusercontent.com/78746917/154521292-07325282-0a80-400d-a8f4-ba92cc6c289d.png"> 
</p>
<b>Source connectors:</b>enable the integration of data from an existing technology into an Apache Kafka topic. Use connectors to copy data between Apache Kafka® and other systems that you want to pull data from or push data to, The following is the list of available source connectors:
<ul>
<li>Couchbase</li>
<li>Official MongoDB preview</li>
<li>Debezium for MongoDB</li>
<li>Debezium for MySQL</li>
<li>Debezium for PostgreSQL</li>
<li>Debezium for SQL Server</li>
<li>Google Cloud Pub/Sub</li>
<li>Schema Source</li>
<li>Stream Reactor Cassandra</li>
  </ul>
  
![0_BL5luf8JGjn459u6](https://user-images.githubusercontent.com/78746917/154477200-0dec951c-6398-49c9-b81c-f26e1a3ccd17.png)

<b>Sink connectors:</b> enable the integration of data from an existing Apache Kafka topic to a target technology. The following is the list of available sink connectors:
<ul>
<li>Aiven for Kafka GCS Sink Connector</li>
<li>Aiven for Kafka S3 Sink Connector</li>
<li>Confluent Amazon S3 Sink</li>
<li>Official MongoDB preview</li>
<li>Couchbase</li>
<li>Elasticsearch</li>
<li>Confluent Elasticsearch Sink</li>
<li>Google Cloud Pub/Sub</li>
<li>Google BigQuery</li>
<li>HTTP preview</li>
<li>Snowflake preview</li>
<li>Splunk</li>
<li>Stream Reactor Cassandra</li>
<li>Stream Reactor InfluxDB</li>
<li>Stream Reactor Mongo DB</li>
</ul>

![connecteur](https://user-images.githubusercontent.com/78746917/154479468-77e177fc-60f0-4ec8-b02d-166b3330ac63.png)

## :hammer_and_wrench:Ways to deploy it :

:computer:<b>On-prem:</b> on-premises environment, resources are deployed in-house and within an enterprise’s IT infrastructure. An enterprise is responsible for maintaining the solution and all its related processes.
Steps to deploy Kafka on-prem: 

```sh
1.	Install Java JDK 8 with Windows:
2.	Download Kafka
3.	Unzip Kafka Folder in Local System. Once the Java JDK is installed, Unzip the Kafka Folder in some local directory. ...
4.	Modify the Configuration for Kafka. ...
5.	Update the LOG Directory in the Config File.
```

*more details to deploy Kafka on-prems:* https://kafka.apache.org/quickstart<br>

:cloud:<b>PaaS / SaaS:</b>
- Platform as a service (PaaS) is a cloud computing model where a third-party provider delivers hardware and software tools to users over the internet. 
- Software-as-a-Service(SaaS) refers to the installation and delivery of software as a service, as opposed to the traditional on premise model of software deployment

> **Kafka on Kubernetes:**
Kubernetes is an open source container orchestration platform that automates many of the manual processes involved in deploying, managing, and scaling containerized applications.
<p align="center">
    <img width="800" height="300" src="https://user-images.githubusercontent.com/78746917/154486414-9d8aa642-2cb6-4589-bf86-4388bb11f81e.png"> 
</p>

```sh
    "steps to deploy Kafka on Kubernetes"
Step 1: Deploy Apache Zookeeper
Step 2: Deploy Apache Kafka
Step 3: Test Apache Kafka
Step 4: Scale Apache Kafka
```
> **Kafka on heroku:**
Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud.
<p align="center">
    <img width="800" height="300" src="https://user-images.githubusercontent.com/78746917/154486674-a7f90de6-b9cf-4ab7-b1bd-09cc5d39d12f.jpeg"> 
</p>

```sh
   "steps to deploy Kafka on heroku"
Step 1: Create a Heroku app
Step 2: Add and provision a Kafka plan
Step 3 :Create and manage topics
Step 4: Deploy your code to your app
Step 5: See your event flows
```

...
## :pushpin:Reviews
:heavy_check_mark:**Good reviews:**<br>
:+1:High availablility<br>
:+1:Highly scalable<br>
:+1:Highly performance<br>
:+1:Consistency<br>
:+1:parallelism<br>
:+1:good support from community<br>
:+1:Very good user base<br>
:+1:network partition tolerence<br>
:+1:The functionality of kafka is just so good, everything works fine and nothing breaks any time. also the distribution is really good<br>
:+1:The feature set is just amazing, it enables you to build resilient and fault tolerant applications with ease<br>
:+1:Fast queuing<br>
:+1:Easy to set up and configure<br>
:+1:Easy to add and remove queues<br>
:+1:Very scalable: easily configured to run on multiple nodes allowing for ease of parallelism (assuming your queues/topics don't have to be consumed in the exact same order the messages were delivered)<br>
:+1: It scales very well over large workloads and can handle extreme-scale deployments (eg. Linkedin with 300 billion user events each day).<br>
:+1:The same Kafka setup can be used as a messaging bus, storage system or a log aggregator making it easy to maintain as one system feeding multiple applications.<br>
:+1:It handles large amount of data simultaneously. Makes application scalable.<br>
:+1:	It is able to handle real time data pipeline.<br>
:+1:	Resistant to node failure within the cluster.<br>

:x:**Bad reviews:**
<br>
:thumbsdown:Really hard to deploy it, and maintain it. depends on a lot of things like zoopkeeper.<br>
:thumbsdown:It's not very easy to install on locally hosted cloud orchestration frameworks like Kubernetes and OpenShift, even though installation on Docker is as simple as running one command with a simple docker-compose file<br>
:thumbsdown:Brokers and consumer pattern reduces the performance.<br>
:thumbsdown:It is not a full solution so for an analytics use case, you will still need something like Tibco.<br>
:thumbsdown:It does not have a SQL based query engine out-of-the-box so building/using analytics on top can be a lot of work. It would be great to have something already baked into Kafka out-of-the-box.<br>
:thumbsdown: Doesn't work well with many small topics (on the order of thousands). There is a physical limit due to file handler usage on the number of topics Kafka can have before it grinds to a halt. This is not an issue for most people but it became an issue for us, as we need to have many, many topics and so we weren't able to fully migrate to Kafka except for a few of our big queues.<br>

## :clock1: Roadmap 
Starting with Apache Kafka 0.10.1.0, 
Time-based releases
- Oct 2016 - 0.10.1.0
- 0.10.1.1 (Dec 2016)
- 0.10.1.2 (question)
- Feb 2017 - 0.10.2.0
- 0.10.2.1 (April 2017)
- 0.10.2.2 (July 2018)
- Jun 2017 - 0.11.0.0
- 0.11.0.3 (July 2018)
- Oct 2017 - 1.0.0
- 1.0.1
- 1.0.2 (July 2018)
- Feb 2018 - 1.1.0
- 1.1.1 (July 2018)
- Jun 2018 - 2.0.0
- 2.0.1 (Oct 2018)
- Nov 2018 - 2.1.0
- 2.1.1 (Jan 2019)
- Mar 2019 - 2.2.0
- 2.2.1 (May 2019)
- 2.2.2 (Oct 2019)
- June 2019 - 2.3.0
- 2.3.1 (Sep 2019)
- Dec 2019 - 2.4.0
- 2.4.1 (March 2020)
- Mar 2020 - 2.5.0
- 2.5.1 (Aug 2020)
- June 2020 - 2.6.0
- 2.6.1 (Jan 2021)
- 2.6.2 (Apr 2021)
- 2.6.3 (Nov 2021)
- Nov 2020 - 2.7.0
- 2.7.1 (May 2021)
- 2.7.2 (Nov 2021)
- 2.8.0 (Apr 2021)
- 2.8.1 (Sep 2021)
- 3.0.0 (Sep 2021)
- 3.0.1 (March 2022)
- 3.1.0 (Jan 2022) 

Older releases
- Kafka 0.9.0.0 (Nov. 2015)
- Kafka 0.10.0.0 (Q2 2016)

















