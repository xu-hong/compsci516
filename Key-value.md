# Key-value store

## Couchbase

**Strength**
* Flexible data model, schemaless, JSON-based document datastore or key-value store;
* Elastic scalability: auto-sharding and consistent hashing;
* Availability through replication;
* Persistence to disk;
* Provides memcached-style in-memory caching buckets for metadata;
* Consistent, supports concurrent write with fine-grained locking;
* Friendly cluster-management web GUI;
* Cross-data center replication.

**Weakness**
* Indexing mechanisms not well developed;
* JSON support is relatively immature;
* Does not support range sharding.

**Reference**
* Couchbase Server Architecture and Capabilities, http://www.couchbase.com/nosql-databases/about-couchbase-server#ElasticScalability
* White Paper, Why NoSQL
* NoSQL Showdown, http://www.javaworld.com/article/2078750/open-source-tools/nosql-showdown--mongodb-vs--couchbase.html


## Riak

**Strength**
* Flexible data model, schemaless, key-value store;
* Elastic scalability: auto-sharding and consistent hashing;
* Availability through replication and cross-data center replication;
* Persistence to disk;
* Excels at high volume writing;
* Concurrency using vector clocks, which doesn’t need the nodes (or clients) clocks to be synchronized;
* Friendly cluster-management web GUI – Riak Control.

**Weakness**
* No support for JOIN;
* No SQL or SQL-like language;
* No ACID transactions;
* Availability over consistency: a master-less system which is eventual consistent.

***Reference**
* White Paper, From Relational to Riak – A Technical Brief
* Basho Riak - NoSQL Key Value Store Designed for Scale, http://www.infoq.com/news/2014/10/Riak-NoSQL-designed-for-scale
* http://basho.com/riak-vs-cassandra/


## Cassandra

**Strength**
* Wide-column store based on ideas of BigTable and DynamoDB, able to handle high write volumes;
* Peer-to-peer, no single point of failure;
* Efficient range queries;
* Elastic scalability: auto-sharding and consistent hashing;
* Availability through replication;
* Persistence to disk;
* Cross-data center replication.

**Weakness**
* A more rigid data model since rows are “fixed”;
* No JOIN or aggregate functions supported;
* Writes can be much faster than reads (when reads are disk-bound);
* Transactional AID support except for consistency.

**Reference**
* Cassandra Architecture, http://sergeyenin.com/apache-cassandra-1-1-part-1-basic-architecture
* http://basho.com/riak-vs-cassandra/




## Cassandra.io
Cassandra.io is a hosted and managed Cassandra ring based on Apache Cassandra and makes it accessible via RESTful API.

## DataStax Enterprise
DataStax Enterprise is built upon Cassandra and extends it with:
* Better security;
* Faster I/O with an in-memory transactional database option;
* Faster startup times.

**Reference**
* http://www.datastax.com/documentation/cassandra/1.2/cassandra/features/features_key_c.html
* http://www.datastax.com/what-we-offer/products-services/datastax-enterprise/cassandra

## FatDB

**Strength**
* Flexible data model: key-value or document;
* Tight integration with SQL Server, scale out quickly;
* Flexible data consistency strategies;
* Memory cache with optional disk based persistence;
* Map/Reduce by using distributed LINQ.

**Weakness**
* LINQ queries not yet supported on a memory only (non-persisted) cache;
* Confined in the Windows ecosystem.

**Reference**
* http://www.infoq.com/articles/fatdb



## Voldemort

**Strength**
* Simple key/value data access;
* Persistency based on Berkley DB, a mature and well-known key/value database;
* Concurrency using vector clocks, which doesn’t need the nodes (or clients) clocks to be synchronized;
* Elastic scalability: auto-sharding and consistent hashing;
* Availability through replication;
* Persistence to disk;
* Read faster than Cassandra.

**Weakness**
* No complex query filters;
* All joins must be done in code;
* No foreign key constraints;
* Slower write compared to Cassandra.

**Reference**
* Design – Voldemort, http://www.project-voldemort.com/voldemort/design.html



## Berkeley DB

**Strength**
* Widely used key/value store;
* Support a wide range of operating systems;
* ACID transaction with tunable Isolation;
* Availability through master-slave replication;
* Persistence to disk.

**Weakness**
* No Hadoop integration;
* Berkeley DB is a library rather than a NoSQL solution – on which you need to build one.

**Reference**
* https://blogs.oracle.com/berkeleydb/entry/is_berkeley_db_a_nosql_solutio
* http://www.oracle.com/technetwork/database/database-technologies/berkeleydb/berkeley-db-datasheet-132390.pdf

## Oracle NoSQL
Key-value store based on Berkeley DB Java Edition.

**Strength**
* Flexible data model, schemaless, JSON-based document datastore;
* Elastic scalability: auto-sharding and consistent hashing;
* Availability through master-slave replication;
* Persistence to disk;
* Tunable ACID transaction;
* Concurrency using vector clocks, which doesn’t need the nodes (or clients) clocks to be synchronized;
* Cross-data center replication.

**Weakness**
* No auto detection and rebalance when new nodes are added.

**Reference**
* White paper, Oracle NoSQL Database Compared to MongoDB
* On Oracle NoSQL Database –Interview with Dave Segleau, http://www.odbms.org/blog/2013/07/on-oracle-nosql-database-interview-with-dave-segleau/




## LevelDB

**Strength**
* Fast, lightweight, persistent, key-value store;
* Flexible key/value type, entries sorted by key;
* Priority on random write performance;
* Dependency free;
* Snapshot, which provides a **Reference** to the state of the database at a point in time.

**Weakness**
* A database library without client-server support builtin;
* All leveldb access is done in a single process.

**Reference**
* http://dailyjs.com/2013/04/19/leveldb-and-node-1/
* https://news.ycombinator.com/item?id=2526032


## HyperDex

**Strength**
* One of the richest APIs in the NoSQL space;
* Flexible data model, schemaless, key-value and document store;
* Strongest consistency properties: key operations are linearizable;
* Better, tunable fault tolerance than MongoDB and Cassandra;
* ACID transaction with a minimal performance penalty.

**Weakness**
* No method to do distributed computation;
* No replication across multiple datacenters;
* Young projects with limited support.

**Reference**
* Hyperdex - A closer look, http://www.slideshare.net/DECK36/c36-hyperdexmeetupdec2013v2nogfx
* Hyperdex: The next generation NoSQL, http://hyperdex.org/slides/2013-06-28-cloudphysics.pdf
* http://hyperdex.org/performance/


## MagnetoDB
A key-value store NoSQL service for OpenStack (a cloud computing operating system), MagnetoDB provides:
**Strength**
* Horizontal scalability, 
* High availability,
* Queryable storage,
* Easy integration with REST API.

**Weakness**
* Tightly integrated with OpenStack.

**Reference**
* Introducing MagnetoDB, a key-value storage sevice for OpenStack, https://www.mirantis.com/blog/introducing-magnetodb-nosql-database-service-openstack/


## AWS DynamoDB

**Strength**
* Minimum maintenance: a hosted NoSQL key-value system distributed among Amazon’s servers with automatic partitioning and SSD technologies;
* Elastic, high and seamless scalability;
* Fast performance at high volume writing;
* Efficient range queries;
* Tunable consistency (strong or eventually consistent);
* High availability provided with three geographically distributed replicas;
* Flexible: both document and key-value data structures supported.

**Weakness**
* Not optimal for complex query with multiple predicates;
* The hash key, range key definition can not be changed in future;
* No multi-operation transactions.

**Reference**
* Amazon CTO’s note, http://www.allthingsdistributed.com/2012/01/amazon-dynamodb.html
* Developer Guide, Working with Items, http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/WorkingWithItems.html#WorkingWithItems.AtomicCounters
* DynamoDB Data Model, http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DataModel.html#DataModel.DataTypes
* DynamoDB shortcomings (and our work arounds), https://www.dailycred.com/blog/10/dynamodb-shortcomings-and-our-work-arounds
* Why My Team Went with DynamoDB Over MongoDB, http://news.dice.com/2013/02/21/why-my-team-went-with-dynamodb-over-mongodb/



## AWS SimpleDB

**Strength**
* Simplicity: automatically indexes all item attributes, easily retrieve or edit through a simple set of API calls;
* Tunable consistency (strong or Eventually Consistent);
* High availability provided with multiple geographically distributed replicas;
* Low cost compared to DynamoDB.

**Weakness**
* Weaker performance/scalability compared to DynamoDB.

**Reference**
* http://stackoverflow.com/questions/8961333/amazon-simpledb-vs-amazon-dynamodb
* http://aws.amazon.com/simpledb/




## FoundationDB

**Strength**
* Multiple data models supported: ordered key-value store supporting higher-level models as "layers";
* SQL queries available using SQL Layer; 
* Serializable, multi-key ACID transactions;
* Availability through replication;
* Strong consistency;
* Persistence to disk;
* Cross data center replication.

**Weakness**
* Limitation on long or large transactions;
* Limitation on large key or values;
* Limitation on cluster size and database size.

**Reference**
* Key value store, user tutorials, https://foundationdb.com/key-value-store/documentation/tutorials.html
* Known limitations, https://foundationdb.com/key-value-store/documentation/known-limitations.html
* FoundationDB extends performance and scalability with Version 3.0, http://sdtimes.com/foundationdb-extends-performance-scalability-version-3-0/



## Aerospike

**Strength**
* Speed: in-memory key-value store;
* Tunable persistence to backed storage;
* Highly parallelized multi-threaded coded in C;
* Scale both up and out;
* Reliability with auto replication;
* Tunable consistency (strong or Eventually Consistent);
* Asynch cross data center replication.

**Weakness**
* Not optimal for complex query with multiple predicates;
* No real ACID transaction.

**Reference**
* A Quest for database scale, http://highscalability.com/blog/2014/5/6/the-quest-for-database-scale-the-1-m-tps-challenge-three-des.html
* Aerospike doubles performance, shows 1 M TPS in YCSB tests, https://foundationdb.com/key-value-store/versus



## ArangoDB

**Strength**
* Flexible data model for documents, graphs, and key-values;
* Convenient joins and SQL-like (AQL) queries supported;
* ACID transactions supported;
* Scale both up and out;
* Reliability by replication and automatic failover organization;
* Multiple platforms supported.

**Weakness**
* No support for map/reduce;
* Though ArangoDB is a universal approach, there are edge cases where it is not recommended.

**Reference**
* Whitepaper, The new sharding feature in ArangoDB 2.0
* Comparison of NoSQL Solutions, Alex, Sidney, Shubha.



## CortexDB

**Strength**
* Flexible data model for documents, graphs, and key-values;
* A temporal database includes valid time and transaction time.

**Weakness**
* Very few support and documentations.

**Reference**
* http://www.odbms.org/2014/04/cortexdb/

## Sqrrl  Enterprise  

**Strength**
* Graph oriented, JSON-based document data structure;
* SqrrlQL allows for selective retrieval and manipulation of linked data graph structures;
* Comprehensive, end-to-end Data-Centric Security;
* Massive scalability given by Apache Accumulo.

**Weakness**
* Weak in global queries and number crunching;
* Weak for binary data store.

**Reference**
* http://sqrrl.com/sqrrl-enterprise-3-databases-in-1-column-document-graph/
* Graph Databases, https://www.fbi.h-da.de/fileadmin/personal/u.stoerl/DBAkt-WS1415/Vorlesung/DBAkt-WS1415-GraphDB-11-Storage-Retrieval-part2.pdf
