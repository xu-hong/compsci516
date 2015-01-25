# Graph 

## YarcData

**Strength**
* Business-focused real-time graph analytics platform;
* Optimized for compute-heavy, memory-centric;

**Weakness**
* Very few documents.

**Reference**
* Whitepaper, CrayUrikaXA-Technical-Specs

## Neo4j

**Strength**
* Native graph storage with flexible schema;
* SQL queries supported with Cypher;
* ACID transactions supported;
* High availability via a master-slave HA protocol.

**Weakness**
* Optimized for reads, not write;
* Weak in global queries and number crunching;
* Weak for binary data store;
* Possible single point of failure.  

**Reference**
* http://neo4j.com/developer/graph-db-vs-nosql/
* http://kkovacs.eu/cassandra-vs-mongodb-vs-couchdb-vs-redis
* A Comparison of Current Graph Database Models, Renzo Angles, Universidad de Talca (Chile)


## GrapheneDB
A Neo4j database host platform with support, 24X7 monitoring, and backups provided.

**Reference**
* http://docs.graphenedb.com/getting-started.html

## Sparksee

**Strength**
* Compact representation of graph storage using bitmaps, high throughput and fast speed; 
* High availability via a master-slave HA protocol;
* First graph database on Android and iOS.

**Weakness**
* Partial transactional;
* No query language;
* Possible single point of failure.  

**Reference**
* Sparksee Technology Overview http://www.slideshare.net/SparsityTechnologies/sparksee-technology-overview
* Sparksee Archetecture, http://www.sparsity-technologies.com/HighAvailability/Architecture.html

## FlockDB

**Strength**
* Distributed graph database for storing adjacency lists;
* Optimized for a high rate of add/update/remove operations;
* Simple, small, lightweight solution tailored for Twitter.

**Weakness**
* Not built for multi-hop queries (or graph-walking queries) or automatic shard migrations
* No transaction;
* No query language (can add query using Gizzard);
* Availability and scalability come through Gizzard.

**Reference**
* https://blog.twitter.com/2010/introducing-flockdb
* https://github.com/twitter/flockdb

## Stardog

**Strength**
* Lightweight graph database on RDF data model;
* Query supported: SPARQL;
* ACID transactions supported;
* High availability via a master-slave HA protocol;
* OWL & Rule Reasoning: semantic search.

**Weakness**
* Weak in number crunching;
* Weak for binary data store;
* Possible single point of failure.  

**Reference**
* The Stardog Manual, http://docs.stardog.com



## Titan

**Strength**
* Linear, elastic scalable graph database, optimized for handling thousands of concurrent transactions;
* Data distribution and replication for performance and fault tolerance, no single point failure;
* Multicenter high availability;
* ACID transaction;
* Support for various storage backends;
* Support for graph query with Gremlin.

**Weakness**
* Niche in multiple short, local queries;
* No search capabilities built within (search capability comes with indexing service such as Lucene)

**Reference**
* Titan vs Neo4J, https://groups.google.com/forum/#!msg/aureliusgraphs/vkQkzjN8fo0/9YYgqI4TA0QJ
* Titan Documentation, http://thinkaurelius.github.io/titan/



## AffinityDB

**Strength**
* Graph database geared towards embedded information-processing, control and communication;
* SQL queries supported with pathSQL;
* ACID transactions supported.

**Weakness**
* Scalability and high availability.

**Reference**
* http://affinityng.cfapps.io/doc/**Strength**s.html
* http://affinityng.cfapps.io/doc/features.html


## Trinity

**Strength**
* Fast, distributed graph system over a memory cloud;
* Highly compact in-memory access geared for parallel computing;
* Rich system management and development tools.

**Weakness**
* No ACID transaction;
* No query language;
* Limited scalability and availability.

**Reference**
* Trinity: A Distributed Graph Engine on a Memory Cloud, Bin Shao et al, ACM SIGMOD



## SPARQL

**Strength**
* Graph database on RDF data model for high performance graph analysis;
* Standard based (Solely built around W3C standards, SPARQL, RDF);
* ACID transaction;
* High scalability;
* High availability provided by backed HDFS.

**Weakness**
* No flexible choice for native store;
* No fault tolerance beyond native storage level. 


**Reference**
* SPARQLverse Guide




## Apache Giraph

**Strength**
* Iterative graph processing system built for high scalability;
* Optimized for batch processing of massive graphs;
* Faster: it loads an entire graph into a cluster's memory.

**Weakness**
* Limited supported size of the graph;
* No fault tolerance beyond Hadoop. 


**Reference**
* Giraph User Guide
* Scalable Graph Processing: Comparing Giraph, Titan, Faunus, http://xinhstechblog.blogspot.com/2012/12/scalable-graph-processing-comparing.html
* Giraph for Large Multigraphs, http://xinhstechblog.blogspot.com/2012/10/giraph-for-large-multigraphs.html





##AllegroGraph

**Strength**
* Graph database that uses efficient memory utilization in combination with persistence to disk-based storage;
* Designed for maximum loading speed and query speed for large files;
* Full Read Concurrency, Near Full Write Concurrency;
* ACID transaction;
* LISP-based development tools.

**Weakness**
* Proprietary product;
* Availability.

**Reference**
* AllegroGraph Introduction, http://franz.com/agraph/support/documentation/current/warm-standby.html#header2-8
* http://franz.com/agraph/allegrograph/




## HyperGraphDB

**Strength**
* Object-oriented multi-relational labeled hypergraph;
* A persistent memory model designed mostly for knowledge management, AI and semantic web projects;
* Flexible: can be used as an embedded object-oriented database for Java projects, or a graph database, or a (non-SQL) relational database;
* Non-blocking concurrent writes and reads;
* Size limitations virtually non-existent;
* P2P framework: no single point of failure.

**Weakness**
* No ACID transaction;
* Scalability.

**Reference**
* Data Management for Complex Systems, http://www.hypergraphdb.org/docs/HyperGraphDB-Presentation.pdf



## InfiniteGraph

**Strength**
* Labeled and directed multi-property-graph optimized for data relationships;
* ACID transaction;
* Elastic scalability;
* High availability.

**Weakness**
* No query language, just API.

**Reference**
* InfiniteGraph Technical Specifications
