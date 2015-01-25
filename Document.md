# Document store

## MarkLogic

**Strength**
* Document-based data model with support for multiple data types;
* Support query with SPARQL; 
* Only Enterprise NoSQL database with built-in search capabilities;
* Flexible with storage choices — SSD, local disk (DAS) and shared disk (SAN, NAS), or Amazon S3 and HDFS;
* High scalability and availability;
* Tunable transaction mode, true ACID transactions.

**Reference**
* Whitepaper, Inside MarkLogic Server


## OrientDB

**Strength**
* Flexible data model for documents, graphs, and key-values;
* Convenient joins and SQL queries supported;
* ACID transactions supported;
* Elastic Distributed scalability added by Hazelcast;
* Reliability by replication and automatic failover organization.

**Weakness**
* JVM compatible;
* Possible single point of failure.  

**Reference**
* https://github.com/orientechnologies/orientdb/wiki/Distributed-Sharding
* http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis




## MongoDB

**Strength**
* Schemaless, JSON-based document datastore;
* High scalability: replication and auto-sharding;
* Replication across data centers;
* Efficient execution of queries with indexing;
* Map/Reduce operation support.

**Weakness**
* Map/Reduce performance;
* Less efficient usage of storage;
* Less flexibility in querying (no JOIN);
* No transactions except for certain atomic operations at a single document level.


**Reference**
* http://stackoverflow.com/questions/5244437/pros-and-cons-of-mongodb
* MongoDB manual


## MongoLab

Fully-managed MongoDB-as-a-Service with data protection and expert support.



## TokuMX
An open source, high-performance distribution of MongoDB with improvements in:
* Better caching and document-level locking: 50x performance improvements;
* Advanced compression: 90% reduction in database size;
* Support for ACID transactions and MVCC.

**Reference**
* http://www.tokutek.com/tokumx-for-mongodb/



## CouchDB

**Strength**
* Schemaless, JSON-based document datastore;
* ACID transaction, multi-version concurrency control;
* High availability with “shared nothing” replication;
* Efficient execution of queries with the view model for looking up and aggregating;
* Map/Reduce operation support,
* Compaction for more efficient use of storage.

**Weakness**
* No scalability “out-of-the-box” with sharding;
* Transaction only on a single document.

**Reference**
* CouchDB, Guide to Views
* CouchDB, Technical Overview



## Iris Couch
Free CouchDB hosting service



## Compose
Hosting service with choices of MongoDB, Elasticsearch, RethinkDB, or Redis. Seamless scalability, SSD backed.



## RavenDB

**Strength**
* Schemaless, JSON-based document datastore for .NET;
* ACID transaction for single or multi documents;
* High scalability: replication and sharding;
* High availability;
* Geared to massive and fast reads with efficient querying using Linq;
* Map/Reduce operation support;
* Compaction for more efficient use of storage.

**Weakness**
* Need to define your own sharding strategy.

**Reference**
* http://ayende.com/blog/4666/ravendb-in-comparison-to-couchdb
* RavenDB - What's the difference, http://codeofrob.com/entries/ravendb---whats-the-difference.html
* RavenDB Documentation, Sharding and Replication

## Cloudant

**Strength**
* Schemaless, JSON-based document datastore as a data management service;
* Tune-able eventual consistency;
* Dynamo-like high and master-less scalability;
* High availability with multi-master replication;
* Full-text search (with Apache Lucene), geo-location services, and flexible, near real-time indexing.

**Weakness**
* Not up for ad-hoc query intensive workloads;
* No real transaction.

**Reference**
* Whitepaper <Technical Overview: Anatomy of the Cloudant DBaaS>




## Azure DocumentDB

**Strength**
* Schemaless, JSON-based document datastore;
* Good performance backed by low-latency, write-optimized, SSD storage;
* SQL-like queries with indexing, async queries via LINQ;
* High Availability and Scalability as a primary goal;
* ACID transactions;
* Tunable consistency model with four modes.

**Weakness**
* No Map/Reduce indexing;
* No aggregation and JOIN;
* No full text search.

**Reference**
* Azure DocumentDB Primer, http://daprlabs.com/blog/blog/2014/08/22/azure-documentdb/
* Query DocumentDB, http://www.documentdb.com/sql/tutorial
* RavenDb vs Azure Document Db, https://groups.google.com/forum/#!topic/ravendb/CEAbfHDGD_g

## RethinkDB

**Strength**
* Schemaless, JSON-based document datastore;
* Efficient execution of queries with advanced indexing, supports table joins and group by;
* High scalability and availability: replication and sharding;
* MVCC, non blocking writes, durability by default;
* Map/Reduce operation support;
* Multi-datacenter replication and failover;
* Easy administration interface.

**Weakness**
* No auto sharding;
* No full ACID transaction;
* Trading off write availability in favor of data consistency.

**Reference**
* Technical comparison: RethinkDB and MongoDB, http://rethinkdb.com/docs/comparison-tables/
* RethinkDB architecture details
* http://rethinkdb.com/docs/architecture/




## JumboDB

**Strength**
* Geared towards massive data processing and indexing data in a parallelized environment like Hadoop;
* Easy parallelization, preorganized and sorted data for better, faster search;
* Sorted data allows grouped read actions;
* Compression: increase disk speed.

**Weakness**
* No SQL;
* Not for data platforms other than Apache Hadoop;
* Cannot update single documents.

**Reference**
* https://github.com/comsysto/jumbodb

## VoltDB

**Strength**
* A relational in-memory NewSQL database system for high-throughput, operational applications;
* Data and processing associated with it are distributed together to a single thread: no multi-threading and locking overhead;
* ACID transactions;
* SQL as native language;
* Near linear scalability;
* High availability: data automatically replicated for intra- and inter-cluster;

**Weakness**
* Limited concurrency;
* Limitation on complex query;
* Limits on database size.

**Reference**
* Whitepaper, <VoltDB technology overview>
* Introduction to VoltDB, http://www.ibm.com/developerworks/library/os-voltdb/
* Comparing VoltDB to Postgres, http://pgsnake.blogspot.com/2010/05/comparing-voltdb-to-postgres.html
