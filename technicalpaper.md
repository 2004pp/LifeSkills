Apache Kafka

# What is Apache Kafka

It is a Open Source Distributed Platform for real time data Streaming and Data Processing.

# What is the use of Apache kafka.

To understand why we need to use Apache Kafka, lets consider with an example of ola or uber software. 
If a person book a ride then the driver will get customer address and customer will get to know how far the driver is from there.
And customer will get exact location of customer. Every second it needs to process the data.And it is not about one driver and customer. There are many . so it means for every sec atleast there will  be 30000 operations per sec. These many operations our normal databases cant handle. But location should be updated. Which makes good user experience and it will benifits the company after long time. 

And not only this for analysing the actions on e-commerence platforms. It will also generate a large data per one sec.

To handle this large throughput we use Apache Kafka.

#Uses of Apache Kafka

  1)   Real time Data Streaming
  2)   For monitoring & Analysis
  3)   Event Sourcing(Maintaining History of interactions on e-commerce website)
  4)   Data Pipelining (transfering large data between different Systems)
  5)   Data Integration

#Advantages / Features of Apache Kafka

1)Large Throughput (no of operations on given time is more)
2)low latency (less delay)
3)Scalability
4)Durability
5)Fault Tolerance

#Components In Apache Tomcat

Message -----> Data Handled by Apache Kafka

Message Has three parts:

1)Headers   ---> Contains metadata like topics and partitioning

2)Key  --- key for producers / organizations

3)Value  -->Actual data to deploy payload












