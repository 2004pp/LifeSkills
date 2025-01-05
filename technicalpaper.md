Apache Kafka

# What is Apache Kafka

It is a Open Source Distributed Platform for real-time data Streaming and Data Processing.

# What is the use of Apache Kafka?

To understand why we need to use Apache Kafka, consider the examples of Ola or Uber software. 
If a person books a ride then the driver will get the customer's address and the customer will get to know how far the driver is from there.
The customer will get the exact location of the driver. Every second, it needs to process the data. And it is not about one driver and customer. There are many. So it means that for every second, at least, there will be 30000 operations per second. These many operations our normal databases can't handle. But the location should be updated, which makes a good user experience and will benefit the company for a long time. 

This is not only for analyzing actions on commerce platforms. It will also generate a large amount of data per second.

To handle this large throughput we use Apache Kafka.

# Uses of Apache Kafka

  1)   Real-time Data Streaming
  2)   For monitoring & Analysis
  3)   Event Sourcing(Maintaining History of interactions on e-commerce website)
  4)   Data Pipelining (transferring large data between different Systems)
  5)   Data Integration

# Advantages / Features of Apache Kafka

* Large Throughput (no of operations on given time is more)
* low latency (less delay)
* Scalability
* Durability
* Fault Tolerance

Message -----> Data Handled by Apache Kafka

The message Has three parts:

1)Headers   ---> Contains metadata like topics and partitioning

2)Key  --- key for producers/organizations

3)Value  -->Actual data to deploy payload

# Components in Apache Tomcat

1) consumers

2) producers

3) Broker
  
4) Cluster

5) Zoo Keeper

6) Tokens

7) Partitions

# How Apache Kafka Works:


* Producer Sends the data to Kafka Broker. The browser will send the data to the Consumers. A cluster is nothing but a group of brokers. The broker  contains the token. A similar Type of Data Will 
  be Stored in  one Token. Tokens contain partitions. 

* When the Producer tries to push the data to Kafka then based on the Id/key it will store on partitions inside Tokens. To provide Fault Tolerance and Data Recovery same data  will be stored in the 
  two  brokers. If one clashes Another will be used.  

* Consumers pull data from the Partitions in the Tokens. And to keep track of at partition the consumer left. Assigning  partitioning for consumers. Scaling all these things will be managed by 
  zookeeper in the Kafka System. 

* Zookeeper is also responsible for Cluster management. Like if one cluster doesn't work. It will be reassigned. It will config metadata like about tokens and partitions. It is also responsible for 
  synchronization and coordination between clusters.
      
* Updating Offset. Offset is about the partition where the consumer left previously.


# Architecture of Apache Kafka

  ![image](https://github.com/user-attachments/assets/f2ac9480-d1be-46db-8c1d-5a801d5ff638)

# Interactions in Kafka

  1)Producer to  Kafka cluster

  2) Kafka Cluster to consumers

  3) Zoo keeper to Kafka cluster

# Kafka Provides Several APIs

  1) Producer API: Allows you to send streams of data to cluster

  2) consumer API: Allows you to read Streams of data from cluster

  3) Stream API: A Java Library to process real-time data.

  4) Connector API: For connecting with External Systems.

# References:

 *  https://www.geeksforgeeks.org/apache-kafka/

 *  https://www.youtube.com/watch?v=fE7clVFe4aU
























