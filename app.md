# Appliance and specialist analytic



## Oracle database 12c

**Strength**
* Supreme performance: a relational in-memory column database system for high-throughput, operational applications;
* ACID transactions;
* SQL as native language;
* Support for both OLTP and data warehousing;
* High availability: data automatically replicated for intra- and inter-cluster;
* Easy administrative tools.

**Weakness**
* High cost;
* Proprietary.

**Reference**
* White paper, Automatic Data Optimization with Oracle Database 12c
* 12c documentation, Database High Availability Overview

## IBM DB2

**Strength**
* Mature relational database manager;
* ACID transactions;
* SQL as native language;
* Dynamic bitmap indexing;
* High scalability in a Symmetric Multi-Processing system;
* Can be tuned for both OLTP and data warehousing;
* High availability: data automatically replicated for intra- and inter-cluster;
* Easy administrative tools.

**Weakness**
* High cost;
* Proprietary;
* Primitive data models.

**Reference**
* White paper,  < IBM DB2 Universal Database on Windows NT Clusters>
* Comparison_and_Compatibility, http://en.wikibooks.org/wiki/Oracle_and_DB2,_Comparison_and_Compatibility

## IBM Informix

**Strength**
* An embeddable database that integrates SQL, NoSQL/JSON, timeseries and spatial data;
* ACID transactions;
* SQL as native language;
* Deep compression of data, indexes, and blobs reduces storage needs and increases performance;
* Accelerated queries with an in-memory, columnar approach;
* Suitable for both OLTP and data warehousing;
* Easy administrative tools;
* High Availability.

**Weakness**
* High cost;
* Proprietary;
* Limited scalability.

**Reference**
* IBM Knowledge Center, Informix Servers 11.7, Administrator's Guide


## PostgreSQL

**Strength**
* Mature, powerful, open source object-relational database system with JSON data type support as well as JSON indexing;
* Good support for BLOBs as well;
* Cost-based query optimization methods geared for complex join;
* Flexibility offered by the advanced GiST (Generalized Search Tree) indexing;
* ACID transactions, Multiversion concurrency control;
* Near linear scalability and High availability;
* A shared buffer cache and the kernel cache offer fast reads;
* Suitable for both OLTP and data warehousing;
* High standard compliance.

**Weakness**
* Behind MySQL in terms of popularity;
* Replication is not yet as well implemented as in MySQL.

**Reference**
* http://www.postgresql.org/about/
* http://wiki.postgresql.org/wiki/Why_PostgreSQL_Instead_of_MySQL%3a_Comparing_Reliability_and_Speed_in_2007
* http://www.quora.com/What-are-the-advantages-and-disadvantages-of-using-PostgreSQL-over-MySQL




## Oracle Exadata 

**Strength**
* A datawarehousing bundle, the highest performing platform for Oracle Database, with scale-out architecture, high speed internal fabric, in-memory fault tolerance and other enterprise level optimization.

**Weakness**
* Heavy, exclusive ecosystem;
* Expensive!

**Reference**
* Oracle Exadata Machine, Features and Benefits, https://www.oracle.com/engineered-systems/exadata/features.html

## IBM PureData 

**Strength**
* A datawarehousing platform wherein the hardware, storage and software capabilities are designed and optimized for specific high performance data workloads;
* Applicable for both OLTP and OLAP.

**Weakness**
* Heavy, exclusive ecosystem;
* Expensive!

**Reference**
* IBM PureData documentation, http://www-01.ibm.com/software/data/puredata/

## SAP HANA

**Strength**
* An in-memory, column-oriented, relational database management system;
* Fast querying, real-time, operational analytic capability: cache/disk latency is eliminated;
* OLAP and OLTP activities can take place in parallel in real time;
* High scalability.

**Weakness**
* Concurrency support;
* Performance will deteriorate as query complexity increases.

**Reference**
* Research Report, IBM DB2 BLU Acceleration vs. SAP HANA vs. Oracle Exadata
* SAP HANA, Why HANA, http://hana.sap.com/abouthana/why-hana.html


## Microsoft SQL Server PDW

**Strength**
* PDW ships as an appliance with hardware and software pre-installed and pre-configured for maximum performance;
* Data load in real-time and fast complex queries with Massively Parallel Processing (MPP) design;
* Applicable for both OLAP and OLTP;
* High scalability: auto-rebalancing.

**Weakness**
* Not all features of SQL Server are supported;
* Not optimal for OLTP.

**Reference**
* A Breakthrough Platform for Next-Generation Data Warehousing and Big Data Solutions, Barbara Kess and Dan Kogan
* Microsoft SQL Server Parallel Data Warehouse (PDW) Explained, http://www.jamesserra.com/archive/2011/08/microsoft-sql-server-parallel-data-warehouse-pdw-explained/



## Oracle Exalytics

**Strength**
* A in-memory analytic relational data platform for Oracle Database, with scale-out architecture, high speed internal fabric, and other enterprise level optimization;
* Geared towards operational computation.

**Weakness**
* Database size limitation;
* Expensive!

**Reference**
* Oracle Exalytics In-Memory Machine, Features, https://www.oracle.com/engineered-systems/exalytics/features.html



## Teradata

**Strength**
* A datawarehousing platform wherein the hardware, storage and software capabilities are designed and optimized for specific high performance data workloads;
* Shared nothing architecture, ability to scale out and to process extremely large data;
* Secondary indexing, partitioning, columnar design and in-memory enhancement to boost complex querying performance.


**Weakness**
* Pool usability; 
* Expensive!


**Reference**
* White Paper, Hadoop and the Data Warehouse: When to Use Which

## Teradata Astor 

**Strength**
* Provides out-of-the box integrated data acquisition, data preparation, analysis and visualization in a single SQL statement;
* Hybrid  across the Aster and Apache Hadoop platforms, enablement of Map/Reduce.

**Reference**
* Product Features, http://www.teradata.com/Aster-Big-Analytics-Appliance/?LangType=1033&LangSelect=true#tabbable=0&tab1=0&tab2=0



## XtremeData

**Strength**
* High performance ANSI SQL database engine based on PostgreSQL, designed for performance at all scales, up to 100s of terabytes;
* Full SQL and ACID compliant database engine based on shared-nothing, massive parallel query execution;
* Easy deployment on AWS or other virtualized platform;
* Schema/query agnostic.

**Weakness**
* Not optimal for OLTP;
* Bulk write latency.

**Reference**
* XtremeData Leapfrogs Competitors, http://www.referencedatareview.com/blog/xtremedata-leapfrogs-competitors-new-breed-appliances-database-analytics
* Large Scale Data Analytics with XtremeData Parallel SQL Database Engine, http://architects.dzone.com/articles/large-scale-data-analytics
* Big Data Management Platforms: Architecting Heterogeneous Solutions, http://www.xtremedata.com/articles/big-data-management-platforms-architecting-heterogeneous-solutions



## SQream

**Strength**
* High performance analytical, transactional SQL database at petabyte scale;
* Capable of processing and analyzing high volumes of data with GPU-based, columnar SQL database employing aggressive compression;
* Ability of powering an entire datacenter from a standard server.

**Weakness**
* Bulk write latency.

**Reference**
* SQream brochure

## RainStor

**Strength**
* Big Data database for storing petabyte-scale volumes of structured and semi-structured data;
* Fast query, high-speed loading at scale, industry-leading compression;
* Storage agnostic: 
* Flexible query: SQL, Map/Reduce, and text search;
* Audit Trails and Encryption.

**Weakness**
* Random, concurrent writes.

**Reference**
* RainStor Product, http://rainstor.com/products/rainstor-database/

## HPCC

**Strength**
* A big data architecture which incorporates middleware components, an external communications layer, client interfaces, and system management tools;
* Highly optimized language and compiler;
* Easy to develop data-centric language: ECL: 
* Inbuilt auditing, monitoring and workflow.

**Weakness**
* Horizontal scalability;
* No SQL or SQL-like language.

**Reference**
* HPCC System, How It Works and Benefits, hpccsystems.com/Why-HPCC/How-it-works



## SciDB

**Strength**
* Computational, ACID transactional DBMS for research: programmable from R & Python;
* Scalability: shared-nothing, massively parallel processing (MPP) architecture;
* Array data model for highly faceted data use.

**Weakness**
* Random, concurrent writes;
* No SQL or SQL-like language.

**Reference**
* Paradigm4, Technology, http://www.paradigm4.com/technology/








## Oracle Big Data Appliance 

**Strength**
* Pre-integrated datawarehousing platform with full-rack configuration, Cloudera, and Oracle NoSQL;
* A budget Oracle's Big Data solution.

**Weakness**
* Limited flexibility;
* Suited for medium size database.

**Reference**
* White Paper, Getting Real About Big Data: Build Versus Buy


## Oracle Big Data Cloud 

**Strength**
* Provision fully configured Hadoop clusters on demand with elastic scalability.

**Weakness**
* Still under development.

**Reference**
* https://cloud.oracle.com/bigdata

