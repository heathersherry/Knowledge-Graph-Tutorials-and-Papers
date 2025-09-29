# General KG Queries and Knowledge Search

## 📝 General Papers
1. Semantic Guided and Response Times Bounded Top-k Similarity Search over Knowledge Graphs [[Video](https://www.google.com/url?q=https://drive.google.com/open?id%3D1ejMq8cZrTZT1Nn0D-zaMlW7X7ESkSDro&sa=D&ust=1587488616453000&usg=AFQjCNEeyFqVvX9q4QWy8jc4jHfpdEc2Zw)][[Slides](https://www.google.com/url?q=https://drive.google.com/open?id%3D1JyhtaWEeRvzS6TmIuplZNd5ZId3Larpz&sa=D&ust=1587488616453000&usg=AFQjCNEI5es_-rKQs-eUImsqivdAFNAnvw)][[Paper](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300a445/290300a445.pdf)] (ICDE 2020) 🌟
2. Online Indices for Predictive Top-k Entity and Aggregate Queries on Knowledge Graphs [[Video](https://www.google.com/url?q=https://drive.google.com/open?id%3D12mo2_5abIbU9BDxrI4eSPsZ-SFDRgMAN&sa=D&ust=1587488616485000&usg=AFQjCNHwZw7kP6JJ2nIbDiMT4FvlwebmsA)][[Slides](https://www.google.com/url?q=https://drive.google.com/open?id%3D1Vy15Q81aZg6Kn0AKqcJQ1LraCAb7ZyPy&sa=D&ust=1587488616485000&usg=AFQjCNEqOaDue8W4ZN91-2I2JPLkQTE3jw)][[Paper](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300b057/290300b057.pdf)] (ICDE 2020) 🌟
4. Effective searching of RDF knowledge graphs (Journal of Web Semantics 2018) [[Paper](https://www.sciencedirect.com/science/article/pii/S1570826817300677)]
5. An analytical study of large SPARQL query logs (VLDBJ 2020) 🌟
6. Keyword Search over Knowledge Graphs via Static and Dynamic Hub Labelings (WWW 2020)  [[Paper](https://dl.acm.org/doi/pdf/10.1145/3366423.3380110)] 🌟
7. Graph-Query Suggestions for Knowledge Graph Exploration (WWW 2020, short paper)
8. Mining summaries for knowledge graph search (ICDM 2016)
9. Efficient Computation of Semantically Cohesive Subgraphs for Keyword-Based Knowledge Graph Exploration (WWW 2021) 
10. WiseKG: Balanced Access to Web Knowledge Graphs (WWW 2021)
11. Self-Supervised Hyperboloid Representations from Logical Queries over Knowledge Graphs (WWW 2021)
12. Querying subjective data [[Paper](https://link.springer.com/article/10.1007/s00778-020-00634-5)] (VLDBJ 2021) 🌟
13. Materializing Knowledge Bases via Trigger Graphs (VLDB 2021) [[Paper](https://vldb.org/pvldb/vol14/p943-tsamoura.pdf)] 🌟
14. Fast Core-based Top-k Frequent Pattern Discovery in Knowledge Graphs (ICDE 2021) 🌟
15. NewsLink: Empowering Intuitive News Search with Knowledge Graphs (ICDE 2021) 🌟
16. Versatile Equivalences: Speeding up Subgraph Query Processing and Subgraph Matching (SIGMOD 2021) 🌟

# KG Representation (RDF and Property Graph), Schema and Query
There are two major approaches to store and query knowledge graphs: (1) RDF (Resource Description Framework) data model with SPARQL query language, (2) property graph model with graph query languages such as Cypher. 

## 📝 RDF Graphs
### Surveys
1. RDF Data Storage and Query Processing Schemes: A Survey [[Paper](https://dl.acm.org/doi/pdf/10.1145/3177850)]

### General Papers
1. Relational schema optimization for RDF-based knowledge graphs (Information Systems 2021) [[Paper](https://www.sciencedirect.com/science/article/pii/S0306437921000223)] 
2. Efficient Exploration of Interesting Aggregates in RDF Graphs (SIGMOD 2021) 🌟
3. Optimizing Multi-Query Evaluation in Federated RDF Systems [[Paper](https://ieeexplore.ieee.org/document/8868210)] 🤩 (TKDE 2021) 🌟

### Queries and Search over RDF based KG

### 1. Keyword search

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

The target is to locate a subtree that covers all the query keywords. Specifically, there are essential requirements for the retrieved subtree rooted at a place vertex. First, it should be spatially close to a query location. Second, it should be compact in terms of the query keywords.

1. Top-k Relevant Semantic Place Retrieval on Spatial RDF Data (SIGMOD 2016) 🌟
2. Top-k relevant semantic place retrieval on spatiotemporal RDF data (VLDBJ 2019) 🌟
> * [1] and [2] investigate a location-based keyword search query on RDF data. In detail, the top-k relevant semantic places (kSP) retrieval [1] aims to determine specific RDF subgraphs that meet the following requirements: (1) they contain the query keywords which rooted at spatial entities, and (2) they are close to the query location. Specifically, such kSP queries are location-sensitive, without employing any structured query language. In addition, two pruning approaches with a data preprocessing technique are introduced, to further accelerate the kSP retrieval. 
To add temporal semantics to the kSP query, [2] introduces the kSPT query that incorporates temporal information by: (1) integrating the temporal differences between the keyword-matched vertices and the query timestamp, or (2) employing a temporal range to filter keyword-matched vertices.

In real-world scenarios, employing a single subtree may not satisfy the user requirements. Therefore, collective spatial keyword query (CSKQ) is proposed, so that a group of subtrees are integrated to collectively cover the query keywords.

3. Collective keyword query on a spatial knowledge base (TKDE 2018) 🌟
> * This work introduces and formulates a spatial keyword query problem on a knowledge base, i.e., CoSKQ-KB. Specifically, the CoSKQ-KB problem determines a set of semantic places that collectively cover the query keywords with the target to minimize a ranking function, which is derived based on spatial closeness and keyword relevance. Moreover, to measure the travel distance of a user who visit all the member semantic places, a hub-based MaxSum distance is proposed. This work also proposes the BCK algorithm, which reduces the search spaces to address the CoSKQ-KB problem, by employing efficient pruning techniques, as well as the iSCK algorithm, which enhances BCK with dynamic bounds for the early termination of iterations.
4. Collectivespatial keyword querying (SIGMOD 2011)
5. Inherent-cost aware collective spatial keyword queries (SSTD 2017)
6. Efficient collective spatial keyword query processing on road networks (IEEE Trans. Intell. Transp. Syst., 2017)

### 2. SPARQL Query on Knowledge Graphs

As the standard query language in RDF data model, SPARQL is widely used to query RDF-based knowledge graphs. [[SPARQL 1.1 Query Language](https://www.w3.org/TR/sparql11-query/)]

__2.1 Efficiency and Correctness Improvement in Traditional SPARQL Queries__

Conventional methods that investigate SPARQL queries over RDF-based knowledge graphs mainly suffer from two limitations. First, they are not able to produce answers for the SPARQL queries with wildcards with scalable approaches. Second, they are not able to deal with the frequent updates in RDF repositories in an efficient manner. 

1. gStore: answering SPARQL queries via subgraph matching (VLDB 2011) 🌟
> * This work proposes a graph-based approach to store the RDF data. They convert a SPARQL query into a subgraph matching query. To accelerate the query processing, they design VS-tree and VS∗-tree as indexes, together with effective pruning rules and efficient search algorithms, which are embedded into the query algorithms that determine the answers for both exact SPARQL queries and queries with wildcards uniformly and seamlessly.
2. Passage: Ensuring Completeness and Responsiveness of Public SPARQL Endpoints with SPARQL Continuation Queries (WWWW 2025)
> * PASSAGE ensures the completeness and responsiveness of SPARQL while delivering high performance

__2.2 Distributed SPARQL Query Processing__

Because of the sheer size, the heterogeneity, and the further complexity brought by RDF reasoning, managing the large volumes of RDF data remains as a challenging issue. To address this size challenge, distributed storage architectures and distributed SPARQL query processing are proposed and investigated by many research works.

1. RDF in the clouds: a survey (VLDBJ 2015) 🌟(a very good survey! 🥳)

The first category of works focus on managing RDF datasets using cloud platforms. 

2. S2RDF: RDF querying with SPARQL on spark (VLDB 2016) 🌟
> * To minimize the query input size regardless of its pattern structure and diameter in an efficient manner, S2RDF describes ExtVP, a novel relational partitioning schema for RDF data, which utilizes a semi-join based preprocessing akin to the concept of join indices in relational databases. S2RDF is constructed on Spark, where the relational interfaces are utilized to execute the SPARQL queries over ExtVP. 
3. S2X: Graph-Parallel Querying of RDF with GraphX (BigO(Q)/DMAH@VLDB 2015) 🌟
> * S2X employs GraphX in Spark to conduct evaluation on the SPARQL queries. Specifically, S2X distributes all triple patterns to all vertices. Afterwards, the vertices validate their triple candidacy with their neighbors via exchanging messages. Finally, S2X collects and merges the partial results.

The second category of works are partition-based, where the large RDF graph are divided into different partitions while each partition is stored in a site managed by a centralized RDF system. In this scenario, a SPARQL is decomposed into several subqueries at run time, while the subqueries can be executed and answered locally by one of the sites. Afterwards, the results of the all the subqueries are integrated.

4. Scalable SPARQL Querying Using Path Partitioning (ICDE 2015) 🌟
> * PathBMC decomposes the large-scale RDF graph into multiple path preserving data partitions. It then generates a collection of complex SPARQL queries to be inner-partition queries. Therefore, it can largely reduce or even avoid the cost of distributed joins over the large-scale RDF graph. 
5. DiploCloud: Efficient and Scalable Management of RDF Data in the Cloud (TKDE 2015) 🌟
> * DiploCloud performs a physiological analysis on the instance and schema information which is prior to partitioning the data. Specifically, it requires the administrator to define a set of templates as the partition unit, and stores the instantiations of the templates in compact lists as in a column-oriented database system.
6. Query Workload-based RDF Graph Fragmentation and Allocation (EDBT 2016)
> * This work conducts mining and selection of a set of frequent access patterns, which partition the RDF graph into several smaller fragments. Moreover, an allocation algorithm that distributes all such fragments over distinct sites is further proposed. Finally, according to the fragmentation and allocation results, the query are processed.

However, the partitions proposed by most techniques are static. In other words, these patterns are not capable of adapting themselves to diverse changes within the query workload. Consequently, there are a few drawbacks. First, the existing approaches cannot consistently avoid the communication cost of the queries not favored or supported by the initial data partitioning. Second, for large-scale universal RDF knowledge graphs, the partitioning phase is likely to be expensive due to the high startup costs. 

7. Accelerating SPARQL Queries by Exploiting Hash-based Locality and Adaptive Partitioning (VLDBJ 2016) 🌟
8. Evaluating SPARQL Queries on Massive RDF Datasets (VLDB 2015) 🌟
> * To address the above shortcomings, AdPart [7] and AdHash [8] apply lightweight hash partitioning that significantly reduces the startup cost. Specifically, the parallel processing of join patterns on subjects without any communication is favored by the partitioning. Through redistributing and replicating the frequently accessed data in an incremental manner, they further monitor the data access patterns, which are adapted to the query load dynamically. Therefore, the communication cost for future queries is eliminated or significantly reduced. 

There are also another category of works that employ neither cloud platforms nor PDF graph partitioning. 

9. DREAM: distributed RDF engine with adaptive query planner and minimal communication (VLDB 2015) 🌟
> * DREAM avoid partitioning RDF datasets but partition only SPARQL queries. 
> * DREAM generates a general paradigm for various types of pattern matching queries without partitioning datasets. In particular, only auxiliary data are shuffled. Moreover, DREAM can adaptively select a suitable set of machines, by partitioning queries. Based on a graph-based query planner with a novel cost model, they largely maximizes the parallelism and minimizes auxiliary data communication for a certain given query, with a new rule-oriented query partitioning strategy.
10. Processing SPARQL Queries over Distributed RDF Graphs (VLDBJ 2016) 🌟
> * This work investigates a graph-based approach to conduct distributed SPARQL query processing based on the partial evaluation and assembly approaches.
> * There are two major steps. First, they conduct query evaluation on each graph fragment in a parallel manner, to determine the local partial matches which is the overlapping parts between a crossing match and a fragment. Then, they apply two distinct assembly strategies to assemble the local partial matches to derive crossing matches: (1) centralized assembly, which sends all the local partial matches to a single site, (2) distributed assembly, which assembles the local partial matches at a collection of sites in parallel.

Recently, to evaluate queries on distributed graphs, partial evaluation has been proposed.

11. Performance Guarantees for Distributed Reachability Queries (VLDB 2012) 🌟
12. Distributed Set Reachability (SIGMOD 2016) 🌟
> * Both works present algorithms to evaluate reachability queries on distributed graphs.
13. Distributed Graph Simulation: Impossibility and Possibility (VLDB 2014) 🌟
14. Distributed Graph Pattern Matching (WWW 2012)
> * Both works propose partial evaluation algorithms as well as optimizations to conduct distributed graph simulation.

Specifically, to deal with SPARQL queries over a distributed RDF graph, [10] employ the “partial evaluation and assembly” framework. However, this work does not provide theoretical performance guarantees on the response time and the data shipment. 

15. Accelerating Partial Evaluation in Distributed SPARQL Query Evaluation (ICDE 2019) 🌟
> * This work improve the “partial evaluation and assembly” framework [10] and provides performance guarantees. To further enhance the partial evaluation-based distributed SPARQL query processing approach, there are three optimizations performed: (1) compress the partial evaluation results in LEC feature which is a compact data structure, and communicate them among different sites, in order to prune out the irrelevant partial evaluation results with performance guarantees, (2) conduct the LEC feature-based assembly of all the local partial matches, in order to cut down the search space, and (3) communicate the candidates of the variables among the sites, in order to eliminate the irrelevant local partial matches.

__2.3 From Natural Language Questions to SPARQL Queries__

The Question Answering (QA) systems based on knowledge graphs can interpret the questions raised by the users as SPARQL query, and return a set of answers retrieved from the RDF-based knowledge graph. Nevertheless, due to the complexity of entity linking and predicate linking, which aims to link natural phrases to specific RDF items, it is still challenging to understand users’ questions precisely. As a result, the answer set may not satisfy the expectation of users if it offers wrong answers and neglects part of the correct answers. There are many works that study this problem, aiming at interpreting the users’ questions to SPARQL queries precisely and efficiently. 

1. Template-based question answering over RDF data (WWW 2012)
> * Leveraging a parse of the question, [1] generates a SPARQL template that mirrors the internal structure of the question directly. Then, through employing statistical entity identification and predicate detection, the template is instantiated. 
2. Evaluation of a Layered Approach to Question Answering over Linked Data (ISWC 2012)
> * Similar to [1], based on part-of-speech tags, BELA [2] utilizes a lexical tree adjoining grammar to parse the input queries. This parsing produces a collection of SPARQL query templates, while each template is associated with a potential interpretation of the given query. Furthermore, an inverted index constructed from DBpedia entity names is consulted, in order to fill in the unknown slots in the SPARQL queries.
3. Natural language questions for the web of data (EMNLP-CoNLL 2012) 🌟
> * DENNA [3] is another work that translates the natural language questions to SPARQL templates. It address this issue by constructing a disambiguation graph, and further reducing the disambiguation task to an integer linear programming (ILP) problem.

There are a group of methods that do not adopt any manually defined SPARQL templates.

4. Natural language question answering over RDF: a graph data driven approach (SIGMOD 2014) 🌟
> * To answer the natural language questions over RDF repository from a graph data-driven perspective, Zou et al. [4] propose a systematic framework. Specifically, they construct a semantic query graph which manipulates and models the query intention in the natural language question in a structural manner. The RDF-based question answering task is then reduced to subgraph matching problem based on the query graph. One of their essential technical contributions is to resolve the ambiguity of natural language questions when locating the matches of query. 
5. IMPROVE-QA: an interactive mechanism for RDF question/answering systems (SIGMOD 2018) 🌟
> * Zhang et al. [6] develop an Interactive Mechanism aiming for Promotion Via feedback to QA systems, which is called IMPROVE-QA. This platform enable the existing QA systems to return answers that are more precise to users. According to the user’s feedback over the answer set, IMPROVE-QA automatically refines the original query into a new query graph with minimum modifications.

__2.4 SPARQL Query Rewriting and Understanding__

Another approach to process SPARQL queries is query rewriting. The first category of works rewrite the SPARQL queries to another target query language, while delegating their execution and optimization and to an engine which supports the target query language. Some of the works rewrite the SPARQL query to SQL, which enables the existing optimizations of relational database engines to be conducted. Some of the works rewrite SPARQL to existing graph query languages such as Gremlin that support navigational features. Moreover, on graph databases, there are also many works study the query rewriting.

1. Efficient answering of why-not questions in similar graph matching (TKDE 2015) 🌟
> * Islam et al. [1] rewrite queries to conduct graph similarity search, with the target to minimize the edit distance between the query and the returned result.
2. Graph Query Reformulation with Diversity (KDD 2015) 🌟
> * This work proposed produces a collection of diverse queries, with the target to cover the original query results by these query results, and hence can be utilized to assist the users to understand and explore the underlying graph database. 

However, most works target at producing only one output node in the given query. Obviously, this simplifies inputs from the users, and hence limits its application in real-world scenarios where users’ interest are based on most or all the nodes in the query. 

3. SPARQL Rewriting: Towards Desired Results (SIGMOD 2020) 🌟
> * To address this user-related issue in knowledge graphs, this work narrows the gap between the actual meaning of a SPARQL query and the user’s real desire, by proposing a set of modifiers for a given query. Specifically, this problem is modelled as two individual sub-problems. The first problem is the query-restricting problem, which is proven to be NP-hard and has no polynomial-time approximation scheme (PTAS). To address the query-restricting problem, a (1−1/e)-approximation method is introduced. The second problem is the query-relaxing problem, which is proven to be NP-hard and has no polynomial-time constant-factor approximation algorithm. Two heuristic strategies are proposed to address the query-relaxing problem.

Furthermore, because of the “schema-free” nature of RDF data, the systems are likely to adopt distinct schemas to represent the same real-world facts. Therefore, complex SPARQL queries containing multiple UNION operators are needed, if the users require multiple answers to one question. Obviously, there are two challenges. First, it is too hard for common users or even the professional users to conceive and generate the complicated SPARQL queries, which both consider the flexible underlying schemas and conform to the syntax. Second, the same knowledge can be captured and represented in diverse graph fragments. 

4. Semantic SPARQL Similarity Search Over RDF Knowledge Graphs (VLDB 2016) 🌟 [[Paper](https://dl.acm.org/doi/pdf/10.14778/2983200.2983201)]
> * This work investigates semantics-based SPARQL similarity search over RDF knowledge graphs. They introduce an instance-driven approach to discover and mine the semantic graph patterns, by taking the diverse semantically equivalent graph structures into account. They then propose semantic graph edit distance as a novel similarity measure, which is based on the semantic graph patterns. To facilitate the query processing, they devise semantic summary graph as an efficient index. The input query graphs are rewritten at query time. Finally, a two-level pruning strategies is conducted to further reduce the search space and achieve satisfactory efficiency. 

### 3. Facet Search over RDF Knowledge Graphs

Although SPARQL queries are popular and widely adopted in the RDF-data model, it is impossible for most users to write SPARQL queries to search in knowledge graphs, which requires professionality and proficiency in the query language. Therefore, a challenging research issue in the Semantic Web community is the design and implementation of simple but powerful query interfaces for non-expert users. As for the large-scale universal knowledge graphs such as DBpedia, Wikidata or Freebase which provide end-users searching services, this challenge becomes even more critical.

To address this problem, faceted search is proposed as a prominent approach, which conducts queries on the entities while users are capable of narrowing down the search results according to their requirements. This is achieved by applying filters called facets progressively. Typically, a facet contains a predicate (e.g., ‘first name’ or ‘occupation’ when querying entities typed as person), as well as a collection of strings (e.g., ‘professor’). Generally, the entities in the collection are annotated with predicate-value pairs. Specifically, the users conduct selection of facet values iteratively during the faceted search. The entities annotated based on the selection are returned as the query result. 

1. Semantic enrichment of web search results at real-time (SIGIR 2016)
2. Faceted search over RDF-based knowledge graphs (Journal of Web Semantics 2016) [[Paper](https://www.sciencedirect.com/science/article/pii/S1570826815001432)] 
> * This work proposes rigorous theoretical underpinnings for faceted search. Specifically, by employing faceted search are identified as a query paradigm, well-defined fragments of SPARQL can be captured. Arenas et al. also investigate the problem of updating faceted interfaces. To guide the faceted navigation, which aims to guide the users to formulate meaningful queries during exploratory search, they present a facet graph, which is a graph-based representation of OWL 2 ontologies as well as their logical entailments. According to the information in the graph, genetic interface generation and update algorithms are proposed. 


## 📝 Property Graphs
### General Papers
1. Property Graph Schema Optimization for Domain-Specific Knowledge Graphs (ICDE 2021) [[Paper](https://arxiv.org/pdf/2003.11580.pdf)] 🌟

### Queries and Search over Property Graph based KG
1. Sqlgraph: An efficient relational-based property graph store (SIGMOD 2015) 🌟
2. Cypher: An evolving query language for property graphs (SIGMOD 2018) 🌟
3. CYPHERBENCH: Towards Precise Retrieval over Full-scale Modern Knowledge Graphs in the LLM Era (ACL 2025) [[Paper](https://aclanthology.org/anthology-files/anthology-files/pdf/acl/2025.acl-long.438.pdf)] `rdf` `cypher`  🔥

## 📝 Other Query Problems on Knowledge Graphs
1. Ranking Indicator Discovery from Very Large Knowledge Graphs [[Paper](https://vldb.org/pvldb/volumes/18/paper/Ranking%20Indicator%20Discovery%20from%20Very%20Large%20Knowledge%20Graphs)]


