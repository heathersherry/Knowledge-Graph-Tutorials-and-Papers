Useful Papers and Slides (as per Topic)
======

## Topic 1: Knowledge Base Construction (Demo or System)
1. CurEx – A System for Extracting, Curating, and Exploring Domain-Specific Knowledge Graphs from Text [CurEx, CIKM 2018]
2. Mining Structures of Factual Knowledge from Text: An Effort-Light Approach [PhD Thesis of Prof Xiang Ren]
3. DeepDive: Incremental Knowledge Base Construction Using DeepDive [VLDB 2015] {[Paper](http://www.vldb.org/pvldb/vol8/p1310-shin.pdf)} {[Slides](https://slideplayer.com/slide/14894493/)}{[Project link](http://deepdive.stanford.edu/)}
> * Distant Supervision; Build a fator graph containing both relation phrases and features.


## Topic 2: Entity Extraction and Entity Typing
1. Knowledge Vault: A Web-Scale Approach to Probabilistic Knowledge Fusion [Knowledge Vault, KDD 2014]
2. ClusType: Effective Entity Recognition and Typing by Relation Phrase-Based Clustering [ClusType, KDD2015] (Also Relation Clustering) croase-grained entity typing
3. Label Noise Reduction in Entity Typingby Heterogeneous Partial-Label Embedding [PLE, KDD 2016] fine-grained entity typing
4. AFET: Automatic Fine-Grained Entity Typing byHierarchical Partial-Label Embedding [AFET, EMNLP 2016] fine-grained entity typing
5. A survey of named entity recoginition and classification {[Paper](https://nlp.cs.nyu.edu/sekine/papers/li07.pdf)}
6. No Noun Phrase Left Behind: Detecting and Typing Unlinkable Entities [EMNLP-CoNLL 2012]{[Paper](https://aclweb.org/anthology/D12-1082)}


## Topic 3: Relation Extraction 
__Tutorial:__
1. A SURVEY ON RELATION EXTRACTION (CMU) {[Slides](http://www.cs.cmu.edu/~nbach/papers/A-survey-on-Relation-Extraction-Slides.pdf)}
2. Relation Extraction: CSE 517: Natural Language Processing {[Slides](https://courses.cs.washington.edu/courses/cse517/13wi/slides/cse517wi13-RelationExtraction.pdf)}
3. Relation Extraction II: CSE 517: Natural Language Processing {[Slides](https://courses.cs.washington.edu/courses/cse517/13wi/slides/cse517wi13-RelationExtractionII.pdf)}

__Papers:__
1. CoType: Joint Extraction of Typed Entities and Relations with Knowledge Bases [CoType, WWW2017]
https://blog.csdn.net/hqc888688/article/details/73559365
2. [g]Knowledge-Based Weak Supervision for Information Extraction of Overlapping Relations {[Code](http://aiweb.cs.washington.edu/ai/raphaelh/mr/)}{[Slides](https://www.slideserve.com/anila/knowledge-based-weak-supervision-for-information-extraction-of-overlapping-relations)} 
> * Recently, researchers have developed multi- instance learning algorithms to combat the noisy training data that can come from heuristic labeling, but their models assume relations are disjoint . for example they cannot extract the pair Founded(Jobs, Apple) and CEO-of(Jobs, Apple). This paper presents a novel approach for multi-instance learning with overlapping relations that combines a sentence-level extraction model with a simple, corpus-level component for aggregating the individual facts. 
3. [g]Modeling missing data in distant supervision for information extraction [ACL2013] missing data problem(?)
4. Neural Relation Extraction with Selective Attention over Instances [ACL 2016] {[Paper](http://www.aclweb.org/anthology/P16-1200)}{[Code](https://github.com/thunlp/OpenNRE)}{[Blog](https://zhuanlan.zhihu.com/p/22666876)}
> * Fix the problem of distant supervised relation extraction
> * Employs CNN to embed the semantics of sentences, then builds sentence-level attention over multi- ple instances, which is expected to dynamically reduce the weights of those noisy instances (major contribution). Notes in group meeting.
5. Multi-instance Multi-label Learning for Relation Extraction [EMMLP-CoNLL 2012]{[Paper](https://www.aclweb.org/anthology/D12-1042)}

## Topic 4: Entity Linking
__Notes:__
1. Candiate Entity Ranking: https://www.jianshu.com/p/90e2c7a5c9f5
2. http://nlpprogress.com/english/entity_linking.html

__Papers:__
1. Entity Linking wuth a Knowledge Base: Issues, Techniques, and Solutions (Survey)
2. Robust Disambihguation of Named Entities in Text [EMNLP 2011]
3. Liege: Link Entities in Web Lists with Knowledge Base [KDD 2012]
4. Entity Lnking for Tweets [ACL 2013]
5. Collective Annotation of Wikipedia Entities in Webb Text [KDD 2009]
6. Local and Global Algorithms for Disambiguation to Wikipedia [ACL 2011]


## Topic 5: Open Information Extraction 
__Sides, Tutorials and Surveys__
1. Brief Introduction and Review of Open Information Extraction System {[Slides](https://ece.umd.edu/~smiran/OpenIE.pdf)}
2. A Survey on Open Information Extraction {[Paper](http://aclweb.org/anthology/C18-1326)}
3. Open Information Extraction on Scientific Text: An Evaluation {[Paper](http://aclweb.org/anthology/C18-1289)}
4. https://github.com/gkiril/oie-resources

__OpenIE Tools__
1. Open Information Extraction from the Web [TextRunner, IJCAI 2007]
> * Incoherent Extractions 
> * Uninformative Extractions
2. MinIE: Minimizing Facts in Open Information Extraction [MinIE, EMNLP 2017] [Code (java)](https://github.com/rgemulla/minie) 
> * Represent information about polarity, modality, attribution and quantities with semantic annotations (instead of actual extraction)
> * idetify and remove parts that are considered over specific
3. Facts that Matter [SALIE, EMNLP 2018] {[Code](https://github.com/mponza/SalIE)}
> * Extract salient facts, which fulfill two requirements: (1) relevance and (2) diversity
4. Identifying Relations for Open Information Extraction [ReVerb, EMNLP 2011] {[Paper](http://www.aclweb.org/anthology/D11-1142)}{[Code](https://github.com/knowitall/reverb)}{[Homepage](http://reverb.cs.washington.edu/)}                  
> * Use syntactic constraints to specify relation phrases (3 simple patterns). Find longest phrase matching one of the syntactic constraints. 
> * Find nearest noun-phrases to the left and right of relation phrase. - Not a relative pronoun or WHO-adverb or an existential there.
> * To avoid "overspecified" relation phrases, a relation phrase must have many distinct args in a large corpus
5. ClausIE: Clause-Based Open Information Extraction [ClausIE, WWW 2013] {[Paper](http://resources.mpi-inf.mpg.de/d5/clausie/clausie-www13.pdf)}{[Code (Python)](https://github.com/AnthonyMRios/pyclausie)}{[Code (Java)](https://github.com/IsaacChanghau/ClausIE)}
> * Map the dependency relations of an input senetnce to clause constituents.
> * A set of coherent clauses presenting a simple linguistic structure is derived from the input

__OpenIE Triple Clustering__
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
9. Relation Extraction with Matrix Fatorization and Universal Schemes [NAACL-HLT 2013] {[Paper](http://www.aclweb.org/anthology/N13-1008)} 
> * Close to relation clustering
> * Create a universal scheme by unioning surface form predicates from Open IE and relations in the schemas of pre-existing databbases.

__Relation Phrases Clustering (finding synonymous phrases and hypernyms)__
1. HARPY: Hypernyms and Alignment of Relational Paraphrases [HAPPY, COLING 2014] {[Paper](http://www.dit.unitn.it/~p2p/RelatedWork/Matching/harpy_COLING14.pdf)}{[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)}
2. POLY: Mining Relational Paraphrases from Multilingual Sentences [POLY, EMNLP 2016] {[Paper](https://www.aclweb.org/anthology/D16-1236)}{[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)}
> * Make use of another language
3. RELLY: Inferring Hypernym Relationships Between Relational Phrases [REELY, EMNLP 2015] {[Paper](https://www.aclweb.org/anthology/D15-1113)}{[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)}
4. PATTY: A Taxonomy of Relational Patterns with Semantic Types [PATTY, EMNLP 2012] {[Paper](https://www.aclweb.org/anthology/D12-1104)}{[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)}
5. Discovering and Exploring Relations on the Web [PATTY demo, VLDB 2012] {[Paper](http://vldb.org/pvldb/vol5/p1982_ndapandulanakashole_vldb2012.pdf)}
6. [g]Ensemble Semantics for Large-Scale Unsupervised Relation Extraction [WEBRE, EMNLP-CoNELL 2012] relation
7. [g]Relation Schema Induction using Tensor Factorization with Side Information [SICTF, EMNLP 2016] relation schema induction (for building domain-specific kb from unstructured text) Code: https://github.com/malllabiisc/sictf
8. [g]Constrained Information-Theoretic Tripartite Graph Clustering to Identify Semantically Similar Relations [IJCAI 2015]

__Relation Linking__
1. Old is Gold: Linguistic Driven Approach for Entity and Relation Linking of Short Text [FALCON, NAACL 2019] {[Paper](https://www.researchgate.net/profile/Ahmad_Sakor/publication/332104600_Old_is_Gold_Linguistic_Driven_Approach_for_Entity_and_Relation_Linking_of_Short_Text/links/5ca0a7ac299bf11169526b5f/Old-is-Gold-Linguistic-Driven-Approach-for-Entity-and-Relation-Linking-of-Short-Text.pdf)} {[Code](https://github.com/AhmadSakor/falcon)}{[Demo](https://labs.tib.eu/falcon/)}{[Notes](https://github.com/BrambleXu/knowledge-graph-learning/issues/211)}
2. EARL: Joint Entity and Relation Linking for Question Answering [EARL, ISWC 2018] {[Paper](https://arxiv.org/abs/1801.03825)} {[Code](https://github.com/AskNowQA/EARL)}

__Others__
1. Intergring Local Context and Global Cohesiveness for Open Information Extraction [ReMine, WSDM 2019]
> * Solving a joint optimization problem to unify (1) segmenting entity/relation phrases in individual sentences based on local context; and (2) measuring the quality of tuples extracted from individual sentences with a translating-based objective.

## Topic 6: Graph Embedding, Learning and Reasoning
1. DeepWalk: Online Learning of Social Representations [DeepWalk, KDD 2014] [Code] (https://github.com/phanein/deepwalk Slides: https://www.slideshare.net/bperz/14-kdddeep-walk-2)
> * Use a sentence embedding model
2. [g]DeepPath: A Reinforcement Learning Method for Knowledge Graph Reasoning [DeepPath, EMNLP 2017] [Code](https://github.com/xwhan/DeepPath Notes: https://zhuanlan.zhihu.com/p/33536026)
3. [g]Know-Evolve: Deep Temporal Reasoning for Dynamic Knowledge Graphs [Know-Evolve, ICML 2017]{[Paper](http://proceedings.mlr.press/v70/trivedi17a/trivedi17a.pdf)}{[Code (C++)](https://github.com/rstriv/Know-Evolve)}
4. [g]Reading and Reasoning with Knowledge Graphs [PhD Thesis of Matthew Gardner] {[Thesis](http://www.cs.cmu.edu/~mg1/thesis.pdf)}
> * Reasoning, Relation Extraction, Modeling Lexical Semantics 
5. EventKG: A Multilingual Event-Centric Temporal Knowledge Graph
> * Has time and location info
> * A system that integrates knowledge from different existing KBs
6. Knowledge Graph Embedding: A Survey of Approaches and Applications {[Paper](https://persagen.com/files/misc/Wang2017Knowledge.pdf)}
7. Multilingual Knowledge Graph Embedding for Cross-lingual Knowledge Alignment. {[Slides](http://yellowstone.cs.ucla.edu/~muhao/slides/mtranse_slides_short.pdf)}


## Topic 7: Dynamic Embedding
1. [g]Dynamic Word Embeddings {[Paper](https://arxiv.org/pdf/1702.08359.pdf)}
2. [g]DYREP: LEARNING REPRESENTATIONS OVER DYNAMIC GRAPHS [ICLR 2019] {[Paper](https://openreview.net/pdf?id=HyePrhR5KX)}
3. [g]Know-Evolve: Deep Temporal Reasoning for Dynamic Knowledge Graphs [Know-Evolve, ICML 2017]{[Paper](http://proceedings.mlr.press/v70/trivedi17a/trivedi17a.pdf)}{[Code (C++)](https://github.com/rstriv/Know-Evolve)}
4. [g] Continuous-Time Dynamic Network Embeddings [WWW 2018] {[Paper](http://ryanrossi.com/pubs/nguyen-et-al-WWW18-BigNet.pdf)}


## Topic 8: Knowledge Base Refinement
__Survey:__
1. Knowledge Graph Refinement:A Survey of Approaches and Evaluation Methods

__Knowledge Base Completion:__
1. Knowledge base completion via search-based question answering [WWW 2014]{[Paper](https://dl.acm.org/citation.cfm?id=2568032)}
2. Knowledge base completion via coupled path ranking [ACL 2016]{[Paper](https://www.aclweb.org/anthology/P16-1124)}

__Knowledge Base Population:__
1. https://nlp.stanford.edu/projects/kbp/
 
## Others
1. A Fresh Look on Knowledge Bases Distilling Named [CIKM 2014] 
> * Event KB. Each news article is regarded as a event. Build the semantic similarity relations and the tmporal relations between evernts.
2. CERES: Distantly Supervised Relation Extractionfrom the Semi-Structured Web [CERES, VLDB 2018]
3. When Open Information Extraction Meets the Semi-Structured Web [OpenCERES, NAACL 2019]
4. How to Keep a Knowledge Base Synchronized with Its Encyclopedia Source [IJCAI 2017] {[Notes](https://zhuanlan.zhihu.com/p/30803950)}


Tutorials and Notes from Talented People
=====
## About Knowledge Graphs
1. https://kgtutorial.github.io An introduction to knowledge graph and knowledge extraction from unstructured text.
2. https://github.com/impillar/knowledge_graph/blob/master/README.md 
3. https://github.com/BrambleXu/knowledge-graph-learning
4. https://github.com/Pelhans/Z_knowledge_graph
5. https://zhuanlan.zhihu.com/p/44904796
6. Information Extraction by Niranjan Balasubramanian {Slides in my Mac}

## Others
1. Probabilistic Graphical Models: Lagrangian Relaxation Algorithms for Natural Language Processing {[Slides](http://people.csail.mit.edu/dsontag/courses/pgm12/slides/lecture3.pdf)}
2. Introduction to Conditional Random Fields {[Blog](http://blog.echen.me/2012/01/03/introduction-to-conditional-random-fields/)}
3. Network Community Detection: A Review and Visual Survey {[Paper](https://arxiv.org/pdf/1708.00977.pdf)}
> * Section 2.3. Community Detection Techniques 
4. Fast unfolding of communities in large networks {[Paper](https://arxiv.org/pdf/0803.0476.pdf)}
> * A discussion of the Louvain method: https://www.quora.com/Is-there-a-simple-explanation-of-the-Louvain-Method-of-community-detection, wiki of the Louvein Modularity: https://en.wikipedia.org/wiki/Louvain_Modularity
> * How do they design the function Q: Finding and evaluating community structure in networks {[Paper](https://arxiv.org/abs/cond-mat/0308217)}
5. A compendium of NP optimization problems http://www.nada.kth.se/~viggo/wwwcompendium/
6. Notes about LSH: https://blog.csdn.net/yc461515457/article/details/48845775
7. Survey about Min Hash Sketch: http://www.cohenwang.com/edith/Surveys/minhash.pdf
8. MinHash Tutorial with Python Code: https://mccormickml.com/2015/06/12/minhash-tutorial-with-python-code/  https://github.com/chrisjmccormick/MinHash
9. GNN: https://github.com/thunlp/GNNPapers


Useful Tools
====
## Entity Linking
1. Wikidata Integrator
2. Stanford KBP

## Named Entity Recognition
1. spaCy {[Link](https://spacy.io/api/annotation#section-named-entities https://towardsdatascience.com/named-entity-recognition-with-nltk-and-spacy-8c4a7d88e7da)}
2. NLTK
3. DBpedia Spotlight {[Link](https://www.dbpedia-spotlight.org/)}

## Pronominal Coreference Resolution
1. BOOKNLP https://github.com/dbamman/book-nlp (a natural language processing pipeline that scales to books and other long documents (in English))

## Others
1. From Freebase to Wikidata: The Great Migration {[Paper and useful links](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44818.pdf)} 
2. SPASQL tutorial {[Link](https://www.w3.org/2009/Talks/0615-qbe/)}
3. Installing and running ElasticSearch {[Link](https://www.elastic.co/guide/en/elasticsearch/reference/current/targz.html)}
