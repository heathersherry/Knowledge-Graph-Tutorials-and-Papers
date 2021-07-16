## Knowledg Graph Representation (RDF and Property Graph) and Schema
There are two major approaches to store and query knowledge graphs: (1) RDF (Resource Description Framework) data model with SPARQL query language, (2) property graph model with graph query languages such as Cypher. 

## RDF Graphs
__Surveys__
1. RDF Data Storage and Query Processing Schemes: A Survey [[Paper](https://dl.acm.org/doi/pdf/10.1145/3177850)]

__General Papers__
1. Relational schema optimization for RDF-based knowledge graphs (Information Systems 2021) [[Paper](https://www.sciencedirect.com/science/article/pii/S0306437921000223)] 

__Queries and Search over RDF based KG__

__1. Keyword search__

__1.1 Summary Graph Based Keyword Query__
1. Top-k exploration of query candidates for efficient keyword search on graph-shaped (rdf) data (ICDE 2009) 🌟
2. Finding top-k min-cost connected trees in databases (ICDE 2007) 🌟
3. Keyword search over RDF graphs (CIKM 2011) 🌟
> * [2] and [3] define the keyword search problem as a minimum connected tree [2] or a subgraph [3] over the data graph, while the target is to cover all the keyword by the nodes and edges of the derived tree or subgraph.
> * This problem definition is very close to the group Steiner tree problem (GST), which is proven to be NP-complete.
> * DPBF [2] guarantees to derive the exact optimal result of a minimum-weight GST with parameterized time complexity. However, DPBF still suffers from the exponential time and space complexity, especially on large graphs. Moreover, DPBF cannot generate a solution until the entire algorithm is completed.
4. Keyword searching and browsing in databases using BANKS (ICDE 2002) 🌟
5. Bidirectional expansion for keyword search on graph databases (VLDB 2005)
6. BLINKS:rankedkeyword searches on graphs (SIGMOD 2007)
> * BANKS [4], BANKS-II [5], and BLINKS [6], which propose approximate algorithms. BANKS merges paths from keyword vertices to approximate a minimum-weight GST, while BANKS-II further improves the performance of BANKS by conducting bidirectional search. In addition, BLINKS exploits the precomputed distances and graph partitioning to further improve the efficiency of the bidirectional search.
7. Scalable keyword search on large rdf data (TKDE 2014) 🌟
> * The search can also be pruned based on the graph summaries. The RDF data is first condensed into a generic graph, while the entity vertex with the corresponding keyword and type vertices are merged together. A type-based summarization approach is then proposed to speed up the search performance.
8. Efficient and Progressive Group Steiner Tree Search (SIGMOD 2016) 🌟
> * To address the two limitations in [2], PrunedDP [8] is developed with optimal-tree decomposition techniques and conditional tree merging strategies. The search space of the parameterized DP algorithm is significantly reduced, and progressively-refined feasible solutions are conducted during the execution of the algorithm.

There are two major disadvantages of these summary graph based approaches discussed above. First, they do not interpret or understand the input keywords, but only target at finding a result tree with as small size as possible. The query intention behind the keywords are not comprehended. Second, the time complexity of the online search algorithm relies heavily on the graph size. As graph scale increases, efficiency becomes a challenging issue. 

9. Keyword Search on RDF Graphs — A Query Graph Assembly Approach (CIKM 2017) 🌟
> * To address both challenges, the query graph assembly (QGA) problem [67] is proposed to integrate the keyword disambiguation and query graph formulation into a uniform framework. A constraint-based bipartite graph matching solution with bound-based pruning approaches is proposed to solve the QGA problem. 
10. Keyword Search over Knowledge Graphs via Static and Dynamic Hub Labelings (WWW 2020) 🌟
> * KeyKG and KeyKG+ are proposed as practical approximation algorithms, while the quality of computed answers is guaranteed with very low run time to address the GST problem.
11. Fast Shortest-path Distance Queries on Road Networks by Pruned Highway Labeling (ALENEX 2014)
> * For the efficient computation of distances and shortest paths, Hub Labeling is utilized to label each vertex in a graph with a set of reachable vertices. In this way, the algorithms efficiently approximate GST-based keyword query answers. 
12. Keyword proximity search in complex data graphs (SIGMOD 2008) 🌟
> * Due to the NP completeness of the GST problem, it is impossible for the algorithms introduced above to achieve satisfactory quality with theoretical guarantee of either the delay between consecutive results or the approximation ratios of non-first results.
> * This paper addresses this issue by enumerating answer in 2-approximate increasing weight-correlated order by height, and a theoretical guarantee without missing any answers with small wights with polynomial delay. 
> * Specifically, by applying shortest-path iterators to identify the first answer as a minimal-rank feasible tree, the remaining answers are enumerated without redundancies based on the inclusion constraints and exclusion constraints.
13. Mining summaries for knowledge graph search (ICDM 2016) 🌟
> * Searching large-scale heterogenous knowledge graphs is still very challenging regarding the real-world resource constraints such as response time and memory.
> * This paper facilitates the knowledge graph search, by proposing a class of summaries characterized by graph patterns, and formulating the graph summarization as a bi-criteria pattern mining task. Efficient query evaluation algorithms are preformed by wisely choosing and accessing a small collection of summaries as the base graphs.

Furthermore, an important but unsolved issue is how to group and summarize the answer graphs which share similar contents and structures, under the requirement of better query interpretation and result understanding. 

14. Summarizing answer graphs induced by keyword queries (VLDB 2013) 🌟
> * This paper studies the summarization of the answer graphs induced by a keyword query. 
> * Specifically, to measure the information loss after the summarization, the coverage ratio, which is a quality metric of summary graphs, is designed. 
> * According to this metric, the authors formulate a set of summarization problems, with the target to determine the minimized summary graphs with the constraints of certain coverage ratio. Exact and heuristic summarization algorithms are proposed to solve the problems.

__1.2 Retrieval Based Keyword Query__

__1.3 Keyword Query Interpretation__

__1.2 Keyword Query on Spatial Knowledge Graphs__

__2. SPARQL Query on Knowledge Graphs__

__2.1 Efficiency Improvement in Traditional SPARQL Queries__

1. Faceted search over RDF-based knowledge graphs (Journal of Web Semantics 2016) [[Paper](https://www.sciencedirect.com/science/article/pii/S1570826815001432)] 
2. Semantic SPARQL similarity search over RDF knowledge graphs (VLDB 2016) [[Paper](https://dl.acm.org/doi/pdf/10.14778/2983200.2983201)] 🌟
3. Effective searching of RDF knowledge graphs (Journal of Web Semantics 2018) [[Paper](https://www.sciencedirect.com/science/article/pii/S1570826817300677)]

## Property Graphs
__General Papers__
1. Property Graph Schema Optimization for Domain-Specific Knowledge Graphs (ICDE 2021) [[Paper](https://arxiv.org/pdf/2003.11580.pdf)] 🌟


__Queries and Search over Property Graph based KG__
1. Sqlgraph: An efficient relational-based property graph store (SIGMOD 2015) 🌟
2. Cypher: An evolving query language for property graphs (SIGMOD 2018) 🌟
