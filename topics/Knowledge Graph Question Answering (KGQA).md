## Knowledge Graph Question Answering (KGQA)
Note: This task is highly related with [Entity Linking and Disambiguation](https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/topics/Entity%20Linking%20and%20Entity%20Disambiguation.md) as well as [Relation Linking and Disambiguation](https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/topics/Relation%20Linking%20and%20Relation%20Disambiguation.md).

### 📝 Survey and Summary
1. Core techniques of question answering systems over knowledge bases: a survey (Knowledge and Information Systems 2017) [[Paper](https://link.springer.com/article/10.1007/s10115-017-1100-y)]
2. A Survey on Complex Question Answering over Knowledge Base: Recent Advances and Challenges (2020) [[Paper](https://arxiv.org/pdf/2007.13069.pdf)]
3. Question Answering Summary (not limited to KBQA) [[GitHub](https://github.com/sebastianruder/NLP-progress/blob/master/english/question_answering.md)]
4. Introduction to Neural Network based Approaches for Question Answering over Knowledge Graphs (2019) [[Paper](https://arxiv.org/pdf/1907.09361.pdf)]
5. Awesome KGQA [[GitHub](https://github.com/BshoterJ/awesome-kgqa)]
6. What is in the KGQA Benchmark Datasets? Survey on Challenges in Datasets for Question Answering on Knowledge Graphs (Journal on Data Semantics, 2021)[[Paper](https://link.springer.com/content/pdf/10.1007/s13740-021-00128-9.pdf)]
7. Complex Knowledge Base Question Answering: A Survey [[Paper](https://arxiv.org/pdf/2108.06688v1.pdf)]
8. Knowledge Graphs & LLMs: Multi-Hop Question Answering [[Neo4j Developer Blog](https://neo4j.com/developer-blog/knowledge-graphs-llms-multi-hop-question-answering/)] [[Another Similar Discussion](https://www.linkedin.com/pulse/multi-hop-question-answering-llms-knowledge-graphs-wisecube/)]

### 📝 Papers
__General KGQA__
1. Question Answering Over Knowledge Graphs: Question Understanding Via Template Decomposition (VLDB 2018) [[Paper](http://www.vldb.org/pvldb/vol11/p1373-zheng.pdf)]🌟
2. KBQA: Learning Question Answering over QA Corpora and Knowledge Bases
3. SPARQA: Skeleton-based Semantic Parsing for Complex Questions over Knowledge Bases [[Paper](https://arxiv.org/pdf/2003.13956.pdf)]
4. Improving Multi-hop Question Answering over Knowledge Graphs using Knowledge Base Embeddings (ACL 2020) [[Paper](https://www.aclweb.org/anthology/2020.acl-main.412.pdf)]
> Efficiency issue.
5. AskNow: A Framework for Natural Language Query Formalization in SPARQL (ESWC 2016)
6. Answering Natural Language Questions by Subgraph Matching over Knowledge Graphs (TKDE 2018) [[Paper](https://ieeexplore.ieee.org/document/8085196)]
7. Natural language question answering over RDF: a graph data driven approach (SIGMOD 2014) 🌟
8. Complex Factoid Question Answering with a Free-Text Knowledge Graph (WWW 2020)
9. Automated template generation for question answering over knowledge graphs （WWW 2017） [[Paper](https://dl.acm.org/doi/pdf/10.1145/3038912.3052583)]
10. Never-Ending Learning for Open-Domain Question Answering over Knowledge Bases (WWW 2018) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3178876.3186004)]
11. Learning to Retrieve Reasoning Paths over Wikipedia Graph for Question Answering (ICLR 2020)
12. An Interpretable Reasoning Network for Multi-Relation Question Answering (COLING 2018)
13. Pattern-revising Enhanced Simple Question Answering over Knowledge Bases (COLING 2018)
14. TEQUILA: Temporal Question Answering over Knowledge Bases (CIKM 2018)
15. FreebaseQA: A New Factoid QA Data Set Matching Trivia-Style Question-Answer Pairs with Freebase (NAACL 2019) [[Paper](https://www.aclweb.org/anthology/N19-1028.pdf)]
16. Knowledge Graph Embedding Based Question Answering (WSDM 2019) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3289600.3290956)] [[Code](https://github.com/xhuang31/KEQA_WSDM19)]
17. Graph-Based Reasoning over Heterogeneous External Knowledge for Commonsense Question Answering (AAAI 2020) [[Paper](https://arxiv.org/pdf/1909.05311.pdf)]
18. Open Question Answering Over Curated and Extracted Knowledge Bases (KDD 2014) [[Paper](https://dl.acm.org/doi/pdf/10.1145/2623330.2623677)]
19. RocketQA: An Optimized Training Approach to Dense Passage Retrieval for Open-Domain Question Answering (2021) [[Paper](https://arxiv.org/pdf/2010.08191.pdf)]
20. Natural language question/answering let users talk with the knowledge graph (CIKM 2017)
21. Asking Clarification Questions in Knowledge-Based Question Answering (EMNLP 2019)
22. What's Missing: A Knowledge Gap Guided Approach for Multi-hop Question Answering (EMNLP 2019)
23. KagNet: Learning to Answer Commonsense Questions with Knowledge-Aware Graph Networks (EMNLP 2019)
24. Message Passing for Complex Question Answering over Knowledge Graphs (CIKM 2019) [[Paper](https://arxiv.org/pdf/1908.06917.pdf)]
25. Keyword Search on RDF Graphs — A Query Graph Assembly Approach (CIKM 2017) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3132847.3132957)] 🌟
26. Semantic Guided and Response Times Bounded Top-k Similarity Search over Knowledge Graphs (ICDE 2020) [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9101747&tag=1)] 🌟
27. Beyond I.I.D.: Three Levels of Generalization for Question Answering on Knowledge Bases (WWW 2021) [[Paper](https://arxiv.org/pdf/2011.07743.pdf)]
28. Query Graph Generation for Answering Multi-hop Complex Questions from Knowledge Bases (ACL 2020) [[Paper](https://www.aclweb.org/anthology/2020.acl-main.91.pdf)] [[Code](https://github.com/lanyunshi/Multi-hopComplexKBQA)]
29. CBench: Towards Better Evaluation of Question Answering Over Knowledge Graphs [[Paper](https://vldb.org/pvldb/vol14/p1325-orogat.pdf)] (VLDB 2021) 🌟
30. SAKE: Spatial Question Answering over Knowledge Graph Based on Embedding Techniques (ICDE 2021) 🌟

__Multiple Hop QA__
1. Scalable Multi-Hop Relational Reasoning for Knowledge-Aware Question Answering (EMNLP 2020) [[Video](https://virtual.2020.emnlp.org/paper_main.1648.html)]
2. QA-GNN: Reasoning with Language Models and Knowledge Graphs for Question Answering (Jure's group, NAACL-HLT 2021) [[Paper](https://arxiv.org/pdf/2104.06378.pdf)]
3. Cognitive Graph for Multi-Hop Reading Comprehension at Scale (ACL 2019) [[Paper](https://arxiv.org/abs/1905.05460)] [[Code](https://github.com/THUDM/CogQA)]
> * Note: Cognitive Graph is not directly equal to Knowledge Graph. You can view CG as a (dynamic, partial, local) KG generated instantly from the query.
4. Complex Question Answering on knowledge graphs using machine translation and multi-task learning (EACL 2021) [[Paper](https://aclanthology.org/2021.eacl-main.300/)]
5. Improving Multi-hop Question Answering over Knowledge Graphs using Knowledge Base Embeddings (ACL 2020) [[Paper](https://malllabiisc.github.io/publications/papers/final_embedkgqa.pdf)] More than 300 stars in Github in Dec 2023!

__Multiple-Options QA__
1. RiddleSense: Reasoning about Riddle Questions Featuring Linguistic Creativity and Commonsense Knowledge (ACL 2021) [[Paper](https://aclanthology.org/2021.findings-acl.131.pdf)]
2. QA-GNN: Reasoning with Language Models and Knowledge Graphs for Question Answering (Jure's group, NAACL-HLT 2021) [[Paper](https://arxiv.org/pdf/2104.06378.pdf)]

__Multiligual QA__
1. Improving Zero-Shot Cross-lingual Transfer for Multilingual Question Answering over Knowledge Graph (ACL 2021) [[Paper](https://aclanthology.org/2021.naacl-main.465/)]

__LLM for KGQA/KG for QA based on LLM__ 🔥
1. Leveraging LLMs in Scholarly Knowledge Graph Question Answering (Arxiv, Nov 2023) [[Paper](https://arxiv.org/abs/2311.09841)]
2. Answering Questions Over Knowledge Graphs Using Logic Programming Along with Language Models (submitted to ICLR 2023 but not revised) [[Paper](https://openreview.net/forum?id=D2lo4toTUTo)]
3. Retrieve-Rewrite-Answer: A KG-to-Text Enhanced LLMs Framework for Knowledge Graph Question Answering (Arxiv, Sep 2023) [[Paper](https://arxiv.org/abs/2309.11206)]
4. Language Models as Controlled Natural Language Semantic Parsers for Knowledge Graph Question Answering (from Amazon Science, 2023) [[Paper](https://assets.amazon.science/10/14/9c09d8964b4b8b6219286d8fc05e/language-models-as-controlled-natural-language-semantic-parsers-for-knowledge-graph-question-answering.pdf)]
5. Is GPT fit for KGQA? – Preliminary Results (CEUR Workshop 2023) [[Paper](https://ceur-ws.org/Vol-3447/Text2KG_Paper_11.pdf)]
> * Only GPT3 and GPT3.5 are used, so the experiemnts prove that there is limitation.
6. Bring Your Own KG: Self-Supervised Program Synthesis for Zero-shot KGQA (Amazon and UMass, Nov 2023) [[Paper](https://arxiv.org/pdf/2311.07850v1.pdf)]
> * In BYOKG, exploration leverages an LLM-backed symbolic agent that generates a diverse set of queryprogram exemplars, which are then used to ground a retrieval-augmented reasoning procedure to predict programs for arbitrary questions.
7. A Benchmark to Understand the Role of Knowledge Graphs on Large Language Model's Accuracy for Question Answering on Enterprise SQL Databases (Arxiv, Nov 2023) [[Paper](https://arxiv.org/abs/2311.07509)]
8. Knowledge-augmented language model prompting for zero-shot knowledge graph question answering (ACL 2023, KAIST + MBZUAI + Amazon) [[Paper](https://www.amazon.science/publications/knowledge-augmented-language-model-prompting-for-zero-shot-knowledge-graph-question-answering)]
9. Empowering Language Models with Knowledge Graph Reasoning for Open-Domain Question Answering (EMNLP 2022) [[Paper](https://aclanthology.org/2022.emnlp-main.650.pdf)]
10. KnowledgeNavigator: Leveraging Large Language Models for Enhanced Reasoning over Knowledge Graph (Arxiv, Dec 2023) [[Paper](https://arxiv.org/pdf/2312.15880.pdf)]
> * The baselines also include __StructGPT__ (A general framework for large language model to reason over structured data, Arxiv 2023) and __TOG__ (Think-on-graph: Deep and responsible reasoning of large language model with knowledge graph, Arxiv 2023)
11. Pretrained transformers for simple question answering over knowledge graphs (Web–ISWC 2019)
> * The first work to utilize LLMs as classifiers for relation prediction.
12. An empirical study of pre-trained language models in simple knowledge graph question answering (Arxiv 2023)
> * It introduce two LLM-based KGQA frameworks that adopt LLMs to detect mentioned entities and relations. Then, they query the answer in KGs using the extracted entity-relation pairs.
13. __QA-GNN__: QAGNN: Reasoning with language models and knowledge graphs for question answering (ACL 2021)
> * It uses LLMs to encode the question and candidate answer pairs, which are adopted to estimate the importance of relative KG entities. The entities are retrieved to form a subgraph, where an answer reasoning is conducted by a GNN.
14. A bert-based approach with relationaware attention for knowledge base question answering (IJCNN 2021)
> * It use LLMs to calculate the similarities between relations and questions to retrieve related facts.
15. Subgraph retrieval enhanced model for multi-hop knowledge base question answering (ACL 2022)
> * a LLM-based path retriever to retrieve question-related relations hop-byhop and construct several paths.
16. Can ChatGPT Replace Traditional KBQA Models? An In-Depth Analysis of the Question Answering Performance of the GPT LLM Family (ISWC 2023) [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-47240-4_19)]
17. ReasoningLM: Enabling Structural Subgraph Reasoning in Pre-trained Language Models for Question Answering over Knowledge Graph (ACL 2023) [[Paper](https://aclanthology.org/2023.emnlp-main.228/)]
18. Language Models as Controlled Natural Language Semantic Parsers for Knowledge Graph Question Answering (ECAI 2023) [[Paper](https://inria.hal.science/hal-04269089/)]
19. LLM-Based SPARQL Generation with Selected Schema from Large Scale Knowledge Base (CCKS2023 CKBQA competition, F1 score is 75.63% on CKBQA dataset) [[Paper](https://link.springer.com/chapter/10.1007/978-981-99-7224-1_24)]
20. Improving Subgraph Extraction Algorithms for One-Shot SPARQL Query Generation with Large Language Models (ISWC 2023) [[Paper](https://ceur-ws.org/Vol-3592/paper6.pdf)]
21. A Structure and Content Prompt-based Method for Knowledge Graph Question Answering over Scholarly Data  (ISWC 2023) [[Paper](https://ceur-ws.org/Vol-3592/paper3.pdf)]
22. Bring Your Own KG: Self-Supervised Program Synthesis for Zero-Shot KGQA (Arxiv 2023) [[Paper](https://arxiv.org/abs/2311.07850)]
23. Check for updates LLM-Based SPARQL Generation with Selected Schema from Large Scale Knowledge Base (Springer Nature Singapore 2023)

### 📊 Leaderboard and Benchmarks
1. __QALD-9__： The 9th challenge on question answering over linked data (QALD-9) (invited paper) (CEUR Workshop 2018)
2. __Lc-quad 2.0__: A large dataset for complex question answering over wikidata and dbpedia (ISWC 2019)
3. Knowledge Graph Question Answering Leaderboard: A Community Resource to Prevent a Replication Crisis (LREC 2022) [[Paper](https://aclanthology.org/2022.lrec-1.321/)] [[Link](https://kgqa.github.io/leaderboard/)]
4. __MetaQA__: Variational reasoning for question answering with knowledge graph (AAAI 2018)
> * A large scale multi-hop KGQA dataset with more than 400k questions in the movie domain. It has 1-hop, 2-hop, and 3-hop questions.
> * It also provides a KG with 135k triples, 43k entities, and nine relations.
6. __WebQuestionsSP__: The value of semantic parse labeling for knowledge base question answering (ACL 2016)
> * a smaller QA dataset with 4,737 questions. The questions in this dataset are 1-hop and 2-hop questions and are answerable through Freebase KG.
7. **ComplexWebQuestions**: The web as a knowledge-base for answering complex questions (ACL 2018)
8. **GraphQ**: On generating characteristic-rich question sets for QA evaluation (EMNLP 2016)
7. __MKQA__: a linguistically diverse benchmark for multilingual open domain question answering (ACL 2021)
8. __GrailQA__: Beyond IID: three levels of generalization for question answering on knowledge bases (WWW 2021)
9. __KQA Pro__: a dataset with explicit compositional programs for complex question answering over knowledge base (ACL 2022)

### 🧐 Others
__Related Readings__
1. Unsupervised Question Decomposition for Question Answering (EMNLP 2020) [[Paper](https://www.aclweb.org/anthology/2020.emnlp-main.713.pdf)] [[Code](https://github.com/facebookresearch/UnsupervisedDecomposition)]
2. The Web as a Knowledge-base for Answering Complex Questions (NAACL-HLT 2018) [[Paper](https://www.aclweb.org/anthology/N18-1059.pdf)]
3. Scalable Join Processing on Very Large RDF Graphs (SIGMOD 2009) [[Paper](https://sites.fas.harvard.edu/~cs265/papers/neumann-2009.pdf)] 🌟

__Some thoughts__
* Consider Combine embedding and subgraph matching for KGQA?
