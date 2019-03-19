Useful Papers and Slides(as per topic)
======

Knowledge Base Construction (Demo or System)
---
1. CurEx – A System for Extracting, Curating, and Exploring Domain-Specific Knowledge Graphs from Text [CurEx, CIKM 2018]
2. Mining Structures of Factual Knowledge from Text: An Effort-Light Approach [PhD Thesis of Prof Xiang Ren]
3. DeepDive: Incremental Knowledge Base Construction Using DeepDive [VLDB 2015] {[Paper](http://www.vldb.org/pvldb/vol8/p1310-shin.pdf)} {[Slides](https://slideplayer.com/slide/14894493/)}{[Project link](http://deepdive.stanford.edu/)}
> * Distant Supervision; Build a fator graph containing both relation phrases and features.



Entity Extraction and Entity Typing
----
1. Knowledge Vault: A Web-Scale Approach to Probabilistic Knowledge Fusion [Knowledge Vault, KDD 2014]
2. ClusType: Effective Entity Recognition and Typing by Relation Phrase-Based Clustering [ClusType, KDD2015] (Also Relation Clustering) croase-grained entity typing
3. Label Noise Reduction in Entity Typingby Heterogeneous Partial-Label Embedding [PLE, KDD 2016] fine-grained entity typing
4. AFET: Automatic Fine-Grained Entity Typing byHierarchical Partial-Label Embedding [AFET, EMNLP 2016] fine-grained entity typing
5. A survey of named entity recoginition and classification {[Paper](https://nlp.cs.nyu.edu/sekine/papers/li07.pdf)}
6. No Noun Phrase Left Behind: Detecting and Typing Unlinkable Entities [EMNLP-CoNLL 2012]{[Paper](https://aclweb.org/anthology/D12-1082)}



Relation Extraction 
----
Tutorial:
1. A SURVEY ON RELATION EXTRACTION (CMU) {[Paper](http://www.cs.cmu.edu/~nbach/papers/A-survey-on-Relation-Extraction-Slides.pdf)}
2. Relation Extraction: CSE 517: Natural Language Processing {[Slides](https://courses.cs.washington.edu/courses/cse517/13wi/slides/cse517wi13-RelationExtraction.pdf)}
3. Relation Extraction II: CSE 517: Natural Language Processing {[Slides](https://courses.cs.washington.edu/courses/cse517/13wi/slides/cse517wi13-RelationExtractionII.pdf)}

Papers:
1. CoType: Joint Extraction of Typed Entities and Relations with Knowledge Bases [CoType, WWW2017]
https://blog.csdn.net/hqc888688/article/details/73559365
2. [g]Knowledge-Based Weak Supervision for Information Extraction of Overlapping Relations {[Code](http://aiweb.cs.washington.edu/ai/raphaelh/mr/)}{[Slides](https://www.slideserve.com/anila/knowledge-based-weak-supervision-for-information-extraction-of-overlapping-relations)} 
> * Recently, researchers have developed multi- instance learning algorithms to combat the noisy training data that can come from heuristic labeling, but their models assume relations are disjoint . for example they cannot extract the pair Founded(Jobs, Apple) and CEO-of(Jobs, Apple). This paper presents a novel approach for multi-instance learning with overlapping relations that combines a sentence-level extraction model with a simple, corpus-level component for aggregating the individual facts. 
3. [g]Modeling missing data in distant supervision for information extraction [ACL2013] missing data problem(?)


Open Information Extraction 
-----
Sides, Tutorials and Surveys
1. Brief Introduction and Review of Open Information Extraction System {[Slides](https://ece.umd.edu/~smiran/OpenIE.pdf)}
2. A Survey on Open Information Extraction {[Paper](http://aclweb.org/anthology/C18-1326)}
3. Open Information Extraction on Scientific Text: An Evaluation {[Paper](http://aclweb.org/anthology/C18-1289)}

OpenIE Tools:
1. Open Information Extraction from the Web [TextRunner, IJCAI 2007]
> * Incoherent Extractions 
> * Uninformative Extractions
2. MinIE: Minimizing Facts in Open Information Extraction [MinIE, EMNLP 2017] [Code](https://github.com/rgemulla/minie) (java)
> * Represent information about polarity, modality, attribution and quantities with semantic annotations (instead of actual extraction)
> * idetify and remove parts that are considered over specific
3. Facts that Matter [SALIE, EMNLP 2018] {[Code](https://github.com/mponza/SalIE)}
> * Extract salient facts, which fulfill two requirements: (1) relevance and (2) diversity
4. Identifying Relations for Open Information Extraction [ReVerb, EMNLP 2011] {[Paper](http://www.aclweb.org/anthology/D11-1142)}{[Code](https://github.com/knowitall/reverb)}{[Homepage](http://reverb.cs.washington.edu/)}                  
> * Use syntactic constraints to specify relation phrases (3 simple patterns). Find longest phrase matching one of the syntactic constraints. 
> * Find nearest noun-phrases to the left and right of relation phrase. - Not a relative pronoun or WHO-adverb or an existential there.
> * To Avoid "overspecified" relation phrases, a relation phrase must have many distinct args in a large corpus



OpenIE Triple Clustering:
1. Query-Driven On-The-Fly Knowledge Base Construction [QKBfly, VLDB2017] relation
2. CESI: Canonicalizing Open Knowledge Bases using Embeddings and Side Information [CESI, WWW2018] [Code](https://github.com/malllabiisc/cesi) triple
3. Canonicalizing Open Knowledge Bases [CIKM 2014] triple
4. Towards Practical Open Knowledge Base Canonicalization [FAC, CIKM 2018] triple
5. Identifying Relations for Open Information Extraction [ReVerb, EMNLP 2011]  {[Paper](http://www.aclweb.org/anthology/D11-1142)}{[Code](https://github.com/knowitall/reverb)}{[Homepage](http://reverb.cs.washington.edu/)} relation
> * Mophological Normalization
6. Open Information Extraction to KBP Relations in 3 Hours [TAC. 2013] {[Paper](https://pdfs.semanticscholar.org/d431/81fa9af5440360d4055e1ce7ddaaa6e82d77.pdf)}
> * Main idea: relation phrases mapping to KB otology
> * Manually define a set of rules for each relation, to conduct the mapping
> * The motivation and error analysis are well written.
7. ClusType: Effective Entity Recognition and Typing by Relation Phrase-Based Clustering [ClusType, KDD2015] 
> * Relation Clustering: Two relation phrases tend to have similar cluster membershipd, if they have similar (1) strings; (2) context words; and (3) left and right argument type indicators
8. Unsupervised Methods for Determining Object and Relation Synonyms on the Web [Resolover, JAIR 2009] relation
9. Relation Extraction with Matrix Fatorization and Universal Schemes [NAACL-HLT 2013] close to relation clustering
> * Create a universal scheme by unioning surface form predicates from Open IE and relations in the schemas of pre-existing databbases.

6. [g]Ensemble Semantics for Large-Scale Unsupervised Relation Extraction [WEBRE, EMNLP-CoNELL 2012] relation
7. [g]Relation Schema Induction using Tensor Factorization with Side Information [SICTF, EMNLP 2016] relation schema induction (for building domain-specific kb from unstructured text) Code: https://github.com/malllabiisc/sictf
8. [g]Constrained Information-Theoretic Tripartite Graph Clustering to Identify Semantically Similar Relations [IJCAI 2015]

Graph Embedding and Learning
----
1. DeepWalk: Online Learning of Social Representations [DeepWalk, KDD 2014] [Code] (https://github.com/phanein/deepwalk Slides: https://www.slideshare.net/bperz/14-kdddeep-walk-2)
2. [g]DeepPath: A Reinforcement Learning Method for Knowledge Graph Reasoning [DeepPath, EMNLP 2017] [Code](https://github.com/xwhan/DeepPath Notes: https://zhuanlan.zhihu.com/p/33536026)

Knowledge Base Refinement
----
1. Knowledge Graph Refinement:A Survey of Approaches and Evaluation Methods


Tutorials and Notes from Talented People
=====
About Knowledge Graphs
---
1. https://kgtutorial.github.io An introduction to knowledge graph and knowledge extraction from unstructured text.
2. https://github.com/impillar/knowledge_graph/blob/master/README.md 
3. https://github.com/BrambleXu/knowledge-graph-learning
4. https://github.com/Pelhans/Z_knowledge_graph
5. https://zhuanlan.zhihu.com/p/44904796
6. Information Extraction by Niranjan Balasubramanian {Slides in my Mac}


Others
---
1. Probabilistic Graphical Models: Lagrangian Relaxation Algorithms for Natural Language Processing {[Slides](http://people.csail.mit.edu/dsontag/courses/pgm12/slides/lecture3.pdf)}
2. Introduction to Conditional Random Fields {[Blog](http://blog.echen.me/2012/01/03/introduction-to-conditional-random-fields/)}
