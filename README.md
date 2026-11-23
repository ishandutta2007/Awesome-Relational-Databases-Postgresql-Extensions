# Awesome-Relational-Databases-Postgresql-Extensions

## Top Relational Databases & PostgreSQL Extensions Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Managed Postgres, Self-Hosted PostgreSQL, Extensions (Vectors, Time-Series, Geo, HA) & Durable In-Database Workloads*  

**Last updated: November 2026**



This repository tracks notable **SaaS/hosted platforms** and **open-source projects** for **Relational Databases & PostgreSQL Extensions**. PostgreSQL is the center of gravity—hosted services, the core database, and the extension ecosystem that turns it into a vector store, time-series engine, GIS platform, and more.



**Examples** include Neon Serverless Postgres, Supabase, Timescale Cloud, Crunchy Bridge, Aiven for PostgreSQL, AWS RDS PostgreSQL, Google Cloud SQL, Azure Database for PostgreSQL, Tembo Cloud, ElephantSQL, and **pg_durable** (`microsoft/pg_durable`)—durable, fault-tolerant SQL function execution inside PostgreSQL.



**Open-source emphasis**: PostgreSQL and its extensions are fully open. **PostgreSQL**, **pgvector**, **PostGIS**, **Citus**, **TimescaleDB** (Apache components), **pg_cron**, **Patroni**, and **pg_durable** define modern Postgres stacks. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Neon, Supabase, Timescale Cloud, Tembo](https://neon.tech/)**  

  Developer-focused managed Postgres—serverless scale-to-zero, auth/storage bundles, time-series, and extension-rich plans.



- **[AWS RDS / Aurora PostgreSQL, Google Cloud SQL, Azure Database for PostgreSQL](https://aws.amazon.com/rds/postgresql/)**  

  Hyperscaler managed PostgreSQL—automated backups, replicas, and deep cloud integration.



- **[Crunchy Bridge, Aiven for PostgreSQL, ElephantSQL](https://www.crunchydata.com/products/crunchy-bridge)**  

  Independent managed Postgres providers—often strong on extensions, support, and multi-cloud choice.



- **[Other commercial Postgres platforms](https://supabase.com/)**  

  Additional hosted Postgres, BaaS, and specialty extension clouds.



## Open-Source GitHub Projects



### Core Database



- **[PostgreSQL](https://github.com/postgres/postgres)**  

  The open-source object-relational database—ACID, extensibility, SQL standards, and the foundation for almost every project below.



### Popular Extensions



- **[pgvector](https://github.com/pgvector/pgvector)**  

  Open vector similarity search for Postgres—`vector` type plus IVFFlat and HNSW indexes for embeddings and RAG.



- **[PostGIS](https://github.com/postgis/postgis)**  

  Open spatial database extender—geometry/geography types, spatial indexes, and GIS functions on top of PostgreSQL.



- **[Citus](https://github.com/citusdata/citus)**  

  Open distributed PostgreSQL extension—shard tables across nodes for multi-tenant and analytical scale-out (AGPL).



- **[TimescaleDB](https://github.com/timescale/timescaledb)**  

  Open time-series extension for PostgreSQL—hypertables, compression, and continuous aggregates (check Apache vs community license features).



- **[pg_cron](https://github.com/citusdata/pg_cron)**  

  Open job scheduler as a Postgres extension—run SQL on a cron schedule inside the database.



- **[pg_partman](https://github.com/pgpartman/pg_partman)**  

  Open partition management extension—automated time and serial partitioning.



- **[pg_durable](https://github.com/microsoft/pg_durable)**  

  Open PostgreSQL extension for durable, fault-tolerant SQL functions—checkpointed workflows, scheduling, and recovery without external workers.



- **[pg_stat_statements / contrib extensions](https://github.com/postgres/postgres)**  

  Built-in and contrib open extensions for query stats, fuzzy search (`pg_trgm`), crypto, and more.



- **[ParadeDB / pg_search](https://github.com/paradedb/paradedb)**  

  Open search-oriented Postgres extensions—BM25 and advanced full-text patterns inside PostgreSQL.



- **[PostgresML](https://github.com/postgresml/postgresml)**  

  Open extension to run ML workloads with a SQL interface inside Postgres.



### High Availability, Pooling & Ops



- **[Patroni](https://github.com/patroni/patroni)**  

  Open HA template for PostgreSQL—automated failover using etcd/Consul/ZooKeeper and streaming replication.



- **[pgBouncer](https://github.com/pgbouncer/pgbouncer)**  

  Lightweight open connection pooler for PostgreSQL—essential for high-churn app workloads.



- **[Pgpool-II](https://github.com/pgpool/pgpool2)**  

  Open connection pooling, load balancing, and replication helper for PostgreSQL.



- **[Barman / pgBackRest](https://github.com/pgbarman/barman)**  

  Open backup and recovery tools purpose-built for PostgreSQL.



- **[CloudNativePG](https://github.com/cloudnative-pg/cloudnative-pg)**  

  Open Kubernetes operator for PostgreSQL—declarative clusters on K8s.



### Additional Strong Open-Source Options



- **Default RDBMS**: PostgreSQL.

- **AI / embeddings**: pgvector (± pgvectorscale / related indexes).

- **Geo**: PostGIS.

- **Time-series**: TimescaleDB (open components) or pure Postgres partitioning + pg_partman.

- **Distributed SQL on Postgres**: Citus.

- **In-DB durable jobs**: pg_durable or pg_cron + application design.

- **Composable stacks**: PostgreSQL + pgvector + PostGIS + Patroni + pgBouncer + pgBackRest.

- Managed services still lead for serverless UX, automatic scaling, and hands-off operations.



**Frameworks for building custom systems**:  

**PostgreSQL** as the core; add **pgvector** for semantic search, **PostGIS** for maps, **Citus**/**TimescaleDB** for scale/time-series, **pg_durable** for in-database workflows, and **Patroni** + **pgBouncer** for production HA and pooling.  

Fully open relational stacks with rich extensions are the default for serious application data layers.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS/hosted or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Extensions run in the database process—install only trusted packages, match versions to your Postgres major, and test upgrades. Backups, access control, and migration discipline remain your responsibility.

- Open-source Postgres offers full control and portability. Managed services shift operations and often extension packaging to the vendor. Neither replaces schema design, indexing strategy, and monitoring.



---



**Made for application developers, DBAs, and platform teams standardizing on PostgreSQL.**  

Let's expand open relational databases and extensions while recognizing the operational convenience of leading managed Postgres platforms.
