# Graph Databases: The Storage Layer, Execution Engine Layer, and Frontend Layer 
## Surveys, Summary and Tutorials
1. Demystifying Graph Databases: Analysis and Taxonomy of Data Organization, System Designs, and Graph Queries (ACM Computing Surveys 2019) [[Paper](https://arxiv.org/pdf/1910.09017)]
> * A very good overview of graph databases with clear illustrations! Strongly recommended for beginners.
2. The journey of GraphScope [[Link](https://graphscope.io/journey/)]

## Overall System Archtecture
1. GraphScope Flex: LEGO-like Graph Computing Stack (SIGMOD 2024) 

## The Storage Layer
1. GraphAr: An Efficient Storage Scheme for Graph Data in Data Lakes (VLDB 2025) [[Paper](https://vldb.org/pvldb/volumes/18/paper/GraphAr%3A%20An%20Efficient%20Storage%20Scheme%20for%20Graph%20Data%20in%20Data%20Lakes)] 
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
6. Columnar Storage and List-based Processing for Graph Database Management Systems (VLDB 2020) [[Github (you can refer to the presentation video)](https://github.com/graphflow/graphflow-columnar-techniques?tab=readme-ov-file)]
> * `in-memory`, `immutable graph`, `adjancency list and CSR?`
7. GraphOne: A Data Store for Real-time Analytics on Evolving Graphs (FAST 2019) [[Paper](https://www.usenix.org/conference/fast19/presentation/kumar)]
> * `in-memory`, `mutable graph`
8. GraphChi: Large-Scale Graph Computation on Just a PC (OSDI 2012) [[Paper](https://www.usenix.org/system/files/conference/osdi12/osdi12-final-126.pdf)] hot!
> * `on-disk`, `mutable graph`
9. GraphCSR: A Degree-Equalized CSR Format for Large-scale Graph Processing (VLDB 2025) [[Paper](https://vldb.org/pvldb/volumes/18/paper/GraphCSR%3A%20A%20Degree-Equalized%20CSR%20Format%20for%20Large-scale%20Graph%20Processing)]
> * `in-memory`, `immutable graph`, `CSR`
  
## Interface
1. GRIN

## The Computing Layer
1. A1: A Distributed In-Memory Graph Database (Micorsoft, SIGMOD 2020) [[Paper](https://arxiv.org/pdf/2004.05712)]
