*Infinispan

**Strength**
*In-memory access: fast;
*Schema-less key/value overcoming the constraints of traditional database;
*Can be used as local cache and as clustered caches as well, which can linearly scale out; 
*Scalable data partitioning across cluster, providing fault tolerance;
*Elastic with consistent hashing, availability during topology changes;
*Support for access to caches either transactionally or non-transactionally;
*Greater concurrency with multiversion concurrency control;
*Support for Write-Through And Write-Behind Caching to persistent storage.

**Weakness**
*Migrating from SQL to Map-like API is not easy;
*More apt to complement traditional database rather than to replace it;
*Network bandwidth may become the bottleneck;
*Less strict schema may require more validation on application data layer.

**Reference**
*Data Grids vs Databases,  http://www.slideshare.net/galderz/data-grids-vs-databases
*Data Grids and Data Caching, http://www.slideshare.net/galderz/data-grids-and-data-caching
*Wikipedia, MVCC, http://en.wikipedia.org/wiki/Multiversion_concurrency_control
*Jags Ramnarayan on In-Memory Data Grids, http://www.infoq.com/articles/in-memory-data-grids


*Red Hat JBoss Data Grid  

**Strength** and the **Weakness**: same as Infinispan (since it is an ecosystem which is built around Infinispan)
***Reference**
*White paper, <Red Hat JBoss Data Grid 6.4 Beta Getting Started Guide>
*White paper, <Improving Application Scalability with In-Memory Data Grids>
*GridGain  

**Strength**
*Integrate fast In-Memory MapReduce implementation;
*Geared towards in-memory near real time computations and low latencies, support affinity co-location;
*Scalable data partitioning across cluster, providing fault tolerance;
*Support for access to caches either transactionally or non-transactionally;
*Support for async repartitioning or delayed repartitioning;
*Greater concurrency with multiversion concurrency control;
*Support for off heap data overflow to better work with JVM Garbage Collection;
*Schema-less key/value to overcome the constraints of traditional database;
*Also allow standard SQL to query in-memory data as well as distributed join,
*Support for Write-Through And Write-Behind Caching to persistent storage.
***Weakness**
*More apt to complement traditional database rather than to replace it;
*Network bandwidth may become the bottleneck.
*Less strict schema may require more validation on application data layer.
***Reference**
*synergies/
*In-Memory Data Grid: Explained, http://gridgain.com/in-memory-data-grid-explained/
*In-Memory Data Fabric, http://gridgain.com/products/in-memory-data-fabric/


*Hazelcast

**Strength**
*Easy scale out by adding nodes, dynamically rebalance data across the new grid.; 
*Elastic with consistent hashing: availability during topology changes;
*Support for access to caches either transactionally or non-transactionally;
*Greater concurrency with multiversion concurrency control;
*Schema-less key/value to overcome the constraints of traditional database.

**Weakness**
*No support for Fully Replicated architecture in peer-to-peer mode;
*No in memory streaming;
*No async repartitioning or delayed repartitioning;
*More apt to complement traditional database rather than to replace it;
*Network bandwidth may become the bottleneck;
*Less strict schema may require more validation on application data layer.

**Reference**
*Java Caches: Ehcache, Hazelcast, Infinispan, https://labs.consol.de/java-caches/
*White paper, <GridGain vs. Hazelcast Feature Comparison>



*Ehcache

**Strength**
*Fast, easy-to-set-up and light weight in-memory data grids (IMDG);
*Scalable data partitioning across cluster, providing fault tolerance;
*Seamless integration as a second-level cache for Hibernate.

**Weakness**
*repartitioning or delayed repartitioning or other advanced features;
*No support for other languages besides Java;
*More apt to complement traditional database rather than to replace it.

**Reference**
*http://ehcache.org/about/features
*http://ehcache.org/documentation/2.6/get-started/about-distributed-cache
*BigMemory
*Collection
*CloudTran

**Strength**
*guaranteed persistence to databases; 
*transactionality with optimized 2-Phase Commit (2PC).

**Weakness**
*Mainly invented for the purpose of improving Coherence;
*The emphasis on transaction might impede its performance.
***Reference**
*White paper,  <CloudTran Technology Genesis>


*Oracle Coherence

**Strength**
*query and parallel transaction processing, etc.

**Weakness**
*Licensing model.

**Reference**
*White paper <ORACLE COHERENCE 12C>
*IBM eXtreme Scale  
*IBM’s counterpart of Oracle Coherence: 
*Better integration with WAS; 
*failure or maintenance; 
*Less expensive price.

**Reference**
*http://whywebsphere.com/2012/07/03/data-grids-and-caching-ibm-or-oracle/
*Redbook, < WebSphere eXtreme Scale V8.6 Key Concepts and Usage Scenarios>

*Memcached

**Strength**
*Simple yet fast;
*Better use of memory with distributed memory object caching;
*database load;
*Near O(1) for every memcached operation.
***Weakness**
*Not a good fit for persistent storage;
*No clustering thus no consistency provided;
*Unreliable;
*Scaling requires code update on client applications.
***Reference**
*http://parsa.epfl.ch/cloudsuite/memcached.html
*https://code.google.com/p/memcached/wiki/NewStart
*AWS ElastiCache, AWS ElastiCache with Redis
*possesses the **Strength** of that of Memcached and also adds:
**Strength**
*Simple to deploy and manage with management console or simple APIs;
*Enhancement in elasticity and scalability, auto discover of new nodes;
*Enhancement in reliability through auto failure detection and recovery.

**Weakness**
*No clustering thus no consistency provided.
***Reference**
*in/2012/11/amazon-elasticache-memcached-ec2.html
*Amazon ElastiCache User Guide


*RedisLabs Memcached Cloud
*safe manner.

**Strength**
*Enhancement in reliability through auto failure detection and recovery;
*Backup to and imports from FTP server and other cloud storages;
*Enhancement in elasticity and scalability.
***Reference**
*https://redislabs.com/memcached-cloud
*RedisLabs Redis Cloud
*scalable manner.

**Strength**
*Enhancement in availability;
*Backup to and imports from FTP server and other cloud storages;
*Enhancement in elasticity and scalability.
***Reference**
*https://redislabs.com/redis-cloud

*Memcachier
*MemCachier manages and scales clusters of memcache servers. 

**Strength**
*Enhancement in reliability through auto failure detection and recovery;
*Enhancement in elasticity and scalability;
*Analytics dashboard provided to monitor cache usage.

**Reference**
*https://www.memcachier.com/how-it-works



*GigaSpaces XAP

**Strength**
*Veteran product in IMDG market; 
*In-memory access: fast;
*Scalable data partitioning across cluster, providing fault tolerance;
*Elastic with consistent hashing: availability during topology changes;
*Support for access to caches either transactionally or non-transactionally;
*Schema-less key/value to overcome the constraints of traditional database;
*Support for replication across data centers.

**Weakness**
*More apt to complement traditional database rather than to replace it;
*Network bandwidth may become the bottleneck;
*Less strict schema may require more validation on application data layer.

**Reference**
*http://www.gigaspaces.com/xap-high-availability-load-balancing/how-it-works
*White Paper, < Elastic Caching Platforms, Q2 2010>
*TIBCO  ActiveSpaces

**Strength**
*Support SQL-like query to in-memory data;
*Configurable data purging: allows Time-to-live (TTL) to be set for in-memory caches;
*Scalable data partitioning across cluster, providing fault tolerance;
*Elastic with consistent hashing: availability during topology changes;
*Support for access to caches either transactionally or non-transactionally;
*Schema-less key/value to overcome the constraints of traditional database;

**Weakness**
*More apt to complement traditional database rather than to replace it;
*Network bandwidth may become the bottleneck;
*Less strict schema may require more validation on application data layer.

**Reference**
*White Paper, < TIBCO ActiveSpaces Use Cases>
*Pivotal  GemFire  

**Strength**
*Schema-less key/value to overcome the constraints of traditional database;
*intelligence;
*Consistency across geo-distributed applications;
*Highly scalable data partitioning across cluster, providing fault tolerance;
*Support for access to caches either transactionally or non-transactionally;
*Easy monitoring and management.

**Weakness**
*Licensing model, very costly;
*Complex configuration;
*More apt to complement traditional database rather than to replace it;
*Network bandwidth may become the bottleneck.

**Reference**
*White Paper, < Elastic Caching Platforms, Q2 2010>
*http://www.vmware.com/products/vfabric-gemfire/features.html
*Pivotal  GemFire  XD 
*be optimized with indexes on key values.
**Reference**: http://www.pivotal.io/big-data/pivotal-gemfire-xd

*Scaleout Software

**Strength**
*execution time;
*Support for replication between data centers for disaster recovery;
*applications/computations;
*Support for access to caches either transactionally or non-transactionally;
*Schema-less key/value to overcome the constraints of traditional database.

**Weakness**
*Licensing model;
*Complex configuration;
*More apt to complement traditional database rather than to replace it;
*Network bandwidth may become the bottleneck.

**Reference**
*ScaleOut hServer V2 Java Programmer's Guide

*IronCache

**Strength**
*Configurable data purging: allows Time-to-live (TTL) to be set for in-memory caches;
*Developer friendly interface with IronMQ; 
*Full visibility into caches and usage with the Iron.io user interface;
*applications/computations;
*Elastic with consistent hashing: availability during topology changes;
*Support for access to caches either transactionally or non-transactionally;
*Schema-less key/value to overcome the constraints of traditional database.

**Weakness**
*More apt to complement traditional database rather than to replace it;
*Network bandwidth may become the bottleneck;
*Less strict schema may require more validation on application data layer.

**Reference**
*https://devcenter.heroku.com/articles/iron_cache
*http://www.iron.io/worker
*Redis

**Strength**
*Very fast, good concurrency support;
*In-memory key-value store for database calls, with flexibility of the objects it can cache;
*Fine-grained control over eviction;
*Master-slave replication supported to ensure highly availability;
*Transaction supported with optimistic locking;
*Persistence to disk;
*Scalability when used as cache;
***Weakness**
*Immature clustering thus no consistency provided;
*Dataset size limited to computer RAM;
*No scalability when used as data store (Redis Cluster is currently in beta).

**Reference**
*http://redis.io/topics/transactions
*an-rdbms
*caching.html
*ObjectRocket Redis, RedisGreen, Redis-to-go
*Commercial product build around Redis with 24x7x365 support and easy interface.

**Reference**
*https://objectrocket.com/redis/
*http://www.redisgreen.net/
*http://redistogo.com/


*Couchbase

**Strength**
*Flexible data model, schemaless, JSON-based document datastore or key-value store;
*Elastic scalability: auto-sharding and consistent hashing;
*Availability through replication;
*Persistence to disk;
*Provides memcached-style in-memory caching buckets for metadata;
*Consistent, supports concurrent write with fine-grained locking;
*Friendly cluster-management web GUI;
*Cross-data center replication.

**Weakness**
*Indexing mechanisms not well developed;
*JSON support is relatively immature;
*Does not support range sharding.

**Reference**
*couchbase-server#ElasticScalability
*White Paper, < Why NoSQL>
*--couchbase.html
*Riak

**Strength**
*Flexible data model, schemaless, key-value store;
*Elastic scalability: auto-sharding and consistent hashing;
*Availability through replication and cross-data center replication;
*Persistence to disk;
*Excels at high volume writing;
*Concurrency using vector clocks, which doesn’t need the nodes (or clients) clocks to be synchronized;
*Friendly cluster-management web GUI – Riak Control.

**Weakness**
*No support for JOIN;
*No SQL or SQL-like language;
*No ACID transactions;
*Availability over consistency: a master-less system which is eventual consistent.
***Reference**
*White Paper, <From Relational to Riak – A Technical Brief>
*designed-for-scale
*http://basho.com/riak-vs-cassandra/


*Cassandra

**Strength**
*Wide-column store based on ideas of BigTable and DynamoDB, able to handle high write volumes;
*Peer-to-peer, no single point of failure;
*Efficient range queries;
*Elastic scalability: auto-sharding and consistent hashing;
*Availability through replication;
*Persistence to disk;
*Cross-data center replication.

**Weakness**
*A more rigid data model since rows are “fixed”;
*No JOIN or aggregate functions supported;
*Writes can be much faster than reads (when reads are disk-bound);
*Transactional AID support except for consistency.

**Reference**
*Cassandra Architecture, http://sergeyenin.com/apache-cassandra-1-1-part-1-basic-architecture
*http://basho.com/riak-vs-cassandra/
*Cassandra.io
*accessible via RESTful API.
*DataStax Enterprise
*DataStax Enterprise is built upon Cassandra and extends it with:
*Better security;
*Faster I/O with an in-memory transactional database option;
*Faster startup times.
***Reference**
*http://www.datastax.com/documentation/cassandra/1.2/cassandra/features/features_key_c.html
*http://www.datastax.com/what-we-offer/products-services/datastax-enterprise/cassandra

*FatDB

**Strength**
*Flexible data model: key-value or document;
*Tight integration with SQL Server, scale out quickly;
*Flexible data consistency strategies;
*Memory cache with optional disk based persistence;
*Map/Reduce by using distributed LINQ;
***Weakness**
*LINQ queries not yet supported on a memory only (non-persisted) cache;
*Confined in the Windows ecosystem.
***Reference**
*http://www.infoq.com/articles/fatdb
*Voldemort

**Strength**
*Simple key/value data access;
*Persistency based on Berkley DB, a mature and well-known key/value database;
*Concurrency using vector clocks, which doesn’t need the nodes (or clients) clocks to be synchronized;
*Elastic scalability: auto-sharding and consistent hashing;
*Availability through replication;
*Persistence to disk;
*Read faster than Cassandra.

**Weakness**
*No complex query filters;
*All joins must be done in code;
*No foreign key constraints;
*Slower write compared to Cassandra.
***Reference**
*Design – Voldemort, http://www.project-voldemort.com/voldemort/design.html
*Berkeley DB

**Strength**
*Widely used key/value store;
*Support a wide range of operating systems;
*ACID transaction with tunable Isolation;
*Availability through master-slave replication;
*Persistence to disk.
***Weakness**
*No Hadoop integration;
*Berkeley DB is a library rather than a NoSQL solution – on which you need to build one.

**Reference**
*https://blogs.oracle.com/berkeleydb/entry/is_berkeley_db_a_nosql_solutio
*132390.pdf

*Oracle NoSQL
*Key-value store based on Berkeley DB Java Edition.

**Strength**
*Flexible data model, schemaless, JSON-based document datastore;
*Elastic scalability: auto-sharding and consistent hashing;
*Availability through master-slave replication;
*Persistence to disk;
*Tunable ACID transaction;
*Concurrency using vector clocks, which doesn’t need the nodes (or clients) clocks to be synchronized;
*Cross-data center replication.

**Weakness**
*No auto detection and rebalance when new nodes are added.
***Reference**
*White paper, <Oracle NoSQL Database Compared to MongoDB>
*nosql-database-interview-with-dave-segleau/
*LevelDB
**Strength**
*Fast, lightweight, persistent, key-value store;
*Flexible key/value type, entries sorted by key;
*Priority on random write performance;
*Dependency free;
*Snapshot, which provides a **Reference** to the state of the database at a point in time.

**Weakness**
*A database library without client-server support builtin;
*All leveldb access is done in a single process.

**Reference**
*http://dailyjs.com/2013/04/19/leveldb-and-node-1/
*https://news.ycombinator.com/item?id=2526032


*HyperDex

**Strength**
*One of the richest APIs in the NoSQL space;
*Flexible data model, schemaless, key-value and document store;
*Strongest consistency properties: key operations are linearizable;
*Better, tunable fault tolerance than MongoDB and Cassandra;
*ACID transaction with a minimal performance penalty.

**Weakness**
*No method to do distributed computation;
*No replication across multiple datacenters;
*Young projects with limited support.
***Reference**
*<Hyperdex - A closer look>, http://www.slideshare.net/DECK36/c36-hyperdexmeetupdec2013v2nogfx
*<Hyperdex: The next generation NoSQL>, http://hyperdex.org/slides/2013-06-28-cloudphysics.pdf
*http://hyperdex.org/performance/
*MagnetoDB

**Strength**
*provides:
*horizontal scalability, 
*high availability,
*queryable storage,
*easy integration with REST API.

**Weakness**
*Tightly integrated with OpenStack.

**Reference**
*com/blog/introducing-magnetodb-nosql-database-service-openstack/

*AWS DynamoDB

**Strength**
*automatic partitioning and SSD technologies;
*Elastic, high and seamless scalability;
*Fast performance at high volume writing;
*Efficient range queries;
*Tunable consistency (strong or Eventually Consistent);
*High availability provided with three geographically distributed replicas;
*Flexible: both document and key-value data structures supported.
***Weakness**
*Not optimal for complex query with multiple predicates;
*The hash key, range key definition can not be changed in future;
*No multi-operation transactions.
***Reference**
*Amazon CTO’s note, http://www.allthingsdistributed.com/2012/01/amazon-dynamodb.html
*com/amazondynamodb/latest/developerguide/WorkingWithItems.html#WorkingWithItems.AtomicCounters
*html#DataModel.DataTypes
*-and-our-work-arounds
*dynamodb-over-mongodb/

*AWS SimpleDB

**Strength**
*of API calls;
*Tunable consistency (strong or Eventually Consistent);
*High availability provided with multiple geographically distributed replicas;
*Low cost compared to DynamoDB.

**Weakness**
*Weaker performance/scalability compared to DynamoDB.

**Reference**
*http://stackoverflow.com/questions/8961333/amazon-simpledb-vs-amazon-dynamodb
*http://aws.amazon.com/simpledb/

*FoundationDB

**Strength**
*Multiple data models supported: ordered key-value store supporting higher-level models as "layers";
*SQL queries available using SQL Layer; 
*Serializable, multi-key ACID transactions;
*Availability through replication;
*Strong consistency;
*Persistence to disk;
*Cross data center replication.

**Weakness**
*Limitation on long or large transactions;
*Limitation on large key or values;
*Limitation on cluster size and database size.
***Reference**
*html
*Known limitations, https://foundationdb.com/key-value-store/documentation/known-limitations.html
*FoundationDB extends performance and scalability with Version 3.0,
*http://sdtimes.com/foundationdb-extends-performance-scalability-version-3-0/
*Aerospike

**Strength**
*Speed: in-memory key-value store;
*Tunable persistence to backed storage;
*Highly parallelized multi-threaded coded in C;
*Scale both up and out;
*Reliability with auto replication;
*Tunable consistency (strong or Eventually Consistent);
*Asynch cross data center replication.

**Weakness**
*Not optimal for complex query with multiple predicates;
*No real ACID transaction.
***Reference**
*-1-m-tps-challenge-three-des.html
*Aerospike doubles performance, shows 1 M TPS in YCSB tests
*https://foundationdb.com/key-value-store/versus


*ArangoDB

**Strength**
*Flexible data model for documents, graphs, and key-values;
*Convenient joins and SQL-like (AQL) queries supported;
*ACID transactions supported;
*Scale both up and out;
*Reliability by replication and automatic failover organization;
*Multiple platforms supported.

**Weakness**
*No support for map/reduce;
*Though ArangoDB is a universal approach, there are edge cases where it is
*not recommended.

**Reference**
*Whitepaper, The new sharding feature in ArangoDB 2.0
*Comparison of NoSQL Solutions, Alex, Sidney, Shubha.
*CortexDB

**Strength**
*Flexible data model for documents, graphs, and key-values;
*A temporal database includes valid time and transaction time.

**Weakness**
*Very few support and documentations.

**Reference**
*http://www.odbms.org/2014/04/cortexdb/

*Sqrrl  Enterprise  

**Strength**
*Graph oriented, JSON-based document data structure;
*SqrrlQL allows for selective retrieval and manipulation of linked data graph structures;
*Comprehensive, end-to-end Data-Centric Security;
*Massive scalability given by Apache Accumulo.

**Weakness**
*Weak in global queries and number crunching;
*Weak for binary data store.

**Reference**
*http://sqrrl.com/sqrrl-enterprise-3-databases-in-1-column-document-graph/
*WS1415-GraphDB-11-Storage-Retrieval-part2.pdf
*MarkLogic

**Strength**
*Document-based data model with support for multiple data types;
*Support query with SPARQL; 
*Only Enterprise NoSQL database with built-in search capabilities;
*HDFS;
*High scalability and availability;
*Tunable transaction mode, true ACID transactions.
***Reference**
*Whitepaper, <Inside MarkLogic Server> 
*OrientDB

**Strength**
*Flexible data model for documents, graphs, and key-values;
*Convenient joins and SQL queries supported;
*ACID transactions supported;
*Elastic Distributed scalability added by Hazelcast;
*Reliability by replication and automatic failover organization.

**Weakness**
*JVM compatible;
*Possible single point of failure.  

**Reference**
*https://github.com/orientechnologies/orientdb/wiki/Distributed-Sharding
*http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis

*YarcData
**Strength**
*Business-focused real-time graph analytics platform;
*Optimized for compute-heavy, memory-centric;

**Weakness**
*Very few documents.
***Reference**
*Whitepaper, CrayUrikaXA-Technical-Specs

*Neo4j

**Strength**
*Native graph storage with flexible schema;
*SQL queries supported with Cypher;
*ACID transactions supported;
*High availability via a master-slave HA protocol.

**Weakness**
*Optimized for reads, not write;
*Weak in global queries and number crunching;
*Weak for binary data store;
*Possible single point of failure.  

**Reference**
*http://neo4j.com/developer/graph-db-vs-nosql/
*http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis
*<A Comparison of Current Graph Database Models>, Renzo Angles, Universidad de Talca (Chile)
*GrapheneDB
*A Neo4j database host platform with support, 24X7 monitoring, and backups provided.
*http://docs.graphenedb.com/getting-started.html

*Sparksee

**Strength**
*Compact representation of graph storage using bitmaps, high throughput and fast speed; 
*High availability via a master-slave HA protocol;
*First graph database on Android and iOS.

**Weakness**
*Partial transactional;
*No query language;
*Possible single point of failure.  
***Reference**
*overview
*Sparksee Archetecture
*http://www.sparsity-technologies.com/HighAvailability/Architecture.html

*FlockDB

**Strength**
*Distributed graph database for storing adjacency lists;
*Optimized for a high rate of add/update/remove operations;
*Simple, small, lightweight solution tailored for Twitter.

**Weakness**
*Not built for multi-hop queries (or graph-walking queries) or automatic shard migrations
*No transaction;
*No query language (can add query using Gizzard);
*Availability and scalability come through Gizzard.

**Reference**
*https://blog.twitter.com/2010/introducing-flockdb
*https://github.com/twitter/flockdb

*Stardog

**Strength**
*Lightweight graph database on RDF data model;
*Query supported: SPARQL;
*ACID transactions supported;
*High availability via a master-slave HA protocol;
*OWL & Rule Reasoning: semantic search.

**Weakness**
*Weak in number crunching;
*Weak for binary data store;
*Possible single point of failure.  

**Reference**
*The Stardog Manual
*http://docs.stardog.com
*Titan

**Strength**
*Linear, elastic scalable graph database, optimized for handling thousands of concurrent transactions;
*Data distribution and replication for performance and fault tolerance, no single point failure;
*Multicenter high availability;
*ACID transaction;
*Support for various storage backends;
*Support for graph query with Gremlin.
***Weakness**
*Niche in multiple short, local queries;
*No search capabilities built within (search capability comes with indexing service such as Lucene)
***Reference**
*Titan vs Neo4J, https://groups.google.com/forum/#!msg/aureliusgraphs/vkQkzjN8fo0/9YYgqI4TA0QJ
*Titan Documentation,
*http://thinkaurelius.github.io/titan/
*AffinityDB

**Strength**
*Graph database geared towards embedded information-processing, control and communication;
*SQL queries supported with pathSQL;
*ACID transactions supported.

**Weakness**
*Scalability and high availability.

**Reference**
*http://affinityng.cfapps.io/doc/**Strength**s.html
*http://affinityng.cfapps.io/doc/features.html


*Trinity

**Strength**
*Fast, distributed graph system over a memory cloud;
*Highly compact in-memory access geared for parallel computing;
*Rich system management and development tools.

**Weakness**
*No ACID transaction;
*No query language;
*Limited scalability and availability.
***Reference**
*<Trinity: A Distributed Graph Engine on a Memory Cloud>, Bin Shao et al, ACM SIGMOD
*SPARQL

**Strength**
*Graph database on RDF data model for high performance graph analysis;
*Standard based (Solely built around W3C standards, SPARQL, RDF);
*ACID transaction;
*High scalability;
*High availability provided by backed HDFS.

**Weakness**
*No flexible choice for native store;
*No fault tolerance beyond native storage level. 
***Reference**
*SPARQLverse Guide
*Apache Giraph

**Strength**
*Iterative graph processing system built for high scalability;
*Optimized for batch processing of massive graphs;
*Faster: it loads an entire graph into a cluster's memory;

**Weakness**
*Limited supported size of the graph;
*No fault tolerance beyond Hadoop. 
***Reference**
*Giraph User Guide
*com/2012/12/scalable-graph-processing-comparing.html
*Giraph for Large Multigraphs,
*http://xinhstechblog.blogspot.com/2012/10/giraph-for-large-multigraphs.html

*AllegroGraph

**Strength**
*storage;
*Designed for maximum loading speed and query speed for large files;
*Full Read Concurrency, Near Full Write Concurrency;
*ACID transaction;
*LISP-based development tools.

**Weakness**
*Proprietary product;
*Availability.

**Reference**
*AllegroGraph Introduction,
*http://franz.com/agraph/support/documentation/current/warm-standby.html#header2-8
*http://franz.com/agraph/allegrograph/
*HyperGraphDB

**Strength**
*Object-oriented multi-relational labeled hypergraph;
*A persistent memory model designed mostly for knowledge management, AI and semantic web projects;
*database, or a (non-SQL) relational database;
*Non-blocking concurrent writes and reads;
*Size limitations virtually non-existent;
*P2P framework: no single point of failure.

**Weakness**
*No ACID transaction;
*Scalability.

**Reference**
*<Data Management for Complex Systems>, http://www.hypergraphdb.org/docs/HyperGraphDB-Presentation.pdf
*InfiniteGraph

**Strength**
*Labeled and directed multi-property-graph optimized for data relationships;
*ACID transaction;
*Elastic scalability;
*High availability.

**Weakness**
*No query language, just API.

**Reference**
*InfiniteGraph Technical Specifications


*MongoDB

**Strength**
*Schemaless, JSON-based document datastore;
*High scalability: replication and auto-sharding;
*Replication across data centers;
*Efficient execution of queries with indexing;
*Map/Reduce operation support.

**Weakness**
*Map/Reduce performance;
*Less efficient usage of storage;
*Less flexibility in querying (no JOIN);
*No transactions except for certain atomic operations at a single document level.
***Reference**
*http://stackoverflow.com/questions/5244437/pros-and-cons-of-mongodb
*MongoDB manual
*MongoLab
*Fully-managed MongoDB-as-a-Service with data protection and expert support.
*TokuMX
*An open source, high-performance distribution of MongoDB with improvements in:
*Better caching and document-level locking: 50x performance improvements;
*Advanced compression: 90% reduction in database size;
*Support for ACID transactions and MVCC.

**Reference**
*http://www.tokutek.com/tokumx-for-mongodb/
*CouchDB

**Strength**
*Schemaless, JSON-based document datastore;
*ACID transaction, multi-version concurrency control;
*High availability with “shared nothing” replication;
*Efficient execution of queries with the view model for looking up and aggregating;
*Map/Reduce operation support,
*Compaction for more efficient use of storage.

**Weakness**
*No scalability “out-of-the-box” with sharding;
*Transaction only on a single document.

**Reference**
*CouchDB, Guide to Views
*CouchDB, Technical Overview
*Iris Couch
*Free CouchDB hosting service
*Compose
*SSD backed.
*RavenDB

**Strength**
*Schemaless, JSON-based document datastore for .NET;
*ACID transaction for single or multi documents;
*High scalability: replication and sharding;
*High availability;
*Geared to massive and fast reads with efficient querying using Linq;
*Map/Reduce operation support;
*Compaction for more efficient use of storage.

**Weakness**
*Need to define your own sharding strategy.

**Reference**
*http://ayende.com/blog/4666/ravendb-in-comparison-to-couchdb
*RavenDB - What's the difference, http://codeofrob.com/entries/ravendb---whats-the-difference.html
*RavenDB Documentation, Sharding and Replication

*Cloudant

**Strength**
*Schemaless, JSON-based document datastore as a data management service;
*Tune-able eventual consistency;
*Dynamo-like high and master-less scalability;
*High availability with multi-master replication;
*Full-text search (with Apache Lucene), geo-location services, and flexible, near real-time indexing.

**Weakness**
*Not up for ad-hoc query intensive workloads;
*No real transaction.
***Reference**
*Whitepaper <Technical Overview: Anatomy of the Cloudant DBaaS>
*Azure DocumentDB

**Strength**
*Schemaless, JSON-based document datastore;
*Good performance backed by low-latency, write-optimized, SSD storage;
*SQL-like queries with indexing, async queries via LINQ;
*High Availability and Scalability as a primary goal;
*ACID transactions;
*Tunable consistency model with four modes.

**Weakness**
*No Map/Reduce indexing;
*No aggregation and JOIN;
*No full text search.

**Reference**
*Azure DocumentDB Primer, http://daprlabs.com/blog/blog/2014/08/22/azure-documentdb/
*Query DocumentDB, http://www.documentdb.com/sql/tutorial
*RavenDb vs Azure Document Db, https://groups.google.com/forum/#!topic/ravendb/CEAbfHDGD_g

*RethinkDB

**Strength**
*Schemaless, JSON-based document datastore;
*Efficient execution of queries with advanced indexing, supports table joins and group by;
*High scalability and availability: replication and sharding;
*MVCC, non blocking writes, durability by default;
*Map/Reduce operation support;
*Multi-datacenter replication and failover;
*Easy administration interface.

**Weakness**
*No auto sharding;
*No full ACID transaction;
*Trading off write availability in favor of data consistency.

**Reference**
*Technical comparison: RethinkDB and MongoDB, http://rethinkdb.com/docs/comparison-tables/
*RethinkDB architecture details
*http://rethinkdb.com/docs/architecture/
*JumboDB

**Strength**
*Geared towards massive data processing and indexing data in a parallelized environment like Hadoop;
*Easy parallelization, preorganized and sorted data for better, faster search;
*Sorted data allows grouped read actions;
*Compression: increase disk speed.

**Weakness**
*No SQL;
*Not for data platforms other than Apache Hadoop;
*Cannot update single documents.

**Reference**
*https://github.com/comsysto/jumbodb

*VoltDB
**Strength**
*A relational in-memory NewSQL database system for high-throughput, operational applications;
*threading and locking overhead;
*ACID transactions;
*SQL as native language;
*Near linear scalability;
*High availability: data automatically replicated for intra- and inter-cluster;

**Weakness**
*Limited concurrency;
*Limitation on complex query;
*Limits on database size.

**Reference**
*Whitepaper, <VoltDB technology overview>
*Introduction to VoltDB, http://www.ibm.com/developerworks/library/os-voltdb/
*Comparing VoltDB to Postgres, http://pgsnake.blogspot.com/2010/05/comparing-voltdb-to-postgres.html

*MemSQL

**Strength**
*A relational in-memory NewSQL database system for high-throughput, operational applications;
*Efficient columnar compression;
*Multiversion concurrency control: querying even as real-time data streams into the system;
*ACID transactions;
*SQL as native language;
*Near linear scalability;
*High availability: data automatically replicated for intra- and inter-cluster.

**Weakness**
*Isolation level is read committed;
*Limits on database size.

**Reference**
*http://www.memsql.com/features/
*Oracle database 12c

**Strength**
*applications;
*ACID transactions;
*SQL as native language;
*Support for both OLTP and data warehousing;
*High availability: data automatically replicated for intra- and inter-cluster;
*Easy administrative tools.

**Weakness**
*High cost;
*Proprietary.

**Reference**
*White paper,  <Automatic Data Optimization with Oracle Database 12c>
*12c documentation, Database High Availability Overview

*IBM DB2

**Strength**
*Mature relational database manager;
*ACID transactions;
*SQL as native language;
*Dynamic bitmap indexing;
*High scalability in a Symmetric Multi-Processing system;
*Can be tuned for both OLTP and data warehousing;
*High availability: data automatically replicated for intra- and inter-cluster;
*Easy administrative tools.

**Weakness**
*High cost;
*Proprietary;
*Primitive data models.

**Reference**
*White paper,  < IBM DB2 Universal Database on Windows NT Clusters>
*Comparison_and_Compatibility

*IBM Informix

**Strength**
*An embeddable database that integrates SQL, NoSQL/JSON, timeseries and spatial data;
*ACID transactions;
*SQL as native language;
*Deep compression of data, indexes, and blobs reduces storage needs and increases performance;
*Accelerated queries with an in-memory, columnar approach;
*Suitable for both OLTP and data warehousing;
*Easy administrative tools;
*High Availability.

**Weakness**
*High cost;
*Proprietary;
*Limited scalability.

**Reference**
*IBM Knowledge Center, Informix Servers 11.7, Administrator's Guide


*PostgreSQL

**Strength**
*as JSON indexing;
*Good support for BLOBs as well;
*Cost-based query optimization methods geared for complex join;
*Flexibility offered by the advanced GiST (Generalized Search Tree) indexing;
*ACID transactions, Multiversion concurrency control;
*Near linear scalability and High availability;
*A shared buffer cache and the kernel cache offer fast reads;
*Suitable for both OLTP and data warehousing;
*High standard compliance.

**Weakness**
*Behind MySQL in terms of popularity;
*Replication is not yet as well implemented as in MySQL.

**Reference**
*http://www.postgresql.org/about/
*_2007
*http://www.quora.com/What-are-the-advantages-and-disadvantages-of-using-PostgreSQL-over-MySQL
*MySQL

**Strength**
*World's most widely used open-source relational database management system (RDBMS);
*ACID transactions;
*Built-in replication support;
*Full-text indexing and searching;
*Commonly used in small to medium scale single-server deployments;
*High availability can be provided by MySQL Fabric;
*Shared-nothing clustering through MySQL Cluster.

**Weakness**
*Strongly limited by hard disk performance;
*Not currently compliant with the full SQL standard.
***Reference**
*http://en.wikipedia.org/wiki/MySQL
*http://www.mysql.com/why-mysql/topreasons.html
*GenieDB
*datacenter or cloud outage and faster response times for users anywhere in the world.
*MariaDB

**Strength**
*with improvements in:
*Variety of storage engines;
*Disk access optimization;
*Join and query optimization;
*Truly open source.

**Reference**
*https://mariadb.com/kb/en/mariadb/mariadb-vs-mysql-features/
*https://mariadb.com/kb/en/mariadb/mariadb-vs-mysql-features/
*MariaDB Enterprise
**Strength**
*technical support, backup and recovery.
**Reference**
*https://mariadb.com/products/mariadb-enterprise
*Spider
**Strength**
*MariaDB.
**Weakness**
*Immature product, incomplete documentation.
**Reference**
*engines/spider/spider-storage-engine-overview/
*Percona

**Strength**
*with improvements in:
*Faster querying and strong consistency;
*Easier administration;
*High availability.

**Reference**
*.html
*databases-comparison/
*TokuDB
**Strength**
*An open source, high-performance storage engine for MySQL, MariaDB, and Percona Server;
*Improvement in scalability and operational efficiency;
*Improvement in insertions and indexing: replaces B-tree indexing with modern Fractal Tree indexing;
*Better compression that cuts disk and flash-drive storage requirements;
*Hot schema changes.
**Weakness**
*Schema.
**Reference**
*http://www.tokutek.com/tokudb-for-mysql/
*differences/
*RackSpace Cloud Databases
*and operation.
*ScaleDB
**Strength**
*A data platform that transforms MySQL/MariaDB into scalable database cluster;
*High scalability: no sharding, shared-data approach;
*High availability with master-only architecture;
*Compatibility: works with existing MySQL applications without the need to change code.
**Weakness**
*Schema.
**Reference**
*White Paper, <ScaleDB for MySQL/MariaDB>
*White Paper, <ScaleDB Technical Overview>
*Drizzle
**Strength**
*with support for IPv6.
**Weakness**
*Incomplete documentation and limited support.
**Reference**
*http://www.drizzle.org/content/drizzle-and-ipv6

*Infobright
**Strength**
*Column-oriented relational database software with a focus in machine-generated data;
*Integration with MySQL with querying optimization;
*Increased scalability;
*Faster load from disk, better compression.
**Weakness**
*Write latency;
*Schema.
**Reference**
*http://en.wikipedia.org/wiki/Infobright
*Google Cloud SQL
**Strength**
*applications running on Google App Engine or Google Compute Engine;
*Security: Cloud SQL data is automatically encrypted;
*High availability and reliability;
*Standard MySQL, supporting complex queries, ACID transaction. 
**Weakness**
*Limited choice in database;
*Less scalable performance.
**Reference**
*com/article/2610430/cloud-computing/google-cloud-sql-debuts--following-amazon-s-rds-lead.html
*Google Cloud SQL, Features, https://cloud.google.com/sql/#features
*managment-systems

*HP Cloud RDB for MySQL  
**Strength**
*A fully managed MySQL service hosted on HP Cloud;
*High availability and reliability;
*Flexible database resize;
*Standard MySQL on OpenStack.
**Weakness**
*Limited choice in database;
*Limited scalability.
**Reference**
*database?t=features

*FathomDB
*development after being acquired by Meteor.
*com/2014/10/07/meteor-acquires-yc-alum-fathomdb-for-its-web-development-platform/
*AWQ RDS
**Strength**
*A fully managed relational database service hosted in the cloud;
*Security: encryption supported for MySQL or PostgreSQL databases;
*High availability and reliability with Multi-AZ;
*Wide range of database options.
**Weakness**
*High cost relative to limited functionality and performance.
**Reference**
*rds-vs-ec2-with-mysql
*<Amazon RDS Product Details>, http://aws.amazon.com/rds/details/
*ClearDB
**Strength**
*A geo-distributed MySQL database geared towards high availability, survivability, and reliability;
*Offers true multi-regional read/write mirroring with 100% uptime;
*Compatibility: native MySQL, works with existing MySQL applications without the need to change code;
*Security.
**Weakness**
*Schema;
*Write performance.
**Reference**
*How ClearDB Works, https://www.cleardb.com/better.view
*WebScaleSQL
**Strength**
*A MySQL data platform that is scale-oriented;
*Optimizations to certain types of queries;
*Compatibility: works with existing MySQL applications without the need to change code.
**Weakness**
*Schema;
*Weak consistency.
**Reference**
*http://webscalesql.org/faq.html
*DeepDB
**Strength**
*workloads;
*Accommodate both structured and unstructured data in the same database;
*Maximize performance by providing a high level of CPU concurrency and efficient memory management;
*Support all common storage types;
*High availability.
**Weakness**
*Distributed consistency.
**Reference**
*DeepDB White Paper, http://deep.is/resources/deepdb-white-paper/
*Galera
**Strength**
*A true MySQL multimaster cluster based on synchronous replication;
*High availability with a highly transparent and scalable synchronous replication solution.
**Weakness**
*Schema.
**Reference**
*White paper, <Minimizing downtime and maximizing elasticity with Galera Cluster for MySQL>
*Zimory
**Strength**
*coordinating communication between several varied product modules;
*Simplicity and excellent usability.

**Reference**
*eco/architecture.html#c403
*Continuent
**Strength**
*A scalable MySQL database cluster;
*High availability with asynchronous, transactional replication;
*Globally reduntant disaster recover (DR) capabilities;
*High performance with real-time data loading;
*Replication in real-time from RDBMS to MongoDB, Hadoop, and Vertica;
*Server (5.5 and 5.6) without changes. 
**Weakness**
*Schema.
**Reference**
*Cotinuent, Solutions, http://www.continuent.com/solutions
*CodeFutures AgilData
**Strength**
*A Real-time high-performance stream processing big data platform;
*SQL abstraction layer for the creation and querying of streams;
*An agile architecture that creates dynamic views of data specific to applications’ needs.
**Weakness**
*Less efficient use of storage.
**Reference**
*White paper, <Real Time Big Data: An Agile Approach>
*Tesora
**Strength**
*Database as a Service platform built upon OpenStack Trove project;
*Easy implementation;
*Multi-database support;
*Automatic backup and recovery.

**Reference**
*The Tesora Trove Difference, http://www.tesora.com/solutions/tesora-trove-difference
*ScaleArc
**Strength**
*An abstraction layer between applications and databases, supporting MySQL, SQL server, and Oracle;
*High scalability through load-balancing and replication;
*High availability and automatic failover;
*Optimized for real-time analytics.
**Weakness**
*Schema;
*Weak consistency;
*Write latency.
**Reference**
*ScaleArc, How It Works, http://scalearc.com/how-it-works
*ScaleBase
**Strength**
*A distributed MySQL database architecture designed for web-scale applications;
*High scalability through auto-sharding and replication;
*High availability and geo-distributed data.
**Weakness**
*Schema;
*Weak consistency (Two-Phase commit);
*Write latency.
**Reference**
*ScaleBase Technical Whitepaper
*HBase

**Strength**
*Google's Bigtable on top of Hadoop and HDFS;
*Map/reduce with Hadoop;
*Optimizations for real time queries;
*Random access performance is like MySQL;
*Strongly consistent reads/writes;
*High scalability of HDFS;
***Weakness**
*Not an ACID compliant database;
*Single point of failure as a master-slave architecture; 
*No JOIN;
*JVM may cause performance issues;
*Weak security.

**Reference**
*http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis
*Riak Compared to HBase, http://docs.basho.com/riak/latest/theory/comparisons/hbase/
*-analysis-part-3-pros-cons/


*HyperTable

**Strength**
*Google's Bigtable on top of Hadoop and HDFS;
*Map/reduce with Hadoop;
*Strongly consistent reads/writes;
*Geared towards fast access to ranges of data by keeping data physically sorted by a primary key;
*Written in C++ other than Java, faster in tests of random write and scan than HBase.
***Weakness**
*Not an ACID compliant database;
*Single point of failure as a master-slave architecture; 
*No JOIN.

**Reference**
*_2/
*Hypertable documentation architecture,
*http://hypertable.com/documentation/architecture/
*Accumulo

**Strength**
*Google's Bigtable on top of Hadoop and HDFS;
*Map/reduce with Hadoop;
*Optimizations for real time queries;
*Random access performance is like MySQL;
*Strongly consistent reads/writes;
*High scalability of HDFS;
*Cell-level security functionality.
***Weakness**
*Not an ACID compliant database;
*Single point of failure as a master-slave architecture; 
*No JOIN;
*No replication across datacenter.

**Reference**
*Distributed NoSQL: HBase and Accumulo, https://haifengl.wordpress.com/2014/05/14/hbase-and-accumulo/
*Accumulo: Why The World Needs Another NoSQL Database,
*http://wikibon.org/blog/breaking-analysis-accumulo-why-the-world-needs-another-nosql-database/

*Google App Engine Datastore

**Strength** 
*An database modeled after Google's Bigtable;
*Highly reliable and covered by the App Engine SLA;
*ACID transactions;
*Advanced querying features;
*High availability of reads and writes;
*Strong consistency for reads and ancestor queries;
*High scalability.
***Weakness**
*Strongly consistent except when performing global queries;
*No support for complex queries.

**Reference**
*Mastering the datastore, https://cloud.google.com/appengine/articles/datastore/overview
*Storing data in Java,
*https://cloud.google.com/appengine/docs/java/storage#app_engine_datastore
*Google Cloud Datastore

**Strength**
*A schemaless datastore modeled after Google's Bigtable;
*No planned downtime;
*Atomic transactions;
*High availability of reads and writes;
*Strong consistency for reads and ancestor queries;
*Eventual consistency for all other queries;
*High availability: replication across multiple datacenters based on the Paxos algorithm. 

**Weakness**
*No Join operations;
*No inequality filtering on multiple properties;
*No filtering of data based on results of a subquery.

**Reference**
*Comparison_with_traditional_databases

*FairCom
**Strength**
*A relational NewSQL database system geared towards insert and retrieval operations;
*SQL access to NoSQL type data;
*ACID transactions;
*High concurrency: sophisticated record locking;
*Robust multithreading for highly scalable SMP support;
*High availability: data automatically replicated for intra- and inter-cluster.

**Weakness**
*Limitation on complex query;
*Proprietary.

**Reference**
*com/articles/sql-access-to-nosql-type-data
*Features & Benefits, http://www.faircom.com/ace/ace_features_t.php
*Trafodion
**Strength**
*An enterprise-class SQL-on-HBase solution targeting big data transactional or operational workloads;
*ACID transactions;
*Geared towards OLTP workloads with compile-time and run-time optimizations;
*Parallel performance using a parallel-aware query optimizer;
*High scalability, high concurrency;
*High availability: data automatically replicated for intra- and inter-cluster.

**Weakness**
*No database security management except for HBase capabilities.

**Reference**
*Technical white paper Trafodion
*releases_of_Trafodion.3F
*InfiniSQL
**Strength**
*real time;
*SQL access to NoSQL type data;
*High scalability with optimized concurrency control.

**Weakness**
*No durability;
*Store only in memory: limitation on database size;
*No synchronous replication: limited fault tolerance.

**Reference**
*Benchmarking InfiniSQL, http://www.infinisql.org/blog/2013/1112/benchmarking-infinisql
*InfiniSQL™ Overview, http://www.infinisql.org/docs/overview/#idp37045792

*Datomic
**Strength**
*capabilities and scaling them independently;
*ACID Transactions and consistency;
*Support for JOIN;
*A logical query language – Datalog.

**Weakness**
*Limited using case: immutable data, and all data is retained by default.

**Reference**
*The Datomic Information Model, http://www.infoq.com/articles/Datomic-Information-Model
*Datomic's Benefits, http://www.datomic.com/benefits.html

*CockroachDB
**Strength**
*A distributed, key/value based, transactional datastore;
*ACID transaction and high consistency;
*Support for JOIN;
*High scalability.

**Weakness**
*No query language;
*Weak availability;
*High write latency.

**Reference**
*Cockroach documentation, Design, https://github.com/cockroachdb/cockroach?hn=true#design
*JustOneDB

**Strength**
*A NewSQL database built upon PostgreSQL with innovation in physical store on disk:  ‘tunnel store’;
*Fast in loading data from disk;
*Excels at highly selective queries and broad aggregate queries;
*ACID transactions, high concurrency;
*Near linear scalability and high availability.

**Weakness**
*High write latency.

**Reference**
*JustOneDB, core innovation, http://www.justonedb.com/products/justonedb/core-innovation/
*relational-database/d/d-id/1105768?

*TransLattice Elastic Database (TED)

**Strength**
*High availability focus: first geographically distributed relational SQL database server;
*Fast performance from all-active commodity servers, built for online transaction processing (OLTP);
*ACID transaction;
*Elastic scalability.

**Weakness**
*Tradeoff in consistency;
*Schema.

**Reference**
*TED Product Brief
*White Paper, TED

*ALTIBASE HDB (Hybrid Database)
**Strength**
*A RDBMS that specializes in in-memory computing;
*abstraction;
*High availability: built-in replication and share-nothing structure;
*ACID transaction and out-place MVCC;
*SQL standard compliance;
*Horizontal and vertical scalability.

**Weakness**
*Schema;
*Weak consistency with datacenter failure.

**Reference**
*Altibase HDB features,
*http://altibase.com/in-memory-database-hybrid-products/hdb/
*ALTIBASE XDB (Extreme In-memory Database)
*The in-memory version of HDB that comes with limitation in database size.
*http://altibase.com/in-memory-database-hybrid-products/xdb/


*NuoDB
**Strength**
*A relational NewSQL database system for high-throughput, operational applications;
*ACID transactions;
*SQL as native language;
*Near linear scalability provided with an new design approach called Durable Distributed Cache (DDC);
*High availability: data automatically replicated for intra- and inter-cluster.

**Weakness**
*Schema;
*Limits on database size.

**Reference**
*NuoDB How It Works, http://www.nuodb.com/explore/newsql-cloud-database-how-it-works
*architecture


*Clustrix
**Strength**
*A relational NewSQL database system for high-throughput, operational applications;
*processing;
*ACID transactions;
*SQL as native language;
*Scalable join and aggregates;
*High availability: data automatically replicated for intra- and inter-cluster;

**Weakness**
*Relational schema;
*Write latency.

**Reference**
*part-2.html
*NewSQL Vs. SQL on Hadoop,
*http://blog.clustrix.com/2014/02/03/newsql-vs-sql-hadoop/


