# Graph Databases: The Storage Layer, Execution Engine Layer, and Frontend Layer

## Surveys, Summary and Tutorials
1. Demystifying Graph Databases: Analysis and Taxonomy of Data Organization, System Designs, and Graph Queries (ACM Computing Surveys 2019) [[Paper](https://arxiv.org/pdf/1910.09017)]
> * A very good overview of graph databases with clear illustrations! Strongly recommended for beginners.
2. The journey of GraphScope [[Link](https://graphscope.io/journey/)]

## Overall System Archtecture
1. GraphScope Flex: LEGO-like Graph Computing Stack (SIGMOD 2024)

## The Storage Layer
1. An Efficient Storage Scheme for Graph Data in Data Lakes (VLDB 2024)
> * `on-disk`, `immutable graph`
> * LPG in datalake, based on Parquet/ORC. 
2. LiveGraph: A Transactional Graph Storage System with Purely Sequential Adjacency List Scans (VLDB 2020)
3. Groot: Persistent Graph Store [[Link](https://graphscope.io/docs/latest/storage_engine/groot)]
> * `on-disk`, `mutable graph`
> * A distributed graph store built on top of the popular RocksDB key-value store. It adopts a row-oriented design to support frequent small updates to the graph. Each row is tagged with a snapshot ID as its version.
4. Vineyard
> * `in-memory` 
5. GART: Bridging the Gap between Relational OLTP and Graph-based OLAP (ATC 2024)
> * `in-memory`, `mutable graph`
> * An in-memory system that extends hybrid transactional/analytical processing (HTAP) systems to support graph analytical processing (GAP).

## Interface
1. GRIN
