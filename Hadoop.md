# Hadoop ecosystem



## Pivotal HD: HAWQ


**Strength**
* HAWQ is a parallel SQL query engine that combines the key technological advantages of Pivotal Analytic Database with the scalability and convenience of Hadoop; 
* High availability, tolerates disk level and node level failures;
* Transactions on Hadoop. 

**Weakness**
* Geared towards OLAP not OLTP.


**Reference**
* White Paper, Pivotal HD: HAWQ, A TRUE SQL ENGINE FOR HADOOP


## Hadapt


**Strength**
* A native implementation of SQL to the Apache Hadoop, which allows interactive SQL-based analysis of massive data set; 
* All data – structured, unstructured, and semi-structured – accessible via SQL.


**Weakness**
* Geared towards OLAP not OLTP;
* No trasaction.


**Reference**
* Hadapt, Schemaless SQL Overview, http://hadapt.com/schemaless-sql-overview/


## JethroData


**Strength**
* A column store SQL Engine to the Apache Hadoop; 
* High performance ad-hoc query: every column is indexed by default, and indexes span entire dataset;
* Shared everything structure, storage and compute scale independently.


**Weakness**
* Geared towards OLAP not OLTP;
* No trasaction.


**Reference**
* Hadapt, Schemaless SQL Overview, http://hadapt.com/schemaless-sql-overview/

##CitusData


**Strength**
* CitusDB scales out PostgreSQL through sharding and replication;
* High availability: real-time recovery;
* Semi-structured data support: run distributed SQL queries on JSON and log files.


**Weakness**
* Geared towards OLAP not OLTP.


**Reference**
* CitusData product, http://www.citusdata.com/products



## Impala


**Strength**
* A transactional SQL Engine on the Apache Hadoop geared towards analytics; 
* Low latency, interactive performance at Hadoop scale;
* Structured, semi-structured, and unstructured data with schema-on-read or schema-on-write capabilities.


**Weakness**
* Geared towards OLAP not OLTP;
* Impala uses a custom C++ runtime, it doesn't support Hive UDFs;
* Not fault tolerant (queries must be restarted if a node fails).


**Reference**
* How does Cloudera Impala compare to Apache Shark (now part of Spark)?, http://www.quora.com/How-does-Cloudera-Impala-compare-to-Apache-Shark-now-part-of-Spark
* Cloudera Impala, http://www.cloudera.com/content/cloudera/en/products-and-services/cdh/impala.html



## IBM Big SQL


**Strength**
* Enables InfoSphere BigInsightsusers to query Hadoop data using industry-standard SQL;
* Geared towards OLTP.


**Weakness**
* No fault tolerance;
* Closed ecosystem;
* No transaction.


**Reference**
* What's the big deal about Big SQL?, http://www.ibm.com/developerworks/library/bd-bigsql/

## Presto


**Strength**
* An distributed SQL query engine for running interactive analytic queries against data sources of all sizes ranging from gigabytes to petabytes;
* Allows querying data on Hive, Cassandra, relational databases as well as data from combined multiple sources.


**Weakness**
* Weakness of the underlying systems.


**Reference**
* Presto Documantation, http://prestodb.io/docs/current/


## Apache Drill

**Strenth**
* A low latency SQL query engine for multi-structured datasets on Hadoop and NoSQL;
* Compatibility with existing SQL environments and Apache Hive deployments;
* Self-describing data support without centralized schema definitions/management;
* Support for complex/multi-structured data types;
* ANSI SQL support (not SQL "Like") & BI tool integration;
* Extensibility to go beyond Hadoop environments.


**Weakness**
* Not an optimal choice for OLTP/operational application;
* No trasaction.


**Reference**
* Why Drill, http://drill.apache.org/why/


## Apache Hive

**Strenth**
* A data warehouse software facilitates querying and managing large datasets residing in distributed storage;
* Query  data using a SQL-like language called HiveQL;
* A matured and proven solution that runs on proven MapReduce framework;
* Can be mapped to HBase and other systems easily.	

**Weakness**
* Query performance;
* No transaction, not for OLTP.


**Reference**
* Hive documantation, https://cwiki.apache.org/confluence/display/Hive/Home
* Hive, Impala and Presto – The War on SQL over Hadoop, https://bigdatanerd.wordpress.com/2013/11/19/war-on-sql-over-hadoop/




## MammothDB

**Strenth**
* A native columnar MySQL Engine on the Apache Hadoop with integration of BI tools; 
* Designed for low cost.

**Weakness**
* Geared towards OLAP not OLTP;
* No trasaction;
* Fledgling.

**Reference**
* MammothDB: The Easy Jet of Big Data, http://dataconomy.com/mammothdb-easy-jet-big-data/



## Apache Tajo

**Strenth**
* A robust big data relational and distributed data warehouse system for Apache Hadoop;
* Designed for low-latency and complex ad-hoc queries, online aggregation, and ETL on HDFS and other data sources;
* ANSI/ISO SQL standard compliance;
* Hive metastore integration for access to Hive datasets.

**Weakness**
* Not an optimal choice for OLTP/operational application;
* No trasaction.

**Reference**
* Tajo documentation, http://tajo.apache.org/





## Cloudera

**Strength**
* Enterprise-ready Hadoop distributions with enduring security and stability;
* Scalability, shared-nothing computing framework;
* Support MapReduce as well as YARN;
* Has a proprietary management software Cloudera Manager, SQL query handling interface Impala, as well as Cloudera Search for easy and real-time access of products. 

**Weakness**
* Licensing fee;
* Not an optimal choice for OLTP.

**Reference**
* Cloudera FAQ, http://www.cloudera.com/content/cloudera/en/about/faqs.html#five
* Cloudera vs Hortonworks vs MapR: Comparing Hadoop Distributions, http://www.experfy.com/blog/cloudera-vs-hortonworks-comparing-hadoop-distributions/

## Spark


**Strength**
* Built on top of Hadoop,extends Hive to dramatically speed up both in-memory and on-disk queries; 
* Designed to support both short and long-running queries, can recover from mid-query faults;
* Support SQL queries, streaming data, and complex analytics such as machine learning and graph algorithms out-of-the-box.

**Weakness**
* Geared towards OLAP not OLTP.

**Reference**
* How does Cloudera Impala compare to Apache Shark (now part of Spark)?, http://www.quora.com/How-does-Cloudera-Impala-compare-to-Apache-Shark-now-part-of-Spark
* Hadoop vs Spark, http://stackoverflow.com/questions/25267204/hadoop-vs-spark



## MetaScale

**Strenth**
* Big Data as a Service (BDaaS) to build, operate and support a custom-designed computing platform and solution stack for running Hadoop and NoSQL technologies within a customer’s data center.

**Weakness**
* Not an optimal choice for OLTP/operational application;
* No trasaction.

**Reference**
* MetaScale, Big Data Platform, http://www.metascale.com/what-we-offer/big-data-platform.html#.VL6uBidrpTM


## Hortonworks

**Strength**
* Enterprise-ready Hadoop distributions without additional proprietary software;
* Scalability, shared-nothing computing framework;
* Support MapReduce as well as YARN;
* 100% open source and free.

**Weakness**
* Not an optimal choice for OLTP.

**Reference**
* Cloudera vs Hortonworks vs MapR: Comparing Hadoop Distributions, http://www.experfy.com/blog/cloudera-vs-hortonworks-comparing-hadoop-distributions/


## Microsoft HDInsight

**Strength**
* Hadoop solution on Azure and provides implementations of Storm, HBase, Pig, Hive, Sqoop, Oozie, Ambari, and so on; 
* Integrates with business intelligence (BI) tools such as Excel, SQL Server Analysis Services, and SQL Server Reporting Services;
* Process unstructured and semi-structured data;
* High availability and reliability of clusters.

**Weakness**
* No native SQL, no transactions.

**Reference**
* HDInsight documentation, http://azure.microsoft.com/en-us/documentation/services/hdinsight/


## IBM BigInsights

**Strength**
* Robust SQL on Hadoop with Big SQL; 
* Integrates with analytics such as R, text analytics, Real-time Streaming Analytics, etc;
* Process unstructured and structured data;
* Fault-tolerant, secure, POSIX Compliant file system option.

**Weakness**
* Expensive;
* For OLAP not OLTP.

**Reference**
* Understanding InfoSphere BigInsights, http://www.ibm.com/developerworks/data/library/techarticle/dm-1110biginsightsintro/


## MapR

**Strength**
* Enterprise-ready Hadoop distributions with high availability, disaster recovery, security, and full data protection;
* Can be easily accessed as traditional network attached storage (NAS) with read-write capabilities;
* Works with nested/hierarchical data structures, schema discovery and NoSQL, Hadoop as well as traditional RDBMS;
* Real-time stream computational engines;
* Point-in-time consistency for all files and tables.

**Weakness**
* Not pure HDFS, proprietary File System.

**Reference**
* Cloudera vs Hortonworks vs MapR – Has MapR Already Won This Contest?, http://data-magnum.com/cloudera-vs-hortonworks-vs-mapr-has-mapr-already-won-this-contest


## AWS EMR

**Strength**
* Easy to configure and deploy with a flexibility of data stores;
* Elastic scalability and reliability;
* Easy to use web UI and robust integration with S3.

**Weakness**
* For OLAP not OLTP;
* May become expensive for production system.

**Reference**
* Amazon EMR Product Details, http://aws.amazon.com/elasticmapreduce/details/

## Goolge Compute Engine

**Strength**
* Large-scale workloads on virtual machines hosted on Google's infrastructure with multiple choices of dataplatforms;
* High-performant, scalable, highly secure and reliable virtual machines;
* Global load-balancing to achieve maximum performance, throughput and availability at low cost.

**Weakness**
* Weaker support and SLA compared to AWS.

**Reference**
* 4 Things CIOs Must Know: Google Compute Engine (GCE) + the Public Cloud, http://siliconangle.com/blog/2013/05/28/round-up-cios-must-know-for-google-compute-engine-gce-the-public-cloud/
* GCE Features, https://cloud.google.com/compute/#features

## Zettaset

**Strength**
* A Hadoop cluster management software for the enterprise with easy administration;
* Enterprise security, high availability, and performance requirements.

**Weakness**
* For OLAP not OLTP;
* No query language;
* Weak speed and performance compared to other competitors.

**Reference**
* Zettaset, Why Zettaset, http://www.zettaset.com/index.php/company/why-zettaset/

## Treasure Data

**Strength**
* End-to-end cloud-based, managed service for data collection, storage and analysis;
* Easy for data collecting;
* Flexible analytical methods;
* Loosely-coupled, multi-layer architecture that allows I/O, processing, and storage layers to independently scale;
* Support infrastructure management and monitoring.

**Weakness**
* For OLAP not OLTP.

**Reference**
* Treasure Data, Technology, http://www.treasuredata.com/technology.php
* Treasure Data takes aim at data warehousing giants, http://research.gigaom.com/2012/09/treasure-data-takes-aim-at-data-warehousing-giants/

## Qubole

**Strength**
* Everything Big Data as a Service: complete Hadoop-based Big Data service on the cloud, from query editor to storage;
* Auto scaling and spot instance pricing;
* Optimized Hiva and improved S3 performance.

**Weakness**
* For OLAP not OLTP.

**Reference**
* Qubole Features, http://www.qubole.com/features/

## Mortar Data

**Strength**
* Hadoop-based data platform with easy deployment and administration;
* Techologies of Mortar, Pig, AWS EMR, Luigi, and R, with flexible integration with different databases.

**Weakness**
* For OLAP not OLTP.

**Reference**
* Mortar Data, Platform, https://www.mortardata.com/platform


## Infochimps

**Strength**
* A scalable cloud services that supports streaming data and real-time analytics;
* Support NoSQL database and ad hoc, query-based analytics;
* Elastic Hadoop clusters and batch analytics.

**Weakness**
* For OLAP not OLTP.

**Reference**
* Infochimps, Overview, http://www.infochimps.com/infochimps-cloud/overview/

## MetaMarkets

**Strength**
* A scalable data platform geared toward real-time stream data analytics;
* Fast speed with in-memory store;
* Exploratory visualizations with proprietary visualization framework Facet.js.

**Weakness**
* For OLAP not OLTP;
* Not optimized for static data.

**Reference**
* MetaMarkets, Technology, https://metamarkets.com/what-we-do/technology/


## Altiscale

**Strength**
* Hadoop-based data platform with easy deployment and administration;
* Industry’s lowest total cost of ownership.

**Weakness**
* For OLAP not OLTP;
* Limited features compared to other Hadoop cloud vendors.

**Reference**
* Altiscale, Features, https://www.altiscale.com/hadoop-as-a-service/hadoop-features-benefits/


## Softlayer

**Strength**
* Big Data as a Service built upon high-performance hardware;
* Advanced network infrastructure with exceptional bandwidth and connectivity for the highest speed and reliability;
* Automated deployment and management of everything..

**Weakness**
* For OLAP not OLTP;
* Limited flexibility of services.

**Reference**
* Softlayer, Our Platform, http://www.softlayer.com/automation-control

## NGDATA

**Strenth**
* A specialized data analytic platform on Hadoop, geared towards real-time customer DNA analysis.

**Weakness**
* Niche application.

**Reference**
* NGDATA, Big Data Technology, http://www.ngdata.com/knowledge-center/big-data-technology/
