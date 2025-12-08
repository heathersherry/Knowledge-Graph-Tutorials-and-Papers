## General Information Extraction

### General Papers
1. Improving Information Extraction from Visually Rich Documents using Visual Span Representations [[Paper](https://vldb.org/pvldb/vol14/p822-sarkhel.pdf)] (VLDB 2021) 🌟
2. Bootstrapping Information Extraction via Conceptualization (ICDE 2021) 🌟
3. C-ICL: Contrastive In-context Learning for Information Extraction (EMNLP 2024) [[Paper](https://arxiv.org/abs/2402.11254)]

### System works for Information Extraction
1. Doctopus: Budget-aware Structural Table Extraction from Unstructured Documents (VLDB 2025) 🌟 [[Paper](https://www.vldb.org/pvldb/vol18/p3695-chai.pdf)]
> * A system designed for accurate attribute extraction from unstructured documents with a user-specified cost constraint.
2. Sycamore
3. DocETL
4. Unstructured
5. Unify

## Open Information Extraction

### Sides, Tutorials and Surveys
1. Brief Introduction and Review of Open Information Extraction System [[Slides](https://ece.umd.edu/~smiran/OpenIE.pdf)]
2. A Survey on Open Information Extraction [[Paper](http://aclweb.org/anthology/C18-1326)]
3. Open Information Extraction on Scientific Text: An Evaluation [[Paper](http://aclweb.org/anthology/C18-1289)]
4. Open Information Extraction (OIE) Resources Summary [[Paper](https://github.com/gkiril/oie-resources)]

### OpenIE Tools or Works
1. Open Information Extraction from the Web (TextRunner, IJCAI 2007)
> * Incoherent Extractions 
> * Uninformative Extractions
2. MinIE: Minimizing Facts in Open Information Extraction (MinIE, EMNLP 2017) [[Code (java)](https://github.com/rgemulla/minie)] [[Code (python)](https://github.com/mmxgn/miniepy)]
> * Represent information about polarity, modality, attribution and quantities with semantic annotations (instead of actual extraction)
> * identify and remove parts that are considered over specific
3. Facts that Matter (SALIE, EMNLP 2018) [[Code](https://github.com/mponza/SalIE)]
> * Extract salient facts, which fulfil two requirements: (1) relevance and (2) diversity
4. Identifying Relations for Open Information Extraction (ReVerb, EMNLP 2011) [[Paper](http://www.aclweb.org/anthology/D11-1142)][[Code](https://github.com/knowitall/reverb)][[Homepage](http://reverb.cs.washington.edu/)]         
> * Use syntactic constraints to specify relation phrases (3 simple patterns). Find longest phrase matching one of the syntactic constraints. 
> * Find nearest noun-phrases to the left and right of relation phrase. - Not a relative pronoun or WHO-adverb or an existential there.
> * To avoid "over-specified" relation phrases, a relation phrase must have many distinct args in a large corpus
5. ClausIE: Clause-Based Open Information Extraction (ClausIE, WWW 2013) [[Paper](http://resources.mpi-inf.mpg.de/d5/clausie/clausie-www13.pdf)][[Code (Python)](https://github.com/AnthonyMRios/pyclausie)][[Code (Java)](https://github.com/IsaacChanghau/ClausIE)]
> * Map the dependency relations of an input sentence to clause constituents.
> * A set of coherent clauses presenting a simple linguistic structure is derived from the input
6. CycleOIE: A Low-Resource Training Framework For Open Information Extraction (COLING 2025) [[Paper](https://aclanthology.org/2025.coling-main.227/)]
7. The Search for Conflicts of Interest: Open Information Extraction in Scientific Publications (EMNLP 2025) [[Paper](https://hal.science/hal-05269842/)] 🔥 (LLM-based)

__Open Relation Extraction (ORE)__
1. LOREM: Language-consistent Open Relation Extraction from Unstructured Text (WWW 2020)
2. Topic-Oriented Open Relation Extraction with A Priori Seed Generation (EMNLP 2024) [[Paper](https://aclanthology.org/2024.emnlp-main.766.pdf)] 🔥
> PriORE leverages the built-in knowledge of LLMs to maintain a dynamic seed relation dictionary for the topic.

### Canonicalization of Open KB/KG, OpenIE Triple Clustering
__General Papers__
1. Query-Driven On-The-Fly Knowledge Base Construction (QKBfly, VLDB2017) relation clustering based on the PATTY dictionary 🌟 
2. CESI: Canonicalizing Open Knowledge Bases using Embeddings and Side Information (CESI, WWW 2018) [Code](https://github.com/malllabiisc/cesi) triple
3. Canonicalizing Open Knowledge Bases (CIKM 2014) triple 🌟 
4. Towards Practical Open Knowledge Base Canonicalization (FAC, CIKM 2018) triple 🌟
5. Identifying Relations for Open Information Extraction (ReVerb, EMNLP 2011)  [[Paper](http://www.aclweb.org/anthology/D11-1142)][[Code](https://github.com/knowitall/reverb)][[Homepage](http://reverb.cs.washington.edu/)] relation
> * Mophological Normalization
6. Open Information Extraction to KBP Relations in 3 Hours (TAC. 2013) [[Paper](https://pdfs.semanticscholar.org/d431/81fa9af5440360d4055e1ce7ddaaa6e82d77.pdf)]
> * Main idea: relation phrases mapping to KB otology
> * Manually define a set of rules for each relation, to conduct the mapping
> * The motivation and error analysis are well written
7. ClusType: Effective Entity Recognition and Typing by Relation Phrase-Based Clustering (ClusType, KDD 2015) 🌟
> * Relation Clustering: Two relation phrases tend to have similar cluster membershipd, if they have similar (1) strings; (2) context words; and (3) left and right argument type indicators
8. Unsupervised Methods for Determining Object and Relation Synonyms on the Web (Resolover, JAIR 2009) relation
9. Relation Extraction with Matrix Fatorization and Universal Schemes (NAACL-HLT 2013) [[Paper](http://www.aclweb.org/anthology/N13-1008)]
> * Close to relation clustering
> * Create a universal scheme by unioning surface form predicates from Open IE and relations in the schemas of pre-existing databases
10. Canonicalization of Open Knowledge Bases with Side Information from the Source Text (ICDE 2018) [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8731346)]  🌟
11. Canonicalizing Open Knowledge Bases with Multi-Layered Meta-Graph Neural Network （2020）[[Paper](https://arxiv.org/pdf/2006.09610.pdf)]
12. Joint Entity and Relation Canonicalization in Open Knowledge Graphs using Variational Autoencoders (2020) [[Paper](https://arxiv.org/abs/2012.04780)]
13. CaSIE: Canonicalize and Informative Selection of the OpenIE System (ICDE 2021, short) 🌟
14. Joint Entity and Relation Linking with Coherence Relaxation (SIGMOD 2021) 🌟 [[Paper](https://dl.acm.org/doi/abs/10.1145/3448016.3457280)]
15. Multi-level feature interaction for open knowledge base canonicalization (Knowledge-Based Systems 2024) [[Paper](https://www.sciencedirect.com/science/article/pii/S0950705124010207?__cf_chl_tk=VldX2UjfxVRSLXLYqj73WJ3IajVHYMNu4nwL6PPdh7A-1724223118-0.0.1.1-6249)]
16. Jointly Canonicalizing and Linking Open Knowledge Base via Unified Embedding Learning (WWW 2024) [[Paper](https://dl.acm.org/doi/10.1145/3589334.3645700)]
17. Enhancing Domain-Independent Knowledge Graph Construction through OpenIE Cleaning and LLMs Validation (International Conference on Knowledge-Based and Intelligent Information & Engineering Systems, 2024) [[Paper](https://hal.science/EC-NANTES/hal-04702397v1)] 🔥
18. CMVC+: a Multi-View Clustering Framework for Open Knowledge Base Canonicalization via Contrastive Learning (TKDE 2025) [[Paper](https://ieeexplore.ieee.org/abstract/document/10891880)] 🌟
>   * CMVC+ is a novel unsupervised framework for canonicalizing OKBs without the need for manually annotated labels.
>   * A multi-view CHF K-Means clustering algorithm mutually reinforces the clustering of view-specific embeddings learned from each view by considering the clustering quality in a fine-grained manner.
>   * A novel contrastive learning module refines the learned view-specific embeddings.
19. Open Knowledge Base Canonicalization with Multi-task Learning (WWW 2024) [[Paper](https://arxiv.org/pdf/2403.14733)]

__Relation Phrases Clustering (finding synonymous phrases and hypernyms)__
1. HARPY: Hypernyms and Alignment of Relational Paraphrases (HAPPY, COLING 2014) [[Paper](http://www.dit.unitn.it/~p2p/RelatedWork/Matching/harpy_COLING14.pdf)}{[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)]
2. POLY: Mining Relational Paraphrases from Multilingual Sentences (POLY, EMNLP 2016) [[Paper](https://www.aclweb.org/anthology/D16-1236)][[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)]
> * Make use of another language
3. RELLY: Inferring Hypernym Relationships Between Relational Phrases (REELY, EMNLP 2015) [[Paper](https://www.aclweb.org/anthology/D15-1113)}[[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)]
4. PATTY: A Taxonomy of Relational Patterns with Semantic Types (PATTY, EMNLP 2012) [[Paper](https://www.aclweb.org/anthology/D12-1104)][[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)]
5. Discovering and Exploring Relations on the Web (PATTY demo, VLDB 2012) [[Paper](http://vldb.org/pvldb/vol5/p1982_ndapandulanakashole_vldb2012.pdf)] 🌟
6. Ensemble Semantics for Large-Scale Unsupervised Relation Extraction (WEBRE, EMNLP-CoNELL 2012) relation
7. Relation Schema Induction using Tensor Factorization with Side Information (SICTF, EMNLP 2016) relation schema induction (for building domain-specific kb from unstructured text) [[Code](https://github.com/malllabiisc/sictf)]
8. Constrained Information-Theoretic Tripartite Graph Clustering to Identify Semantically Similar Relations (IJCAI 2015)

__Entity Summerazation__
1. ANTS: Abstractive Entity Summarization in Knowledge Graphs (ESWC 2025) [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-94575-5_8)] 🔥

__Other Canonicalization__
1.  Constructing Explainable Opinion Graphs from Reviews (WWW 2021) [[Paper](https://arxiv.org/pdf/2006.00119.pdf)]
> * Canicaliza opinion phrases

__Related Works__
1. Query-Efficient Correlation Clustering (WWW 2020)

__Clustering Methods Used for Canonicalization__
Note: So far most of the papers I read employ HAC for canonicalization for two major reasons: (1) no predefined number of clusters, (2) Un-sensitive to similarity metrics. The standard algorithm for hierarchical agglomerative clustering (HAC) has a time complexity of O(n^3) and requires O(n^2) memory.
1. An efficient algorithm for a complete link method. Comput. J. 20, 4 (1977), complete linkage, O(n^2)
2. A Hierarchical Algorithm for Extreme Clustering (KDD 2017), approximate Hierarchical clustering algorithms at the cost of some loss in performance.
3. SLINK: an optimally efficient algorithm for the single-link cluster method, O(n^2)

__Benchmarks__
1. BenchIE^FL: A Manually Re-Annotated Fact-Based Open Information Extraction Benchmark (ACL 2024) [[Paper](https://aclanthology.org/2024.findings-acl.496.pdf)]

### Other Interesting Works about Open IE
1. Intergring Local Context and Global Cohesiveness for Open Information Extraction (ReMine, WSDM 2019)
> * Solving a joint optimization problem to unify (1) segmenting entity/relation phrases in individual sentences based on local context; and (2) measuring the quality of tuples extracted from individual sentences with a translating-based objective.
2. Extracting Knowledge from Web Text with Monte Carlo Tree Search (WWW 2020, short paper)
3. OpenKI: Integrating Open Information Extraction and Knowledge Bases with Relation Inference (NAACL 2019)
4. On Aligning OpenIE Extractions with Knowledge Bases: A Case Study (ACL 2020) [[Paper](https://www.aclweb.org/anthology/2020.eval4nlp-1.14.pdf)]
5. Syntactic and Semantic-driven Learning for Open Information Extraction (EMNLP 2020) [[Paper](https://www.aclweb.org/anthology/2020.findings-emnlp.69.pdf)]

## Joint Multimodal Entity-Relation Extraction (JMERE) 
### Research Papers
1. CAG: A Consistency-Adaptive Text-Image Alignment Generation for Joint Multimodal Entity-Relation Extraction (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679883)]
2. Enhancing Multimodal Object-Entity Relation Extraction via Multi-Aspect Contrastive Learning in Large Multimodal Models (IEEE Transactions on Audio, Speech and Language Processing, 2025) [[Paper](https://ieeexplore.ieee.org/abstract/document/10910215)]
