# In-memory / Data Grid 


## Infinispan

**Strength**
* In-memory access: fast;
* Schema-less key/value overcoming the constraints of traditional database;
* Can be used as local cache and as clustered caches as well, which can linearly scale out; 
* Scalable data partitioning across cluster, providing fault tolerance;
* Elastic with consistent hashing, availability during topology changes;
* Support for access to caches either transactionally or non-transactionally;
* Greater concurrency with multiversion concurrency control;
* Support for Write-Through And Write-Behind Caching to persistent storage.

**Weakness**
* Migrating from SQL to Map-like API is not easy;
* More apt to complement traditional database rather than to replace it;
* Network bandwidth may become the bottleneck;
* Less strict schema may require more validation on application data layer.

**Reference**
* Data Grids vs Databases,  http://www.slideshare.net/galderz/data-grids-vs-databases
* Data Grids and Data Caching, http://www.slideshare.net/galderz/data-grids-and-data-caching
* Wikipedia, MVCC, http://en.wikipedia.org/wiki/Multiversion_concurrency_control
* Jags Ramnarayan on In-Memory Data Grids, http://www.infoq.com/articles/in-memory-data-grids


## Red Hat JBoss Data Grid  

**Strength** and the **Weakness**: same as Infinispan (since it is an ecosystem which is built around Infinispan)

**Reference**
* White paper, Red Hat JBoss Data Grid 6.4 Beta Getting Started Guide
* White paper, Improving Application Scalability with In-Memory Data Grids




## GridGain  

**Strength**
* Integrate fast In-Memory MapReduce implementation;
* Geared towards in-memory near real time computations and low latencies, support affinity co-location;
* Scalable data partitioning across cluster, providing fault tolerance;
* Support for access to caches either transactionally or non-transactionally;
* Support for async repartitioning or delayed repartitioning;
* Greater concurrency with multiversion concurrency control;
* Support for off heap data overflow to better work with JVM Garbage Collection;
* Schema-less key/value to overcome the constraints of traditional database;
* Also allow standard SQL to query in-memory data as well as distributed join;
* Support for Write-Through And Write-Behind Caching to persistent storage.

**Weakness**
* More apt to complement traditional database rather than to replace it;
* Network bandwidth may become the bottleneck;
* Less strict schema may require more validation on application data layer.

**Reference**
* GridGain & Hadoop: Differences & Synergies, http://gridgain.com/gridgain-hadoop-differences-synergies/
* In-Memory Data Grid: Explained, http://gridgain.com/in-memory-data-grid-explained/
* In-Memory Data Fabric, http://gridgain.com/products/in-memory-data-fabric/


## Hazelcast

**Strength**
* Easy scale out by adding nodes, dynamically rebalance data across the new grid; 
* Elastic with consistent hashing: availability during topology changes;
* Support for access to caches either transactionally or non-transactionally;
* Greater concurrency with multiversion concurrency control;
* Schema-less key/value to overcome the constraints of traditional database.

**Weakness**
* No support for Fully Replicated architecture in peer-to-peer mode;
* No in memory streaming;
* No async repartitioning or delayed repartitioning;
* More apt to complement traditional database rather than to replace it;
* Network bandwidth may become the bottleneck;
* Less strict schema may require more validation on application data layer.

**Reference**
* Java Caches: Ehcache, Hazelcast, Infinispan, https://labs.consol.de/java-caches/
* White paper, GridGain vs. Hazelcast Feature Comparison



## Ehcache

**Strength**
* Fast, easy-to-set-up and light weight in-memory data grids (IMDG);
* Scalable data partitioning across cluster, providing fault tolerance;
* Seamless integration as a second-level cache for Hibernate.

**Weakness**
* No support for Fully Replicated architecture in peer-to-peer mode, in memory streaming, async repartitioning or delayed repartitioning or other advanced features;
* No support for other languages besides Java;
* More apt to complement traditional database rather than to replace it.

**Reference**
* http://ehcache.org/about/features
* http://ehcache.org/documentation/2.6/get-started/about-distributed-cache


## BigMemory
An upgrade of Ehcache with support for off heap data overflow to better work with JVM Garbage Collection.



## CloudTran

**Strength**
* Extends in-memory data grids (IMDG) by adding scalable transactions across the grid and implementing guaranteed persistence to databases; 
* Integrate Oracle Coherence with back-end data stores asynchronously and provide ACID transactionality with optimized 2-Phase Commit (2PC).

**Weakness**
* Mainly invented for the purpose of improving Coherence;
* The emphasis on transaction might impede its performance.

**Reference**
* White paper,  CloudTran Technology Genesis


## Oracle Coherence

**Strength**
* The commercial counterpart of Hazelcast. IMDG that provides availability, scalability, parallel query and parallel transaction processing, etc.

**Weakness**
* Licensing model.

**Reference**
* White paper, ORACLE COHERENCE 12C


## IBM eXtreme Scale  
IBM’s counterpart of Oracle Coherence: 
* Better integration with WAS; 
* Features like Disk Off-load or Disk Snapshot support enables faster restoration of the grid post failure or maintenance;  
* Less expensive price.

**Reference**
* http://whywebsphere.com/2012/07/03/data-grids-and-caching-ibm-or-oracle/
* Redbook,  WebSphere eXtreme Scale V8.6 Key Concepts and Usage Scenarios

## Memcached

**Strength**
* Simple yet fast;
* Better use of memory with distributed memory object caching;
* In-memory key-value store for database calls, speeding up dynamic web applications by alleviating database load;
* Near O(1) for every memcached operation.

**Weakness**
* Not a good fit for persistent storage;
* No clustering thus no consistency provided;
* Unreliable;
* Scaling requires code update on client applications.

**Reference**
* http://parsa.epfl.ch/cloudsuite/memcached.html
* https://code.google.com/p/memcached/wiki/NewStart


## AWS ElastiCache, AWS ElastiCache with Redis
ElastiCache is a web service that supports Memcached (or Redis) as in-memory cache engine. It possesses the strength of that of Memcached and also adds:

**Strength**
* Simple to deploy and manage with management console or simple APIs;
* Enhancement in elasticity and scalability, auto discover of new nodes;
* Enhancement in reliability through auto failure detection and recovery.

**Weakness**
* No clustering thus no consistency provided.

**Reference**
* Caching architectures using Memcached & Amazon ElastiCache, http://harish11g.blogspot.in/2012/11/amazon-elasticache-memcached-ec2.html
* Amazon ElastiCache User Guide


## RedisLabs Memcached Cloud
Memcached Cloud is a fully-managed service for hosting and running Memcached in a reliable and fail-safe manner.
**Strength**
* Enhancement in reliability through auto failure detection and recovery;
* Backup to and imports from FTP server and other cloud storages;
* Enhancement in elasticity and scalability.
**Reference**
* https://redislabs.com/memcached-cloud


## RedisLabs Redis Cloud

**Strength**
* Enhancement in availability;
* Backup to and imports from FTP server and other cloud storages;
* Enhancement in elasticity and scalability.
***Reference**
* https://redislabs.com/redis-cloud

## Memcachier
MemCachier manages and scales clusters of memcache servers. 

**Strength**
* Enhancement in reliability through auto failure detection and recovery;
* Enhancement in elasticity and scalability;
* Analytics dashboard provided to monitor cache usage.

**Reference**
* https://www.memcachier.com/how-it-works



## GigaSpaces XAP

**Strength**
* Veteran product in IMDG market; 
* In-memory access: fast;
* Scalable data partitioning across cluster, providing fault tolerance;
* Elastic with consistent hashing: availability during topology changes;
* Support for access to caches either transactionally or non-transactionally;
* Schema-less key/value to overcome the constraints of traditional database;
* Support for replication across data centers.

**Weakness**
* More apt to complement traditional database rather than to replace it;
* Network bandwidth may become the bottleneck;
* Less strict schema may require more validation on application data layer.

**Reference**
* http://www.gigaspaces.com/xap-high-availability-load-balancing/how-it-works
* White Paper,  Elastic Caching Platforms, Q2 2010


## TIBCO  ActiveSpaces

**Strength**
* Support SQL-like query to in-memory data;
* Configurable data purging: allows Time-to-live (TTL) to be set for in-memory caches;
* Scalable data partitioning across cluster, providing fault tolerance;
* Elastic with consistent hashing: availability during topology changes;
* Support for access to caches either transactionally or non-transactionally;
* Schema-less key/value to overcome the constraints of traditional database;

**Weakness**
* More apt to complement traditional database rather than to replace it;
* Network bandwidth may become the bottleneck;
* Less strict schema may require more validation on application data layer.

**Reference**
* White Paper,  TIBCO ActiveSpaces Use Cases



## Pivotal  GemFire  

**Strength**
* Schema-less key/value to overcome the constraints of traditional database;
* Focused almost exclusively on large enterprise projects in financial services, defense, and intelligence;
* Consistency across geo-distributed applications;
* Highly scalable data partitioning across cluster, providing fault tolerance;
* Support for access to caches either transactionally or non-transactionally;
* Easy monitoring and management.

**Weakness**
* Licensing model, very costly;
* Complex configuration;
* More apt to complement traditional database rather than to replace it;
* Network bandwidth may become the bottleneck.

**Reference**
* White Paper,  Elastic Caching Platforms, Q2 2010
* http://www.vmware.com/products/vfabric-gemfire/features.html

## Pivotal  GemFire  XD 
Pivotal GemFire with SQL query support: Supports SQL queries of data over distributed nodes that can be optimized with indexes on key values.

**Reference**
* http://www.pivotal.io/big-data/pivotal-gemfire-xd

## Scaleout Software

**Strength**
* A suite of IMDG products that provides in-memory map/reduce implementation, faster Hadoop MapReduce execution time;
* Support for replication between data centers for disaster recovery;
* Scalable data partitioning across cluster, fault tolerance and distributed applications/computations;
* Support for access to caches either transactionally or non-transactionally;
* Schema-less key/value to overcome the constraints of traditional database.

**Weakness**
* Licensing model;
* Complex configuration;
* More apt to complement traditional database rather than to replace it;
* Network bandwidth may become the bottleneck.

**Reference**
* ScaleOut hServer V2 Java Programmer's Guide

## IronCache

**Strength**
* Configurable data purging: allows Time-to-live (TTL) to be set for in-memory caches;
* Developer friendly interface with IronMQ; 
* Full visibility into caches and usage with the Iron.io user interface;
* Scalable data partitioning across cluster, fault tolerance and distributed applications/computations;
* Elastic with consistent hashing: availability during topology changes;
* Support for access to caches either transactionally or non-transactionally;
* Schema-less key/value to overcome the constraints of traditional database.

**Weakness**
* More apt to complement traditional database rather than to replace it;
* Network bandwidth may become the bottleneck;
* Less strict schema may require more validation on application data layer.

**Reference**
* https://devcenter.heroku.com/articles/iron_cache
* http://www.iron.io/worker


## Redis

**Strength**
* Very fast, good concurrency support;
* In-memory key-value store for database calls, with flexibility of the objects it can cache;
* Fine-grained control over eviction;
* Master-slave replication supported to ensure highly availability;
* Transaction supported with optimistic locking;
* Persistence to disk;
* Scalability when used as cache.

**Weakness**
* Immature clustering thus no consistency provided;
* Dataset size limited to computer RAM;
* No scalability when used as data store (Redis Cluster is currently in beta).

**Reference**
* http://redis.io/topics/transactions
* http://stackoverflow.com/questions/10906246/what-is-the-disadvantage-of-just-using-redis-instead-of-an-rdbms
* http://www.infoworld.com/article/2825890/application-development/why-redis-beats-memcached-for-caching.html



## ObjectRocket Redis, RedisGreen, Redis-to-go
Commercial product build around Redis with 24x7x365 support and easy interface.

**Reference**
* https://objectrocket.com/redis/
* http://www.redisgreen.net/
* http://redistogo.com/