# Real Time Data Streaming using Apache Nifi AWS Snowpipe Stream Task

## **Overview** 
This project demonstrates a robust real-time data streaming pipeline utilizing **Apache NiFi** 
for data ingestion and transformation, **AWS EC2** for processing, and **Snowflake** for data warehousing. 


## Project Architecture
![End-To-End Project Architecture](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/Project_Architecture.png)



## Technologies Used
1. Programming Language - Python
2. Scripting Language - SQL
3. AWS
   - IAM( Identity and Access Management)
   - S3 ( Simple Storage Service)
   - EC2 
4. Snowflake : Cloud data warehouse for data storage and querying.

## Data Flow

1. Data Extraction: Ingest real-time data streams from various sources using Apache NiFi.
2. Data Processing: Utilize an EC2 instance for data transformation and processing.
3. Data Loading: Load cleaned and structured data into Snowflake for storage and analysis.
4. Data Analytics: Analyze and visualize the data using business intelligence tools connected to Snowflake.
5. Monitoring: Implement monitoring solutions to ensure the health and performance of the data pipeline.

## Scripts for project 
1. [Data Generation ](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/faker.ipynb)
2. [Table Creation ](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/1.%20Table%20Creation.sql)
3. [Data Loading in Table](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/2.%20Data%20Loading.sql)
4. [Slowly Changing Dimensions Handling Code 1](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/3.%20SCD%201.sql)
5. [Slowly Changing Dimensions Handling Code 2](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/4.%20SCD%202.sql)
6. [Necessary Commands](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/commands.txt)
7. [Docker Compose File Code](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/docker-compose.yml)

## Transformed Data (Format : csv)
1. [Target Data.csv](https://github.com/Adwait0043/-Real-Time-Data-Streaming-using-Apache-Nifi-AWS-Snowpipe-Stream-Task/blob/main/Target_data.csv)

## Motivation

In today’s fast-paced data landscape, the ability to process and analyze real-time data is critical. 
This project targets industries requiring instantaneous data insights, such as finance, e-commerce, and social media analysis. 
By leveraging real-time data streaming, organizations can make informed decisions and respond to trends as they happen.

**Real-World Use Case**
Real-time data streaming is essential for various stakeholders, including:

**E-commerce Platforms:** To track user interactions and inventory levels in real-time, enabling dynamic pricing and recommendations.
**Financial Services:** To monitor transactions for fraud detection and compliance in real-time.
**Marketing Analysts:** To analyze social media trends and customer sentiments instantly.
This project illustrates how a well-architected data streaming pipeline can meet the growing demand for real-time analytics.

## Features

**Real-Time Data Ingestion**
  
  -- Apache NiFi: Utilized for seamless data ingestion from various sources, enabling real-time data collection.
  
  -- Data Provenance: Apache NiFi's built-in data lineage tracking allows for transparency and traceability in data processing.

**Scalable Processing**
  
  -- AWS EC2: Leveraged EC2 instances for scalable processing of streaming data, ensuring high availability and performance.
  
  -- Dynamic Scaling: Configured EC2 instances to scale up or down based on data volume and processing needs.

**Efficient Data Loading**

  -- Snowflake Integration: Employed Snowflake for efficient data storage and querying, providing high-performance analytics capabilities.
  
  -- ETL Processes: Implemented robust ETL processes to clean and transform data before loading into Snowflake.

**Comprehensive Monitoring**

  -- Pipeline Monitoring: Utilized monitoring tools to track the health and performance of the pipeline, ensuring real-time alerts and issue resolution.
  
  -- Performance Metrics: Collected performance metrics to analyze processing speed and efficiency.

## Challenges Faced

**1. Data Latency Issues**

**Issue:**: Ensuring minimal latency during data ingestion and processing to provide real-time insights.

**Solution:**
Optimized Apache NiFi flow configurations and EC2 instance settings to enhance performance and reduce latency.

**2. Data Quality Management**

**Issue:**:  Maintaining high data quality and consistency throughout the streaming process.

**Solution:** 
Implemented validation checks and error handling mechanisms within Apache NiFi to ensure data integrity.

**3. Resource Management**

**Issue:** Managing EC2 instances effectively to balance performance and cost.

**Solution:**
Employed auto-scaling and instance monitoring to optimize resource allocation based on demand.
