# Data Engineering and AWS-Projects

###### You can find my AWS projects along with their architectures and a step-by-step explanation of my reasoning behind them. I want to clarify that these projects were developed after extensive research and following guides. I have added detailed notes and explanations to aid my own learning.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------



[Title: Real-Time Stock Market Data Engineering using Apache Kafka and AWS](https://github.com/Aff1nity/AWS-Projects/tree/main/Real-Time%20Stock%20Market%20Data%20Engineering%20using%20Apache%20Kafka%20and%20AWS)

Summary: In this project, we set up an end-to-end data engineering pipeline to collect and process real-time stock market data using Apache Kafka and AWS services such as Glue, Athena, and S3. We created a Kafka topic, produced and consumed data using Python, and stored the data in an S3 bucket. Then, we used Glue Crawler to crawl and create a table in Athena for querying and analysis. The main aim of this project was to learn how to use Kafka and AWS services to build a real-time data processing pipeline for stock market data.

[Extended Explanation](https://github.com/Aff1nity/AWS-Projects/blob/main/Real-Time%20Stock%20Market%20Data%20Engineering%20using%20Apache%20Kafka%20and%20AWS/Stock%20Market%20Project.pdf)

**Architecture**
![Architecture](https://github.com/Aff1nity/AWS-Projects/blob/main/Real-Time%20Stock%20Market%20Data%20Engineering%20using%20Apache%20Kafka%20and%20AWS/Stock%20Market%20Project.png)

Services Used:
```
1.Apache Kafka
2.Amazon Elastic Compute Cloud (EC2)
3.Amazon Simple Storage Service (S3)
4.Amazon Glue
5.Amazon Athena
6.Amazon Identity and Access Management (IAM
7.Python programming language
```

**Possible improvements**

**Security**: One way to enhance the security of this project would be to use a VPN to connect to the EC2 instance running Kafka. This would provide an extra layer of security by encrypting the traffic between the client and server.

**Scaling**: While this project focuses on a single EC2 instance running Kafka, it may be necessary to scale up as the project grows. One way to handle this would be to use an auto-scaling group to manage a fleet of EC2 instances running Kafka. This would help ensure that the service remains highly available and can handle increased traffic.

**Monitoring**: It's important to monitor the health and performance of the Kafka cluster, and to be alerted to any issues that arise. This can be accomplished by using a tool like CloudWatch to monitor the EC2 instance and Kafka metrics, as well as using alarms to alert you to any issues.

**Backup and Disaster Recovery**: It's important to have a backup and disaster recovery plan in place to ensure the availability of the data in the event of an outage. One way to accomplish this would be to use EBS snapshots to back up the EC2 instance, and to use a multi-AZ deployment to provide automatic failover in the event of an outage.


------------------------------------------------------------------------------------------------------------------------------------------------------------------------

[Title: Simple Twitter data Pipeline using Airflow()
