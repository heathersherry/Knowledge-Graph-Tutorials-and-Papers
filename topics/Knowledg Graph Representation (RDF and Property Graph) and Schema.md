## Knowledg Graph Representation (RDF and Property Graph), Schema and Query
There are two major approaches to store and query knowledge graphs: (1) RDF (Resource Description Framework) data model with SPARQL query language, (2) property graph model with graph query languages such as Cypher. 

## RDF Graphs
__Surveys__
1. RDF Data Storage and Query Processing Schemes: A Survey [[Paper](https://dl.acm.org/doi/pdf/10.1145/3177850)]

__General Papers__
1. Relational schema optimization for RDF-based knowledge graphs (Information Systems 2021) [[Paper](https://www.sciencedirect.com/science/article/pii/S0306437921000223)] 

__Queries and Search over RDF based KG__

__1. Keyword search__

__1.1 Summary Graph-based Keyword Query__
1. Top-k exploration of query candidates for efficient keyword search on graph-shaped (rdf) data (ICDE 2009) 🌟
2. Finding top-k min-cost connected trees in databases (ICDE 2007) 🌟
3. Keyword search over RDF graphs (CIKM 2011) 🌟
> * [2] and [3] define the keyword search problem as a minimum connected tree [2] or a subgraph [3] over the data graph, while the target is to cover all the keyword by the nodes and edges of the derived tree or subgraph.
> * This problem definition is very close to the group Steiner tree problem (GST), which is proven to be NP-complete.
> * DPBF [2] guarantees to derive the exact optimal result of a minimum-weight GST with parameterized time complexity. However, DPBF still suffers from the exponential time and space complexity, especially on large graphs. Moreover, DPBF cannot generate a solution until the entire algorithm is completed.
4. Keyword searching and browsing in databases using BANKS (ICDE 2002) 🌟
5. Bidirectional expansion for keyword search on graph databases (VLDB 2005) 🌟
6. BLINKS:rankedkeyword searches on graphs (SIGMOD 2007) 🌟
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
> * According to this metric, the authors formulate a set of summarization problems, with the target to determine the minimized summary graphs with the constraints of certain coverage ratio. 
> * Exact and heuristic summarization algorithms are proposed to solve the problems.

__1.2 Retrieval-based Keyword Query__

Retrieval-based methods precompute an index a collection of size-bounded subgraphs as candidate answers.

1. EASE: an effective 3-in-1 keyword search method for unstructured, semi-structured and structured data （SIGMOD 2008）🌟
> * EASE processes keyword queries on the graph constructed based on the target heterogenous data. 
> * Specifically, instead of employing traditional inverted indices, EASE summarizes the graphs and constructs graph indices. 
> * To facilitate the keyword-based search, an extended inverted index is proposed together with a novel ranking mechanism to enhance the effectiveness of search.
2. Finding Top-k Answers in Keyword Search over Relational Databases Using Tuple Units (TKDE 2011) 🌟
> * Motivation: effectively answer keyword queries by integrating multiple related tuple units (instead of single unit) to answer a keyword query in many real-world scenarios.
> * SAINT devises single-keyword-based structure-aware index as well as keyword-pair-based structure-aware index. Then, the structural relationships between different tuple units are incorporated into these indexes, to identify the answers of integrated tuple units in an efficient manner. 
> * Moreover, novel ranking strategies and algorithms are developed to locate the top-k answers progressively.

__1.3 Keyword Query Interpretation__

These works first transform a keyword query into a structured query such as a SPARQL query. Then they  execute the structured query over the RDF graph to retrieve answers. 

1. Top-k Exploration of Query Candidates for Efficient Keyword Search on Graph-Shaped (RDF) Data (ICDE 2005) 🌟
> * They first conduct queries from the keywords while allowing the users to select the appropriate query. Moreover, to compute queries from keywords, they propose novel algorithms to determine the top-k exploration of subgraphs, which is guaranteed to compute all k subgraphs, including cyclic graphs, with the lowest costs.
2. Finding Patterns in a Knowledge Base using Keywords to Compose Table Answers (VLDB 2014) 🌟
> * This paper determines patterns which are relevant to the query based on a class of scoring functions in an efficient manner. They formulate a d-height tree pattern problem.
> * They formally define the tree patterns that aggregate subtrees in the knowledge graph which contains all the keywords within a query, while the tree patterns are expected to (1) figure out the semantics of keyword queries, (2) generate and compose the table answers. 
> * They further construct path-based indexes efficiently to discover the tree patterns for a given keyword query, and a sampling-based approach to provide approximate top-k to speed up query processing.

Moreover, to generate top-k interpretations aligned with user intentions, based on a user’s query context, context-aware approaches that aim at keyword query interpretation to personalizes the interpretation is proposed.

3. Effectively interpreting keyword queries on rdf databases with a rear view (ISWC 2011)
> * They study a sequence of structured queries associated with the interpretations of keyword queries in the query history. 
> * In detail, they propose a dynamic weighted summary graph model, which captures the representative characteristics of a user’s query history concisely. To extend the existing cost-balanced graph exploration algorithms, they further propose a top-k context-aware graph exploration algorithm, which is supported by biasing the exploration process based on context. 
> * Early termination conditions according to a notion of dominance is done to enhance the efficiency. 
4. Personalizing keyword search on RDF data (International Conference on Theory and Practice of Digital Libraries, 2013)
> * Based on the ranking SVM approach which trains ranking functions according to the RDF-specific training features, the rank personalization is conducted with the employment of historical user feedback.


__1.4 Keyword Query on Spatial Knowledge Graphs__

__2. SPARQL Query on Knowledge Graphs__

As the standard query language in RDF data model, SPARQL is widely used to query RDF-based knowledge graphs. [[SPARQL 1.1 Query Language](https://www.w3.org/TR/sparql11-query/)]


__2.1 Efficiency Improvement in Traditional SPARQL Queries__

__2.2 Distributed SPARQL Query Processing__

__2.3 From Natural Language Questions to SPARQL Queries__

__2.4 SPARQL Query Rewriting and Understanding__

__3. Facet Search over RDF Knowledge Graphs__

1. Faceted search over RDF-based knowledge graphs (Journal of Web Semantics 2016) [[Paper](https://www.sciencedirect.com/science/article/pii/S1570826815001432)] 
2. Semantic SPARQL similarity search over RDF knowledge graphs (VLDB 2016) [[Paper](https://dl.acm.org/doi/pdf/10.14778/2983200.2983201)] 🌟
3. Effective searching of RDF knowledge graphs (Journal of Web Semantics 2018) [[Paper](https://www.sciencedirect.com/science/article/pii/S1570826817300677)]

## Property Graphs
__General Papers__
1. Property Graph Schema Optimization for Domain-Specific Knowledge Graphs (ICDE 2021) [[Paper](https://arxiv.org/pdf/2003.11580.pdf)] 🌟


__Queries and Search over Property Graph based KG__
1. Sqlgraph: An efficient relational-based property graph store (SIGMOD 2015) 🌟
2. Cypher: An evolving query language for property graphs (SIGMOD 2018) 🌟
