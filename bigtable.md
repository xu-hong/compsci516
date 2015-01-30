# Bigtable

## HBase

**Strength**
* Google's Bigtable on top of Hadoop and HDFS;
* Automatic sharding: tables are distributed via regions, and regions are automatically split and re-distributed as data grows;
* Map/reduce with Hadoop;
* Optimizations for real time queries;
* Optimized for sequential write operations, and it is highly efficient for batch inserts, updates, and deletes;
* Strongly consistent reads/writes;
* High scalability of HDFS.

**Weakness**
* Not an ACID compliant database;
* Single point of failure as a master-slave architecture; 
* No JOIN;
* JVM may cause performance issues;
* Weak security.

**Reference**
* http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis
* Riak Compared to HBase, http://docs.basho.com/riak/latest/theory/comparisons/hbase/
* HBase Architecture Analysis Part 3 Pros and Cons, http://www.cyanny.com/2014/03/13/hbase-architecture-analysis-part-3-pros-cons/


## HyperTable

**Strength**
* Google's Bigtable on top of Hadoop and HDFS;
* Map/reduce with Hadoop;
* Strongly consistent reads/writes;
* Geared towards fast access to ranges of data by keeping data physically sorted by a primary key;
* Written in C++ other than Java, faster in tests of random write and scan than HBase.

**Weakness**
* Not an ACID compliant database;
* Single point of failure as a master-slave architecture; 
* No JOIN.

**Reference**
* Hypertable vs. HBase Performance Evaluation, http://hypertable.com/why_hypertable/hypertable_vs_hbase_2/
* Hypertable documentation architecture, http://hypertable.com/documentation/architecture/



## Accumulo

**Strength**
* Google's Bigtable on top of Hadoop and HDFS;
* Map/reduce with Hadoop;
* Optimizations for real time queries;
* Random access performance is like MySQL;
* Strongly consistent reads/writes;
* High scalability of HDFS;
* Cell-level security functionality.

**Weakness**
* Not an ACID compliant database;
* Single point of failure as a master-slave architecture; 
* No JOIN;
* No replication across datacenter.

**Reference**
* Distributed NoSQL: HBase and Accumulo, https://haifengl.wordpress.com/2014/05/14/hbase-and-accumulo/
* Accumulo: Why The World Needs Another NoSQL Database, http://wikibon.org/blog/breaking-analysis-accumulo-why-the-world-needs-another-nosql-database/

## Google App Engine Datastore

**Strength** 
* An database modeled after Google's Bigtable;
* Highly reliable and covered by the App Engine SLA;
* ACID transactions;
* Advanced querying features;
* High availability of reads and writes;
* Strong consistency for reads and ancestor queries;
* High scalability.

**Weakness**
* Strongly consistent except when performing global queries;
* No support for complex queries.

**Reference**
* Mastering the datastore, https://cloud.google.com/appengine/articles/datastore/overview
* Storing data in Java, https://cloud.google.com/appengine/docs/java/storage#app_engine_datastore




## Google Cloud Datastore

**Strength**
* A schemaless datastore modeled after Google's Bigtable;
* No planned downtime;
* Atomic transactions;
* High availability of reads and writes;
* Strong consistency for reads and ancestor queries;
* Eventual consistency for all other queries;
* High availability: replication across multiple datacenters based on the Paxos algorithm. 

**Weakness**
* No Join operations;
* No inequality filtering on multiple properties;
* No filtering of data based on results of a subquery.

**Reference**
* Datastore Concepts Overview, https://cloud.google.com/datastore/docs/concepts/overview#Datastore_Comparison_with_traditional_databases
