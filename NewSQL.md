# NewSQL

## MemSQL

**Strength**
* A relational in-memory NewSQL database system for high-throughput, operational applications;
* Efficient columnar compression;
* Multiversion concurrency control: querying even as real-time data streams into the system;
* ACID transactions;
* SQL as native language;
* Near linear scalability;
* High availability: data automatically replicated for intra- and inter-cluster.

**Weakness**
* Isolation level is read committed;
* Limits on database size.

**Reference**
* http://www.memsql.com/features/




## FairCom

**Strength**
* A relational NewSQL database system geared towards insert and retrieval operations;
* SQL access to NoSQL type data;
* ACID transactions;
* High concurrency: sophisticated record locking;
* Robust multithreading for highly scalable SMP support;
* High availability: data automatically replicated for intra- and inter-cluster.

**Weakness**
* Limitation on complex query;
* Proprietary.

**Reference**
* How to Provide SQL Access to NoSQL Type Data using Multi-Record Type, http://www.infoq.com/articles/sql-access-to-nosql-type-data
* Features & Benefits, http://www.faircom.com/ace/ace_features_t.php




## Trafodion

**Strength**
* An enterprise-class SQL-on-HBase solution targeting big data transactional or operational workloads;
* ACID transactions;
* Geared towards OLTP workloads with compile-time and run-time optimizations;
* Parallel performance using a parallel-aware query optimizer;
* High scalability, high concurrency;
* High availability: data automatically replicated for intra- and inter-cluster.

**Weakness**
* No database security management except for HBase capabilities.

**Reference**
* Technical white paper Trafodion
* Trafodion wiki FAQ, https://wiki.trafodion.org/wiki/index.php/FAQ#What_is_the_Roadmap_for_future_releases_of_Trafodion.3F



## InfiniSQL

**Strength**
* A massively scalable RDBMS geared towards 'always on' applications and for complex transactions in real time;
* SQL access to NoSQL type data;
* High scalability with optimized concurrency control.

**Weakness**
* No durability;
* Store only in memory: limitation on database size;
* No synchronous replication: limited fault tolerance.

**Reference**
* Benchmarking InfiniSQL, http://www.infinisql.org/blog/2013/1112/benchmarking-infinisql
* InfiniSQL™ Overview, http://www.infinisql.org/docs/overview/#idp37045792

## Datomic

**Strength**
* A new database that deconstructs the traditional database, separating storage, query and transaction capabilities and scaling them independently;
* ACID Transactions and consistency;
* Support for JOIN;
* A logical query language – Datalog.

**Weakness**
* Limited using case: immutable data, and all data is retained by default.

**Reference**
* The Datomic Information Model, http://www.infoq.com/articles/Datomic-Information-Model
* Datomic's Benefits, http://www.datomic.com/benefits.html

## CockroachDB

**Strength**
* A distributed, key/value based, transactional datastore;
* ACID transaction and high consistency;
* Support for JOIN;
* High scalability.

**Weakness**
* No query language;
* Weak availability;
* High write latency.

**Reference**
* Cockroach documentation, Design, https://github.com/cockroachdb/cockroach?hn=true#design




## JustOneDB

**Strength**
* A NewSQL database built upon PostgreSQL with innovation in physical store on disk: ‘tunnel store’;
* Fast in loading data from disk;
* Excels at highly selective queries and broad aggregate queries;
* ACID transactions, high concurrency;
* Near linear scalability and high availability.

**Weakness**
* High write latency.

**Reference**
* JustOneDB, core innovation, http://www.justonedb.com/products/justonedb/core-innovation/
* JustOneDB Reinvents Relational Database, http://www.informationweek.com/software/justonedb-reinvents-relational-database/d/d-id/1105768?

## TransLattice Elastic Database (TED)

**Strength**
* High availability focus: first geographically distributed relational SQL database server;
* Fast performance from all-active commodity servers, built for online transaction processing (OLTP);
* ACID transaction;
* Elastic scalability.

**Weakness**
* Tradeoff in consistency;
* Schema.

**Reference**
* TED Product Brief
* White Paper, TED

## ALTIBASE HDB (Hybrid Database)

**Strength**
* A RDBMS that specializes in in-memory computing;
* Unified engine allows for the use of an in-memory and on-disk database solution with layer of abstraction;
* High availability: built-in replication and share-nothing structure;
* ACID transaction and out-place MVCC;
* SQL standard compliance;
* Horizontal and vertical scalability.

**Weakness**
* Schema;
* Weak consistency with datacenter failure.

**Reference**
* Altibase HDB features, http://altibase.com/in-memory-database-hybrid-products/hdb/




## ALTIBASE XDB (Extreme In-memory Database)
The in-memory version of HDB that comes with limitation in database size.
**Reference**
* http://altibase.com/in-memory-database-hybrid-products/xdb/


## NuoDB

**Strength**
* A relational NewSQL database system for high-throughput, operational applications;
* ACID transactions;
* SQL as native language;
* Near linear scalability provided with an new design approach called Durable Distributed Cache (DDC);
* High availability: data automatically replicated for intra- and inter-cluster.

**Weakness**
* Schema;
* Limits on database size.

**Reference**
* NuoDB How It Works, http://www.nuodb.com/explore/newsql-cloud-database-how-it-works
* NuoDB Durable Distributed Cache Architecture, http://www.nuodb.com/explore/newsql-cloud-database-ddc-architecture


## Clustrix

**Strength**
* A relational NewSQL database system for high-throughput, operational applications;
* Geared towards real-time analytics with multi-version concurrency control and massively parallel processing;
* ACID transactions;
* SQL as native language;
* Scalable join and aggregates;
* High availability: data automatically replicated for intra- and inter-cluster;

**Weakness**
* Relational schema;
* Write latency.

**Reference**
* MongoDB vs. Clustrix Comparison, http://sergei.clustrix.com/2011/02/mongodb-vs-clustrix-comparison-part-2.html
* NewSQL Vs. SQL on Hadoop, http://blog.clustrix.com/2014/02/03/newsql-vs-sql-hadoop/
