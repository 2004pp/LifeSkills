Apache Kafka

# What is Apache Kafka

It is a Open Source Distributed Platform for real time data Streaming and Data Processing.

# What is the use of Apache kafka.

To understand why we need to use Apache Kafka, lets consider with an example of ola or uber software. 
If a person book a ride then the driver will get customer address and customer will get to know how far the driver is from there.
And customer will get exact location of customer. Every second it needs to process the data.And it is not about one driver and customer. There are many . so it means for every sec atleast there will  be 30000 operations per sec. These many operations our normal databases cant handle. But location should be updated. Which makes good user experience and it will benifits the company after long time. 

And not only this for analysing the actions on e-commerence platforms. It will also generate a large data per one sec.

To handle this large throughput we use Apache Kafka.

# Uses of Apache Kafka

  1)   Real time Data Streaming
  2)   For monitoring & Analysis
  3)   Event Sourcing(Maintaining History of interactions on e-commerce website)
  4)   Data Pipelining (transfering large data between different Systems)
  5)   Data Integration

# Advantages / Features of Apache Kafka

1)Large Throughput (no of operations on given time is more)
2)low latency (less delay)
3)Scalability
4)Durability
5)Fault Tolerance

Message -----> Data Handled by Apache Kafka

Message Has three parts:

1)Headers   ---> Contains metadata like topics and partitioning

2)Key  --- key for producers / organizations

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


  ==> Producer Sends the data to Kafka Broker. Browser will sends the data to the Consumers. Cluster is nothing but group of broker. Broker  contains the token. Similar Type of Data Will be Stored in  
       one Token. Tokens contains partitions. 

  ==> When the Producer try to push the data to Kafka then based on Id /key it will store on partitions inside Tokens. To provide Fault Tolerance and Data Recovery same data  will be stored in the two 
      brokers. If one clashes Another will be used .  

  ==> Consumers pull data from the Partitions in the Tokens.And to keep track of at partition the consumer left. Assigning  partitioning for consumers. Scaling all these things will be managed by 
      zookeeper in the Kafka System. 

  ==> Zookeeper is also responsible for Cluster management. Like if one cluster doesn't work. It will reassign. It will config meta data like about tokens and partitions. It is also responsible for 
      synchronization and coordination between clusters.
      
  ==> Updating Offset. Offset is about the partition where the consumer left previously.


# Architecture of Apache Kafka

  ![image](https://github.com/user-attachments/assets/f2ac9480-d1be-46db-8c1d-5a801d5ff638)

# Interactions in Kafka

  1)Producer to  Kafka cluster

  2) kafka Cluster to consumers

  3) Zoo keeper to Kafka cluster

# Kafka Provides Several API's

  1) Producer API: Allows you to send streams of data to cluster

  2) consumer API : Allows you to read Streams of data from cluster

  3) Stream API: A java Library to process real time data.

  4) Connecter API : For connecting with External Systems.

























