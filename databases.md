# History of databases

Timeline of technologies:
* 1964 IDS (navigational, network model)
* 1966 IBM IMS (navigational, hyerarchical model)
* 1970 IBM IS1 (relational)
* 1973 IDMS (navigational, network model)
* 1973 IBM Peterlee Relational Test Vehicle (relational)
* 1974 INGRES (relational)
* 1974 IBM System R (relational)
* 1975 Mimer SQL (relational)
* 1979 Oracle Database (relational)
* 1983 IBM DB2 (relational)
* 1989 POSTGRES (relational, object-oriented)
* 1989 Microsoft SQL Server (relational)
* 1992 Microsoft Access (relational)
* 1995 MySQL (relational)
* 1996 PostgreSQL (relational)
* 1999 Apache Lucene (search)
* 2000 SQLite (embedded, relational)
* 2003 Memcached (NoSQL, key-value)
* 2004 Apache Solr (search)
* 2005 Apache CouchDB (NoSQL)
* 2005 Google Bigtable (column)
* 2007 Neo4j (graph)
* 2008 Apache HBase (column)
* 2008 Apache Cassandra (column)
* 2009 MongoDB (NoSQL, document)
* 2009 Redis (NoSQL, key-value)
* 2009 Riak (NoSQL, key-value)
* 2009 MariaDB (relational)
* 2010 ElasticSearch (search)
* 2012 Amazon DynamoDB (NoSQL)
* 2012 Amazon Redshift (cloud)
* 2012 Google Spanner (NewSQL)
* 2012 Prometheus (time series)
* 2013 InfluxDB (time series)
* 2014 Amazon Aurora (cloud)
* 2015 Snowflake (cloud)
* 2016 Clickhouse (time series)
* 2017 Firestore (document, cloud)
* 2017 CockroachDB (NewSQL)
* 2017 Microsoft Cosmos DB (cloud)
* 2019 DuckDB (embedded, column)


## Navigational database

A navigational database is a type of database in which records or objects are
found primarily by following references from other objects.

Problems that is solves:
* magnetic disks enable arbitrary navigation of data storage media, as opposed
  to earlier magnetic-tape and punched card systems where data access was
  strictly sequential

Open problems:
* this family of databases is procedural (and proud to be so, because it was
  cool at those times), but databases are usually best queried in a
  declarative way
* users of the database have to know the storage implementation quite a lot


## Relational database

...

Problems that it solves:
* no more procedural databases: relational DBs are declarative
* users of the database don't have to know the implementation, they just have
  to know a high-level language

Open problems:
* ...


## Object-oriented database

...


## NoSQL database

...

Problems that is solves:
* huge companies care more about availability and scalability than consistency
* ...


## NewSQL database

...


## Data warehouse

Analytics [...]
Column store? [...]


## Cloud database

...


## Shared-disk system / Data lake

...


## Time series database

Optimization that relies on the assumption that thigs
are more or less ordered [...]
