## Open Information Extraction

### Sides, Tutorials and Surveys
1. Brief Introduction and Review of Open Information Extraction System [[Slides](https://ece.umd.edu/~smiran/OpenIE.pdf)]
2. A Survey on Open Information Extraction [[Paper](http://aclweb.org/anthology/C18-1326)]
3. Open Information Extraction on Scientific Text: An Evaluation [[Paper](http://aclweb.org/anthology/C18-1289)]
4. Open Information Extraction (OIE) Resources Summary [[Paper](https://github.com/gkiril/oie-resources)]

### OpenIE Tools
1. Open Information Extraction from the Web [TextRunner, IJCAI 2007]
> * Incoherent Extractions 
> * Uninformative Extractions
2. MinIE: Minimizing Facts in Open Information Extraction [MinIE, EMNLP 2017] [[Code (java)](https://github.com/rgemulla/minie)] [[Code (python)](https://github.com/mmxgn/miniepy)]
> * Represent information about polarity, modality, attribution and quantities with semantic annotations (instead of actual extraction)
> * identify and remove parts that are considered over specific
3. Facts that Matter [SALIE, EMNLP 2018] [[Code](https://github.com/mponza/SalIE)]
> * Extract salient facts, which fulfil two requirements: (1) relevance and (2) diversity
4. Identifying Relations for Open Information Extraction [ReVerb, EMNLP 2011] [[Paper](http://www.aclweb.org/anthology/D11-1142)][[Code](https://github.com/knowitall/reverb)][[Homepage](http://reverb.cs.washington.edu/)]               
> * Use syntactic constraints to specify relation phrases (3 simple patterns). Find longest phrase matching one of the syntactic constraints. 
> * Find nearest noun-phrases to the left and right of relation phrase. - Not a relative pronoun or WHO-adverb or an existential there.
> * To avoid "over-specified" relation phrases, a relation phrase must have many distinct args in a large corpus
5. ClausIE: Clause-Based Open Information Extraction [ClausIE, WWW 2013] [[Paper](http://resources.mpi-inf.mpg.de/d5/clausie/clausie-www13.pdf)][[Code (Python)](https://github.com/AnthonyMRios/pyclausie)][[Code (Java)](https://github.com/IsaacChanghau/ClausIE)]
> * Map the dependency relations of an input sentence to clause constituents.
> * A set of coherent clauses presenting a simple linguistic structure is derived from the input

__Open Relation Extraction__
1. LOREM: Language-consistent Open Relation Extraction from Unstructured Text (WWW 2020)

### Canonicalization of Open Knowledge Bases, OpenIE Triple Clustering
__General Papers__
1. Query-Driven On-The-Fly Knowledge Base Construction [QKBfly, VLDB2017] relation 🌟 
2. CESI: Canonicalizing Open Knowledge Bases using Embeddings and Side Information [CESI, WWW2018] [Code](https://github.com/malllabiisc/cesi) triple
3. Canonicalizing Open Knowledge Bases [CIKM 2014] triple 🌟 
4. Towards Practical Open Knowledge Base Canonicalization [FAC, CIKM 2018] triple 🌟
5. Identifying Relations for Open Information Extraction [ReVerb, EMNLP 2011]  [[Paper](http://www.aclweb.org/anthology/D11-1142)][[Code](https://github.com/knowitall/reverb)][[Homepage](http://reverb.cs.washington.edu/)] relation
> * Mophological Normalization
6. Open Information Extraction to KBP Relations in 3 Hours [TAC. 2013] [[Paper](https://pdfs.semanticscholar.org/d431/81fa9af5440360d4055e1ce7ddaaa6e82d77.pdf)]
> * Main idea: relation phrases mapping to KB otology
> * Manually define a set of rules for each relation, to conduct the mapping
> * The motivation and error analysis are well written
7. ClusType: Effective Entity Recognition and Typing by Relation Phrase-Based Clustering [ClusType, KDD2015] 🌟
> * Relation Clustering: Two relation phrases tend to have similar cluster membershipd, if they have similar (1) strings; (2) context words; and (3) left and right argument type indicators
8. Unsupervised Methods for Determining Object and Relation Synonyms on the Web [Resolover, JAIR 2009] relation
9. Relation Extraction with Matrix Fatorization and Universal Schemes [NAACL-HLT 2013] [[Paper](http://www.aclweb.org/anthology/N13-1008)]
> * Close to relation clustering
> * Create a universal scheme by unioning surface form predicates from Open IE and relations in the schemas of pre-existing databases
10. Canonicalization of Open Knowledge Bases with Side Information from the Source Text [[PDF](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8731346)] (ICDE 2018) 🌟
11. Canonicalizing Open Knowledge Bases with Multi-Layered Meta-Graph Neural Network [[Paper](https://arxiv.org/pdf/2006.09610.pdf)]

__Relation Phrases Clustering (finding synonymous phrases and hypernyms)__
1. HARPY: Hypernyms and Alignment of Relational Paraphrases [HAPPY, COLING 2014] [[Paper](http://www.dit.unitn.it/~p2p/RelatedWork/Matching/harpy_COLING14.pdf)}{[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)]
2. POLY: Mining Relational Paraphrases from Multilingual Sentences [POLY, EMNLP 2016] [[Paper](https://www.aclweb.org/anthology/D16-1236)][[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)]
> * Make use of another language
3. RELLY: Inferring Hypernym Relationships Between Relational Phrases [REELY, EMNLP 2015] [[Paper](https://www.aclweb.org/anthology/D15-1113)}[[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)]
4. PATTY: A Taxonomy of Relational Patterns with Semantic Types [PATTY, EMNLP 2012] [[Paper](https://www.aclweb.org/anthology/D12-1104)][[Data](https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/patty/)]
5. Discovering and Exploring Relations on the Web [PATTY demo, VLDB 2012] [[Paper](http://vldb.org/pvldb/vol5/p1982_ndapandulanakashole_vldb2012.pdf)] 🌟
6. Ensemble Semantics for Large-Scale Unsupervised Relation Extraction [WEBRE, EMNLP-CoNELL 2012] relation
7. Relation Schema Induction using Tensor Factorization with Side Information [SICTF, EMNLP 2016] relation schema induction (for building domain-specific kb from unstructured text) Code: https://github.com/malllabiisc/sictf
8. Constrained Information-Theoretic Tripartite Graph Clustering to Identify Semantically Similar Relations [IJCAI 2015]

__Related Works__
1. Query-Efficient Correlation Clustering (WWW 2020)


### Other Interesting Works about Open IE
1. Intergring Local Context and Global Cohesiveness for Open Information Extraction [ReMine, WSDM 2019]
> * Solving a joint optimization problem to unify (1) segmenting entity/relation phrases in individual sentences based on local context; and (2) measuring the quality of tuples extracted from individual sentences with a translating-based objective.
2. Extracting Knowledge from Web Text with Monte Carlo Tree Search (WWW 2020, short paper)
