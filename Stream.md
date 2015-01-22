# Stream processing


## Apache Storm


**Strength**
* Processing massive amounts of streaming events with real-time responsiveness;
* Integrates with any queueing system and any database system;
* Scalability: adjust the parallelism of running topologies on the fly;
* High-available and fault tolerant;
* Simple API;
* Guarantee no data loss.

**Weakness**
* No well-defined framework;
* Not for batch-mode processing or transactions;
* No persistency.

**Reference**
* Apache Storm, Rationale, https://storm.apache.org/documentation/Rationale.html
* Real-Time Stream Processing as Game Changer in a Big Data World with Hadoop and Data Warehouse, http://www.infoq.com/articles/stream-processing-hadoop


## Apache S4


**Strength**
* Processing massive amounts of streaming events with real-time responsiveness;
* Scalability: adjust the parallelism of running topologies on the fly;
* High-available and fault tolerant;
* Simple API, well-defined Map/Reduce like framework, easy to program.

**Weakness**
* No guaranteed data delivery;
* Not for batch-mode processing or transactions.

**Reference**
* http://incubator.apache.org/s4/
* Distributed stream processing showdown: S4 vs Storm, http://gdfm.me/2013/01/02/distributed-stream-processing-showdown-s4-vs-storm/



## SQLStream


**Strength**
* Real-time stream processing platform with enterprise support;
* Proven more throughput and lower latency;
* SQL for stream processing.

**Weakness**
* Proprietary;
* Not for batch-mode processing or transactions.

**Reference**
* SQLStream, SQL for stream processing, http://www.sqlstream.com/stream-processing-with-sql/


## DataTorrent


**Strength**
* Real-time stream processing platform built upon Hadoop with enterprise support;
* Native support for application window abstraction;
* Separate the functional specifications from the operability of the application;
* Built-in fault-tolerance, self-healing and state recovery.

**Weakness**
* Proprietary;
* Not for batch-mode processing or transactions.

**Reference**
* Open source “Storm” vs. Commercially available “Data Torrent", https://mybigdatajourney.wordpress.com/2014/07/24/open-source-storm-vs-commercially-available-data-torrent/
* Crossing the Big Data Stream with DataTorrent, http://www.datanami.com/2014/04/23/crossing_the_big_data_stream_with_datatorrent/


## FeedZai


**Strength**
* Real-time stream processing geared towards fraud detection with  machine learning;
* Data visualization and dashboard interface.

**Weakness**
* Proprietary;
* Limited use case.

**Reference**
* FeedZai, Big Data Solutions, https://www.feedzai.com/home/big-data-insight/

## TIBCO StreamBase


**Strength**
* Real-time stream processing platform with enterprise support;
* Rapid time from development to deployment with graphical event-flow language;
* Shorter development cycles with easier maintenance.

**Weakness**
* Proprietary;
* Not for batch-mode processing or transactions.

**Reference**
* White Paper, TIBCO StreamBase Overview



## Software AG Apama


**Strength**
* Enterprise real-time stream processing platform with enterprise support.
* Rich analytics tooling, visualization of real-time analytics;
* Static data cached for fast, in-memory access and event enrichment;



**Weakness**
* Proprietary;
* Not for batch-mode processing or transactions.

**Reference**
* http://www.softwareag.com/corporate/products/apama_webmethods/analytics/capabilities/default.asp


## Lokad


**Strength**
* Real-time stream processing geared towards commerce and demand forcast.

**Weakness**
* Proprietary;
* Limited use case.

**Reference**
* Lokad, Technology, http://www.lokad.com/forecasting-technology


## Amazon Kinesis 


**Strength**
* Full-managed real-time stream processing platform with support;
* Elastic scalability;
* Can emit data from Amazon Kinesis to other AWS services;
* CloudWatch Monitoring built-in.

**Weakness**
* Not for batch-mode processing or transactions.

**Reference**
* Kinesis Details, http://aws.amazon.com/kinesis/details/


## Google Cloud Dataflow


**Strength**
* Full-managed real-time stream processing platform;
* Elastic scalability;
* Integration with other Google services;
* Support stream and batch-mode.

**Weakness**
* Still in Alpha.

**Reference**
* MapReduce Successor Google Cloud Dataflow is a Game Changer for Hadoop Thunder, http://cloudtimes.org/2014/07/07/mapreduce-successor-google-cloud-dataflow-is-a-game-changer-for-hadoop-thunder/


## Guavus

**Strength**
* End-to-End streaming analytics platform and decisioning applications for various industries;
* Near real-time streaming with built-in data science.

**Weakness**
* Proprietary.

**Reference**
* http://www.guavus.com/products/


## IBM InfoSphere Streams


**Strength**
* Real-time streaming processing platform for analysis of large structured and unstructured data volumes;
* Integration with IBM's other services;
* Comes with IBM Accelerator for Machine Data Analytics, Social Data Analytics and Telecommunications Event Data Analytics. 

**Weakness**
* Not for batch-mode processing or transactions;
* Proprietary.

**Reference**
* White Paper, InfoSphere Streams Quick Start Edition Overview
