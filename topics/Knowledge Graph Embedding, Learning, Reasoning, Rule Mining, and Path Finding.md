## Knowledge Graph Embedding, Learning, Reasoning, Rule Mining, and Path Finding

__Surveys and Experimental Studies__
1. Knowledge graph embedding: A survey of approaches and applications (TKDE 2017)🌟
2. Knowledge representation learning: A quantitative review (2018) [[Code in this paper](https://github.com/thunlp/OpenKE)]
3. A Comprehensive Survey of Knowledge Graph Embeddings with Literals: Techniques and Applications (ESWC 2019) [[Paper](http://ceur-ws.org/Vol-2377/paper_4.pdf)]
4. Knowledge Graph Embedding for Link Prediction: A Comparative Analysis [[Paper](https://arxiv.org/pdf/2002.00819.pdf)]
5. Realistic Re-evaluation of Knowledge Graph Completion Methods: An Experimental Study [[Paper](https://doi.org/10.1145/3318464.3380599)] (SIGMOD 2020) 🌟

__Summary__
1. Papers, Surveys, and Datasets on Knowledge Graph Embedding (KGE) [[GitHub](https://github.com/xinguoxia/KGE)]
2. Knowledge Graph Reasoning: Recent Advances (Slides) [[Link](https://sites.cs.ucsb.edu/~william/papers/Part3_KB_Reasoning.pdf)]
3. KG Embedding Approaches [[Link](https://gist.github.com/mommi84/07f7c044fa18aaaa7b5133230207d8d4)]

__General KG Embedding and KG Representation__
1. DeepWalk: Online Learning of Social Representations (DeepWalk, KDD 2014) [Code] (https://github.com/phanein/deepwalk Slides: https://www.slideshare.net/bperz/14-kdddeep-walk-2)
> * Use a sentence embedding model
2. EventKG: A Multilingual Event-Centric Temporal Knowledge Graph
> * Has time and location info
> * A system that integrates knowledge from different existing KBs
3. Multilingual Knowledge Graph Embedding for Cross-lingual Knowledge Alignment. [[Slides](http://yellowstone.cs.ucla.edu/~muhao/slides/mtranse_slides_short.pdf)]
4. SimplE Embedding for Link Prediction in Knowledge Graphs
5. STransE: a novel embedding model of entities and relationships in knowledge bases (NAACL 2016)
6. The Role of “Condition”: A Novel Scientific Knowledge Graph Representation and Construction Model [[Paper](https://dl.acm.org/citation.cfm?id=3292500.3330942), [Presentation](https://www.kdd.org/kdd2019/accepted-papers/view/the-role-of-condition-a-novel-scientific-knowledge-graph-representation-and)] (KDD 2019)
7. Universal Representation Learning of Knowledge Bases by Jointly Embedding Instances and Ontological Concepts [[Paper](http://web.cs.ucla.edu/~yzsun/papers/2019_KDD_JOIE.pdf), [Presentation](https://www.kdd.org/kdd2019/accepted-papers/view/universal-representation-learning-of-knowledge-bases-by-jointly-embedding-i)] (KDD 2019)
8. NSCaching: Simple and Efficient Negative Sampling for Knowledge Graph Embedding [[PDF](https://arxiv.org/pdf/1812.06410.pdf)] (ICDE 2019) 🌟
> How to find valuable negative samples efficiently
9. Entity Integrity, Referential Integrity, and Query Optimization with Embedded Uniqueness Constraints [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8731360), short paper] (ICDE 2019) 🌟
10. AutoSF: Searching Scoring Functions for Knowledge Graph Embedding [[Video](https://www.google.com/url?q=https://drive.google.com/open?id%3D1wRHmVHiit8xIZalwL2ZUx5IZcu8BVr_4&sa=D&ust=1587488616452000&usg=AFQjCNF27HybM9QnROVO4NeCbqFVvObi0w)][[Slides](https://www.google.com/url?q=https://drive.google.com/open?id%3D1fYdh05WWG0Aco403ArzWafMrf7-joBpu&sa=D&ust=1587488616452000&usg=AFQjCNHnaXb02kbU7LZq5zHG1RhvDon07A)][[Paper](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300a433/290300a433.pdf)] (ICDE 2020) 🌟
11. TransN: Heterogeneous Network Representation Learning by Translating Node Embeddings [[Video](https://www.google.com/url?q=https://drive.google.com/open?id%3D1-KH4NUD2LNN1ESvbXTUfu3HDOYXYylqx&sa=D&ust=1595668107927000&usg=AFQjCNF74glNGWzt3FmGSo5W9th8VGfGwQ)][[Slides](https://www.google.com/url?q=https://drive.google.com/open?id%3D1CAuwlXPIV1rLXZFHvln-VvoSr3IRtM59&sa=D&ust=1595668107927000&usg=AFQjCNELQ0Q52103E2s_vziBq5_jF9TOdQ)][[Paper](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300a589/290300a589.pdf)] (ICDE 2020) 🌟
12. Generalized Translation-Based Embedding of Knowledge Graph (TKDE 2020) 🌟
13. Interstellar: Searching Recurrent Architecture for Knowledge Graph Embedding (NeurIPS 2020) [[Paper](https://proceedings.neurips.cc/paper/2020/file/722caafb4825ef5d8670710fa29087cf-Paper.pdf)]
14. DGL-KE: Training Knowledge Graph Embeddings at Scale (SIGIR 2020) [[Paper](https://arxiv.org/pdf/2004.08532.pdf)] [[Code](https://github.com/awslabs/dgl-ke)]

__Dynamic Embedding__
1. Dynamic Word Embeddings [[Paper](https://arxiv.org/pdf/1702.08359.pdf)]
2. DYREP: LEARNING REPRESENTATIONS OVER DYNAMIC GRAPHS [ICLR 2019] [[Paper](https://openreview.net/pdf?id=HyePrhR5KX)]
3. Know-Evolve: Deep Temporal Reasoning for Dynamic Knowledge Graphs [Know-Evolve, ICML 2017][[Paper](http://proceedings.mlr.press/v70/trivedi17a/trivedi17a.pdf)][[Code (C++)](https://github.com/rstriv/Know-Evolve)]
4. Continuous-Time Dynamic Network Embeddings [WWW 2018] [[Paper](http://ryanrossi.com/pubs/nguyen-et-al-WWW18-BigNet.pdf)]
5. Efficiently Embedding Dynamic Knowledge Graphs (2019) [[Paper](https://arxiv.org/pdf/1910.06708.pdf)]

__KG Reasoning__
1. Know-Evolve: Deep Temporal Reasoning for Dynamic Knowledge Graphs (Know-Evolve, ICML 2017)[[Paper](http://proceedings.mlr.press/v70/trivedi17a/trivedi17a.pdf)][[Code (C++)](https://github.com/rstriv/Know-Evolve)]
2. DeepPath: A Reinforcement Learning Method for Knowledge Graph Reasoning (DeepPath, EMNLP 2017) [Code](https://github.com/xwhan/DeepPath Notes: https://zhuanlan.zhihu.com/p/33536026)
3. Reading and Reasoning with Knowledge Graphs (PhD Thesis of Matthew Gardner) [[Thesis](http://www.cs.cmu.edu/~mg1/thesis.pdf)]
> * Reasoning, Relation Extraction, Modeling Lexical Semantics 
4. The Vadalog System: Datalog-based Reasoning for Knowledge Graphs (VLDB 2018)[[PDF](http://www.vldb.org/pvldb/vol11/p975-bellomarini.pdf)] 🌟
5. Linguistic Petri Nets Based on Cloud Model Theory for Knowledge Representation and Reasoning (TKDE 2018) 🌟
6. Iteratively Learning Embeddings and Rules for Knowledge Graph Reasoning (WWW 2019)

__Rule Mining and Path Finding in KGs__
1. RuDiK: Rule Discovery in Knowledge Bases (VLDB 2018) [[PDF](http://www.vldb.org/pvldb/vol11/p1946-ortona.pdf), demo] 🌟
2. Discovering Diversified Paths in Knowledge Bases (VLDB 2018) [[PDF](http://www.vldb.org/pvldb/vol11/p2002-aebeloe.pdf), demo] 🌟
3. Robust Discovery of Positive and Negative Rules in Knowledge Bases (ICDE 2018) [[PDF](http://www.eurecom.fr/fr/publication/5321/download/data-publi-5321_2.pdf)] 🌟

__Related Reading__
1. Awesome Embeddings [[GitHub](https://arxiv.org/pdf/2004.08532.pdf)]
