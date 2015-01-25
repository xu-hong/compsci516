
# MySQL ecosystem

## MySQL

**Strength**
* World's most widely used open-source relational database management system (RDBMS);
* ACID transactions;
* Built-in replication support;
* Full-text indexing and searching;
* Commonly used in small to medium scale single-server deployments;
* High availability can be provided by MySQL Fabric;
* Shared-nothing clustering through MySQL Cluster.

**Weakness**
* Strongly limited by hard disk performance;
* Not currently compliant with the full SQL standard.

**Reference**
* http://en.wikipedia.org/wiki/MySQL
* http://www.mysql.com/why-mysql/topreasons.html


## GenieDB
GenieDB is a globally distributed MySQL-as-a-Service to provide continuous availability during datacenter or cloud outage and faster response times for users anywhere in the world.





## MariaDB

**Strength**

A community-developed fork, drop-in replacement for the MySQL relational database management system with improvements in:
* Variety of storage engines;
* Disk access optimization;
* Join and query optimization;
* Truly open source.

**Reference**
* https://mariadb.com/kb/en/mariadb/mariadb-vs-mysql-features/
* https://mariadb.com/kb/en/mariadb/mariadb-vs-mysql-features/




## MariaDB Enterprise

MariaDB Enterprise is a proprietary version that extends MariaDB with fully-tested binaries and technical support, backup and recovery.

**Reference**
* https://mariadb.com/products/mariadb-enterprise

## Spider

**Strength**
* A storage engine with built-in sharding features, supporting partitioning and XA transactions for MariaDB.

**Weakness**
* Immature product, incomplete documentation.

**Reference**
* Spider Storage Engine Overview, https://mariadb.com/kb/en/mariadb/documentation/storage-engines/spider/spider-storage-engine-overview/



## Percona

**Strength**

A community-developed fork, drop-in replacement for the MySQL relational database management system with improvements in:
* Faster querying and strong consistency;
* Easier administration;
* High availability.

**Reference**
* Percona Server Feature Comparison, http://www.percona.com/doc/percona-server/5.6/feature_comparison.html
* Oracle MySQL 5.6 vs Percona Server 5.5 vs MariaDB 5.5, http://www.sobstel.org/blog/mysql-like-databases-comparison/



## TokuDB

**Strength**
* An open source, high-performance storage engine for MySQL, MariaDB, and Percona Server;
* Improvement in scalability and operational efficiency;
* Improvement in insertions and indexing: replaces B-tree indexing with modern Fractal Tree indexing;
* Better compression that cuts disk and flash-drive storage requirements;
* Hot schema changes.

**Weakness**
* Schema.

**Reference**
* http://www.tokutek.com/tokudb-for-mysql/
* TokuDB Differences, https://mariadb.com/kb/en/mariadb/documentation/storage-engines/tokudb/tokudb-differences/


## RackSpace Cloud Databases
A managed cloud service with a wide range of services at different levels in architecture, building, and operation.


## ScaleDB


**Strength**
* A data platform that transforms MySQL/MariaDB into scalable database cluster;
* High scalability: no sharding, shared-data approach;
* High availability with master-only architecture;
* Compatibility: works with existing MySQL applications without the need to change code.

**Weakness**
* Schema.

**Reference**
* White Paper, ScaleDB for MySQL/MariaDB
* White Paper, ScaleDB Technical Overview



## Drizzle

**Strength**
* A community-developed fork, drop-in replacement for the MySQL relational database management system with support for IPv6.

**Weakness**
* Incomplete documentation and limited support.

**Reference**
* http://www.drizzle.org/content/drizzle-and-ipv6

## Infobright

**Strength**
* Column-oriented relational database software with a focus in machine-generated data;
* Integration with MySQL with querying optimization;
* Increased scalability;
* Faster load from disk, better compression.

**Weakness**
* Write latency;
* Schema.

**Reference**
* http://en.wikipedia.org/wiki/Infobright




## Google Cloud SQL

**Strength**
* A fully managed MySQL service hosted on Google Cloud Platform, providing a database backbone for applications running on Google App Engine or Google Compute Engine;
* Security: Cloud SQL data is automatically encrypted;
* High availability and reliability;
* Standard MySQL, supporting complex queries, ACID transaction. 

**Weakness**
* Limited choice in database;
* Less scalable performance.

**Reference**
* Google Cloud SQL debuts, following Amazon's RDS lead, http://www.infoworld.com/article/2610430/cloud-computing/google-cloud-sql-debuts--following-amazon-s-rds-lead.html
* Google Cloud SQL, Features, https://cloud.google.com/sql/#features
* http://stackoverflow.com/questions/10905861/gae-datastore-vs-google-cloud-sql-for-enterprise-managment-systems


## HP Cloud RDB for MySQL 

**Strength**
* A fully managed MySQL service hosted on HP Cloud;
* High availability and reliability;
* Flexible database resize;
* Standard MySQL on OpenStack.

**Weakness**
* Limited choice in database;
* Limited scalability.

**Reference**
* HP Cloud Relational Database, Features, http://www.hpcloud.com/products-services/relational-database?t=features

## FathomDB
Set out as a fault-tolerant and scalable relational database service. Currently under further development after being acquired by Meteor.

**Reference*
* Meteor Acquires YC Alum FathomDB For Its Development Platform, http://techcrunch.com/2014/10/07/meteor-acquires-yc-alum-fathomdb-for-its-web-development-platform/

## AWQ RDS

**Strength**
* A fully managed relational database service hosted in the cloud;
* Security: encryption supported for MySQL or PostgreSQL databases;
* High availability and reliability with Multi-AZ;
* Wide range of database options.

**Weakness**
* High cost relative to limited functionality and performance.

**Reference**
* http://stackoverflow.com/questions/4806272/what-are-the-respective-advantages-limitations-of-amazon-rds-vs-ec2-with-mysql
* Amazon RDS Product Details, http://aws.amazon.com/rds/details/





## ClearDB

**Strength**
* A geo-distributed MySQL database geared towards high availability, survivability, and reliability;
* Offers true multi-regional read/write mirroring with 100% uptime;
* Compatibility: native MySQL, works with existing MySQL applications without the need to change code;
* Security.

**Weakness**
* Schema;
* Write performance.

**Reference**
* How ClearDB Works, https://www.cleardb.com/better.view



## WebScaleSQL

**Strength**
* A MySQL data platform that is scale-oriented;
* Optimizations to certain types of queries;
* Compatibility: works with existing MySQL applications without the need to change code.

**Weakness**
* Schema;
* Weak consistency.

**Reference**
* http://webscalesql.org/faq.html




## DeepDB

**Strength**
* Designed to deliver significant performance and scaling benefits for both transactional and analytic workloads;
* Accommodate both structured and unstructured data in the same database;
* Maximize performance by providing a high level of CPU concurrency and efficient memory management;
* Support all common storage types;
* High availability.


**Weakness**
* Distributed consistency.

**Reference**
* DeepDB White Paper, http://deep.is/resources/deepdb-white-paper/

## Galera

**Strength**
* A true MySQL multimaster cluster based on synchronous replication;
* High availability with a highly transparent and scalable synchronous replication solution.

**Weakness**
* Schema.

**Reference**
* White paper, <Minimizing downtime and maximizing elasticity with Galera Cluster for MySQL>


## Zimory
**Strength**
* A Cloud Computing Software that supports the heterogeneous of the technological platform by coordinating communication between several varied product modules;
* Simplicity and excellent usability.

**Reference**
* Zimory, Technology and Architecture, http://www.zimory.com/en/technology-and-services/zimory-eco/architecture.html#c403



## Continuent

**Strength**
* A scalable MySQL database cluster;
* High availability with asynchronous, transactional replication;
* Globally reduntant disaster recover (DR) capabilities;
* High performance with real-time data loading;
* Replication in real-time from RDBMS to MongoDB, Hadoop, and Vertica;
* Supports MySQL, MySQL Community and Enterprise versions (5.0 to 5.6), MariaDB (5.5) and Percona Server (5.5 and 5.6) without changes. 

**Weakness**
* Schema.

**Reference**
* Cotinuent, Solutions, http://www.continuent.com/solutions




## CodeFutures AgilData

**Strength**
* A Real-time high-performance stream processing big data platform;
* SQL abstraction layer for the creation and querying of streams;
* An agile architecture that creates dynamic views of data specific to applications’ needs.

**Weakness**
* Less efficient use of storage.

**Reference**
* White paper, Real Time Big Data: An Agile Approach



## Tesora

**Strength**
* Database as a Service platform built upon OpenStack Trove project;
* Easy implementation;
* Multi-database support;
* Automatic backup and recovery.

**Reference**
* The Tesora Trove Difference, http://www.tesora.com/solutions/tesora-trove-difference



## ScaleArc

**Strength**
* An abstraction layer between applications and databases, supporting MySQL, SQL server, and Oracle;
* High scalability through load-balancing and replication;
* High availability and automatic failover;
* Optimized for real-time analytics.

**Weakness**
* Schema;
* Weak performant consistency;
* Write latency.

**Reference**
* ScaleArc, How It Works, http://scalearc.com/how-it-works


## ScaleBase

**Strength**
* A distributed MySQL database architecture designed for web-scale applications;
* High scalability through auto-sharding and replication;
* High availability and geo-distributed data.

**Weakness**
* Schema;
* Weak performant consistency (Two-Phase commit);
* Write latency.

**Reference**
* ScaleBase Technical Whitepaper

