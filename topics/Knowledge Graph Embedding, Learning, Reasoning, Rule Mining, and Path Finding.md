## Knowledge Graph Embedding, Learning, Reasoning, Rule Mining, and Path Finding
```
KG Embedding/Learning/Reasoning also contributes to a lot of downstream tasks such as KG completion and KGQA.
Therefore, you may also find KG Embedding/Learning/Reasoning in the KG applications sections.
```

### 📝 Surveys and Summary
__Surveys, Tutorials and Experimental Studies__
1. Knowledge graph embedding: A survey of approaches and applications (TKDE 2017)🌟
2. Knowledge representation learning: A quantitative review (2018) [[Code in this paper](https://github.com/thunlp/OpenKE)]
3. A Comprehensive Survey of Knowledge Graph Embeddings with Literals: Techniques and Applications (ESWC 2019) [[Paper](http://ceur-ws.org/Vol-2377/paper_4.pdf)]
4. Knowledge Graph Embedding for Link Prediction: A Comparative Analysis [[Paper](https://arxiv.org/pdf/2002.00819.pdf)]
5. Realistic Re-evaluation of Knowledge Graph Completion Methods: An Experimental Study [[Paper](https://doi.org/10.1145/3318464.3380599)] (SIGMOD 2020) 🌟
6. Reasoning on Knowledge Graphs: Symbolic or Neural? (AAAI 2022 Tutorial) [[Link](https://aaai2022kgreasoning.github.io/)]
7. A Survey of Knowledge Graph Reasoning on Graph Types: Static, Dynamic, and Multimodal	[[Link](https://github.com/LIANGKE23/Awesome-Knowledge-Graph-Reasoning)]
8. Uniting Large Language Models and Knowledge Graphs for Enhanced Knowledge Representation (Big Data LDN 2023) [[Video](https://www.youtube.com/watch?v=CEaDSOh_AoM)] 🔥
9. Knowledge Graph Embedding: A Survey from the Perspective of Representation Spaces (ACM Computing Surveys 2024) [[Paper](https://dl.acm.org/doi/full/10.1145/3643806)]
10. Overview of knowledge reasoning for knowledge graph (Neurocomputing 2024) [[Paper](https://www.sciencedirect.com/science/article/pii/S0925231224003424)]
11. LLMs for knowledge graph construction and reasoning: recent capabilities and future opportunities (WWW jornal 2024) [[Paper](https://link.springer.com/article/10.1007/s11280-024-01297-w)] 🔥
12. Graph machine learning in the era of large language models (llms) (TKDE 2024) [[Paper](https://arxiv.org/pdf/2404.14928)] 🌟

__Summary__
1. Papers, Surveys, and Datasets on Knowledge Graph Embedding (KGE) [[GitHub](https://github.com/xinguoxia/KGE)]
2. Knowledge Graph Reasoning: Recent Advances (Slides) [[Link](https://sites.cs.ucsb.edu/~william/papers/Part3_KB_Reasoning.pdf)]
3. KG Embedding Approaches [[Link](https://gist.github.com/mommi84/07f7c044fa18aaaa7b5133230207d8d4)]

__Related Reading__
1. Awesome Embeddings [[GitHub](https://arxiv.org/pdf/2004.08532.pdf)]
2. Stanford CS224W - Knowledge Graph Reasoning [[Slides](http://web.stanford.edu/class/cs224w/slides/17-knowledge.pdf)]
3. Random Walk in Node Embeddings (DeepWalk, node2vec, LINE, and GraphSAGE) [[Link](https://medium.com/towards-artificial-intelligence/random-walk-in-node-embeddings-deepwalk-node2vec-line-and-graphsage-ca23df60e493)]


### 📝 KG Embedding and KG Representation
__General Papers__
1. DeepWalk: Online Learning of Social Representations (DeepWalk, KDD 2014) [[Code](https://github.com/phanein/deepwalk), [Slides](https://www.slideshare.net/bperz/14-kdddeep-walk-2)]
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
> * How to find valuable negative samples efficiently
9. Entity Integrity, Referential Integrity, and Query Optimization with Embedded Uniqueness Constraints [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8731360), short paper] (ICDE 2019) 🌟
10. AutoSF: Searching Scoring Functions for Knowledge Graph Embedding [[Video](https://www.google.com/url?q=https://drive.google.com/open?id%3D1wRHmVHiit8xIZalwL2ZUx5IZcu8BVr_4&sa=D&ust=1587488616452000&usg=AFQjCNF27HybM9QnROVO4NeCbqFVvObi0w)][[Slides](https://www.google.com/url?q=https://drive.google.com/open?id%3D1fYdh05WWG0Aco403ArzWafMrf7-joBpu&sa=D&ust=1587488616452000&usg=AFQjCNHnaXb02kbU7LZq5zHG1RhvDon07A)][[Paper](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300a433/290300a433.pdf)] (ICDE 2020) 🌟
11. TransN: Heterogeneous Network Representation Learning by Translating Node Embeddings [[Video](https://www.google.com/url?q=https://drive.google.com/open?id%3D1-KH4NUD2LNN1ESvbXTUfu3HDOYXYylqx&sa=D&ust=1595668107927000&usg=AFQjCNF74glNGWzt3FmGSo5W9th8VGfGwQ)][[Slides](https://www.google.com/url?q=https://drive.google.com/open?id%3D1CAuwlXPIV1rLXZFHvln-VvoSr3IRtM59&sa=D&ust=1595668107927000&usg=AFQjCNELQ0Q52103E2s_vziBq5_jF9TOdQ)][[Paper](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300a589/290300a589.pdf)] (ICDE 2020) 🌟
12. Generalized Translation-Based Embedding of Knowledge Graph (TKDE 2020) 🌟
13. Interstellar: Searching Recurrent Architecture for Knowledge Graph Embedding (NeurIPS 2020) [[Paper](https://proceedings.neurips.cc/paper/2020/file/722caafb4825ef5d8670710fa29087cf-Paper.pdf)]
14. DGL-KE: Training Knowledge Graph Embeddings at Scale (SIGIR 2020) [[Paper](https://arxiv.org/pdf/2004.08532.pdf)] [[Code](https://github.com/awslabs/dgl-ke)]
15. Iterative Entity Alignment via Joint Knowledge Embeddings (IJCAI 2017) [[Paper](https://www.ijcai.org/Proceedings/2017/0595.pdf)] [[Slides](http://www.zhuhao.me/static/zhu17iterative/zhu17iterative_slides.pdf)]
16. Representation Learning of Knowledge Graphs with Hierarchical Types (IJCAI 2016) [[Paper](https://www.ijcai.org/Proceedings/16/Papers/421.pdf)] 
> *  relation prediction: predict relations between two given entities, i.e., (h; ?; t).
17. Modeling Relation Paths for Representation Learning of Knowledge Bases (EMNLP 2015) [[Paper](https://www.aclweb.org/anthology/D15-1082.pdf)] [[Code](https://github.com/mrlyk423/relation_extraction)]
> *  relation prediction: predict relations between two given entities, i.e., (h; ?; t).
18. Efficient Knowledge Graph Embedding without Negative Sampling (WWW 2021)
19. MQuadE: a Unified Model for Knowledge Fact Embedding (WWW 2021)
20. MulDE: Multi-teacher Knowledge Distillation for Low-dimensional Knowledge Graph Embeddings (WWW 2021)
21. Efficient Relation-Aware Scoring Function Search for Knowledge Graph Embedding (ICDE 2021) 🌟
22. Simple and automated negative sampling for knowledge graph embedding [[Paper](https://link.springer.com/article/10.1007/s00778-020-00640-7)] (VLDBJ 2021) 🌟
23. OntoProtein: Protein Pretraining With Gene Ontology Embedding (ICLR 2022) [[Paper](https://arxiv.org/pdf/2201.11147.pdf)] [[Github](https://github.com/zjunlp/OntoProtein)]
24. How to Turn Your Knowledge Graph Embeddings into Generative Models (NeurIPS 2023) [[Paper](https://proceedings.neurips.cc/paper_files/paper/2023/file/f4b768188be63b8d2680a46934fd295a-Paper-Conference.pdf)]
25. Towards Continual Knowledge Graph Embedding via Incremental Distillation (AAAI 2024) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/28722)]
26. Knowledge Graph Enhanced Multimodal Transformer for Image-Text Retrieval (ICDE 2024) 🌟
27. Exploiting Pre-trained Language Models for Black-box Attack against Knowledge Graph Embeddings (TKDD 2024)
28. Document-Level Relation Extraction Based on Heterogeneous Graph Reasoning (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679899)]
29. Embedding Knowledge Graphs in Function Spaces (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679819)]
30. Clustering then Propagation: Select Better Anchors for Knowledge Graph Embedding (NeuRIPS 2024)
31. Noise-powered Multi-modal Knowledge Graph Representation Framework (COLING 2025)
31. Distance-Adaptive Quaternion Knowledge Graph Embedding with Bidirectional Rotation (COLING 2025)
32. Including Co-Relation via Concatenate Operator for Static and Temporal Knowledge Graph Embedding (ACM Transactions on Information Systems, 2025) [[Paper](https://dl.acm.org/doi/abs/10.1145/3733231)]
33. Structure Is All You Need: Structural Representation Learning on Hyper-Relational Knowledge Graphs (ICML 2025, poster)
34. Improving Soft Unification with Knowledge Graph Embedding Methods (ICML 2025, poster)
35. Universal Knowledge Graph Embeddings (WWW 2024) [[Paper](https://doi.org/10.1145/3589335.3651978)]
36. Poisoning Attack on Federated Knowledge Graph Embedding (WWW 2024) [[Paper](https://doi.org/10.1145/3589334.3645422)]
37. Robustness Evaluation of Knowledge Graph Embedding Models Under Non-targeted Attacks (ESWC 2025) [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-94575-5_15)]
38. Croppable Knowledge Graph Embedding (ACL 2025)
39. RSCF: Relation-Semantics Consistent Filter for Entity Embedding of Knowledge Graph (ACL 2025)
40. A Mutual Information Perspective on Knowledge Graph Embedding (ACL 2025) [[Paper](https://aclanthology.org/2025.acl-long.1077/)]
41. Conformalized Answer Set Prediction for Knowledge Graph Embedding (NAACL 2025)
42. Mitigating Heterogeneity among Factor Tensors via Lie Group Manifolds for Tensor Decomposition Based Temporal Knowledge Graph Embedding (NAACL 2025)
43. Structure Is All You Need: Structural Representation Learning on Hyper-Relational Knowledge Graphs (ICML 2025) [[Paper](https://openreview.net/forum?id=2tH2vexW1Z)]
44. Predicate-Conditional Conformalized Answer Sets for Knowledge Graph Embeddings (ACL 2025)
45. Time-enhanced compound geometric operations for temporal knowledge graph embedding (Neurocomputing 2025) [[Paper](https://www.sciencedirect.com/science/article/pii/S0925231225018545)]
46. Less Is MuRE: Revisiting Shallow Knowledge Graph Embeddings (EMNLP 2025) [[Paper](https://aclanthology.org/2025.emnlp-main.779/)]
47. Improving Soft Unification with Knowledge Graph Embedding Methods (ICML 2025) [[Paper](https://icml.cc/virtual/2025/poster/45835)]
48. Structure Is All You Need: Structural Representation Learning on Hyper-Relational Knowledge Graphs (ICML 2025) [[Paper](https://icml.cc/virtual/2025/poster/46565)]

 
__Dynamic/Adaptive Embedding__
1. Dynamic Word Embeddings [[Paper](https://arxiv.org/pdf/1702.08359.pdf)]
2. DYREP: LEARNING REPRESENTATIONS OVER DYNAMIC GRAPHS [ICLR 2019] [[Paper](https://openreview.net/pdf?id=HyePrhR5KX)]
3. Know-Evolve: Deep Temporal Reasoning for Dynamic Knowledge Graphs [Know-Evolve, ICML 2017][[Paper](http://proceedings.mlr.press/v70/trivedi17a/trivedi17a.pdf)][[Code (C++)](https://github.com/rstriv/Know-Evolve)]
4. Continuous-Time Dynamic Network Embeddings [WWW 2018] [[Paper](http://ryanrossi.com/pubs/nguyen-et-al-WWW18-BigNet.pdf)]
5. Efficiently Embedding Dynamic Knowledge Graphs (2019) [[Paper](https://arxiv.org/pdf/1910.06708.pdf)]
6. Dynamic Heterogeneous Information Network Embedding with Meta-path based Proximity (TKDE 2020) [[https://ieeexplore.ieee.org/document/9091208]] [[Github](https://github.com/rootlu/DyHNE)]
7. ChronoR: Rotation Based Temporal Knowledge Graph Embedding (arxiv 2021 or AAAI 2021?) [[Paper](https://arxiv.org/abs/2103.10379)]
8. AdaE: Knowledge Graph Embedding with Adaptive Embedding Sizes (TKDE 2025) [[Paper](https://ieeexplore.ieee.org/abstract/document/10981648)] 🌟
9. SIT: Selective Incremental Training for Dynamic Knowledge Graph Embedding (ICDE 2025) 🌟

__CNN Based Embedding__
1. A novel embedding model for knowledge base completion based on convolutional neural network (NAACL 2018)
2. Convolutional 2d knowledge graph embeddings (AAAI 2018)

__Graph Based Embedding__
1. Learning Attention-based Embeddings for Relation Prediction in Knowledge Graphs (ACL 2019) [[Paper](https://arxiv.org/pdf/1906.01195.pdf)]
> * Guide attention to both entity (node) and relation (edge) features in a multi-hop neigh-borhood of a given entity/node
> * This paper discuss that KG embedding models are classified as (1) translational models (which are more widely used and popular, such as TransE), (2) CNN based models, and (3) graph based models.
2. Modeling Relational Data with Graph Convolutional Networks (ESWC 2018) [[Paper](https://arxiv.org/pdf/1703.06103.pdf)]
> * Apply GCN for KG Completion (link prediction), compared with the performance of KG embedding models in the experiment.

__Enfficient Emedding__
1. NodePiece: Compositional and Parameter-Efficient Representations of Large Knowledge Graphs (ICLR 2022) [[Paper](https://openreview.net/forum?id=xMJWUKJnFSw)]
> * Anchor based strategy, to achieve parameter efficiency.
> * Some new works have already use NodePiece in experiments, such as InterHT: Knowledge Graph Embeddings by Interaction between Head and Tail Entities (Arxiv 2022) [[Paper](https://arxiv.org/pdf/2202.04897.pdf)]

__LLM related__ 🔥
1. LLM-Guided Explanation Generation for Knowledge Graph Embedding-Based Node Classification (ACL 2025 submission) [[Paper](https://openreview.net/forum?id=vSucHYb4oh)]

__Related Reading__
1. Neural Subgraph Isomorphism Counting (KDD 2020) [[Paper](https://arxiv.org/pdf/1912.11589.pdf)] [[Code](https://github.com/HKUST-KnowComp/NeuralSubgraphCounting)] 🌟
2. DFS-based frequent graph pattern extraction to characterize the content of RDF Triple Stores (2010) [[Paper](https://hal.inria.fr/hal-01170896/document)]
3. COMPOSITION-BASED MULTI-RELATIONAL GRAPH CONVOLUTIONAL NETWORKS (ICLR 2020) [[Paper](https://arxiv.org/pdf/1911.03082.pdf)] [[Code](https://github.com/malllabiisc/CompGCN)]
5. Knowledge Embedding Based Graph Convolutional Network (WWW 2021)
6. Making Large Language Models Perform Better in Knowledge Graph Completion (Arxiv 2024) [[Paper](https://arxiv.org/abs/2310.06671)]

__Downstream Applications__
1. Link Prediction
> * You may refer to the SOTA listed on PaperWithCode, e.g., the exp results on FB15K [[Link](https://paperswithcode.com/sota/link-prediction-on-fb15k-237)]
2. Entity Classification

### 📝 KG Reasoning
__Summarys and Surveys__
1. Knowledge Graph Reasoning Papers [[GitHub](https://github.com/THU-KEG/Knowledge_Graph_Reasoning_Papers)]
2. Awesome-Knowledge-Graph-Reasoning [[GitHub](https://github.com/LIANGKE23/Awesome-Knowledge-Graph-Reasoning)]
3. A Survey of Knowledge Graph Reasoning on Graph Types: Static, Dynamic, and Multi-Modal [[Paper](https://ieeexplore.ieee.org/abstract/document/10577554)]
4. Neural-Symbolic Methods for Knowledge Graph Reasoning: A Survey (ACM Transactions on Knowledge Discovery from Data 2025) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3686806)]

__General Papers__
1. Know-Evolve: Deep Temporal Reasoning for Dynamic Knowledge Graphs (Know-Evolve, ICML 2017)[[Paper](http://proceedings.mlr.press/v70/trivedi17a/trivedi17a.pdf)][[Code (C++)](https://github.com/rstriv/Know-Evolve)]
2. DeepPath: A Reinforcement Learning Method for Knowledge Graph Reasoning (DeepPath, EMNLP 2017) [Code](https://github.com/xwhan/DeepPath Notes: https://zhuanlan.zhihu.com/p/33536026)
3. Reading and Reasoning with Knowledge Graphs (PhD Thesis of Matthew Gardner) [[Thesis](http://www.cs.cmu.edu/~mg1/thesis.pdf)]
> * Reasoning, Relation Extraction, Modeling Lexical Semantics 
4. The Vadalog System: Datalog-based Reasoning for Knowledge Graphs (VLDB 2018)[[PDF](http://www.vldb.org/pvldb/vol11/p975-bellomarini.pdf)] 🌟
5. Linguistic Petri Nets Based on Cloud Model Theory for Knowledge Representation and Reasoning (TKDE 2018) 🌟
6. Iteratively Learning Embeddings and Rules for Knowledge Graph Reasoning (WWW 2019)
7. Beta Embeddings for Multi-Hop Logical Reasoning in Knowledge Graphs (NeurIPS 2020) [[Paper and Code](http://snap.stanford.edu/betae/)]
8. Query2box: Reasoning Over Knowledge Graphs In Vector Space Using Box Embeddings (ICLR 2020)
9. Incorporating Graph Attention Mechanism into Knowledge Graph Reasoning Based on Deep Reinforcement Learning (EMNLP 2019)
10. DIVINE: A Generative Adversarial Imitation Learning Framework for Knowledge Graph Reasoning  (EMNLP 2019)
11. Collaborative Policy Learning for Open Knowledge Graph Reasoning (EMNLP 2019)
12. Adapting Meta Knowledge Graph Information for Multi-Hop Reasoning over Few-Shot Relations (EMNLP 2019) [[Paper](https://arxiv.org/abs/1908.11513)]
13. xERTE: Explainable Subgraph Reasoning for Forecasting on Temporal Knowledge Graphs (ICLR 2021) [[Paper](https://openreview.net/pdf?id=pGIHq1m7PU)] [[Code](https://github.com/TemporalKGTeam/xERTE)] 
14. SMORE: KNOWLEDGE GRAPH COMPLETION AND MULTI-HOP REASONING IN MASSIVE KNOWLEDGE GRAPHS (Jure's group, Oct 2021) [[Paper](https://arxiv.org/pdf/2110.14890.pdf)]
15. Knowledge Graph Reasoning with Relational Digraph (arxiv 2022) [[Paper](https://arxiv.org/pdf/2108.06040.pdf)]
16. Local-Global History-aware Contrastive Learning for Temporal Knowledge Graph Reasoning (ICDE 2024) 🌟
17. Towards Foundation Models for Knowledge Graph Reasoning (ICLR 2024) [[Paper](https://arxiv.org/pdf/2310.04562)] [[Discussion](https://mp.weixin.qq.com/s?__biz=MzU2NjAxNDYwMg==&mid=2247507232&idx=1&sn=d0d987505e14b5fdc07bfbbac61ef052&chksm=fcb07ac5cbc7f3d39e72a107ba52980d50eca7c3404aab2ee6c316e82f153ff81314a4da6916&token=614723215&lang=zh_CN#rd)]
18. Relation Logical Reasoning and Relation-aware Entity Encoding for Temporal Knowledge Graph Reasoning (COLING 2025)
19. Hawkes based Representation Learning for Reasoning over Scale-free Community-structured Temporal Knowledge Graphs (COLING 2025)
20. Large Language Models-guided Dynamic Adaptation for Temporal Knowledge Graph Reasoning (NeurIPS 2024) [[Paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/0fd17409385ab9304e5019c6a6eb327a-Abstract-Conference.html)] 🔥
21. DPCL-Diff: The Temporal Knowledge Graph Reasoning Based on Graph Node Diffusion Model with Dual-Domain Periodic Contrastive Learning (AAAI 2025) [[Paper](https://arxiv.org/abs/2411.01477)]
22. Advancing Abductive Reasoning in Knowledge Graphs through Complex Logical Hypothesis Generation (Yangqiu Song, ACL 2024)
23. Reasoning of Large Language Models over Knowledge Graphs with Super-Relations (ICLR 2025, Poster) [[Paper](https://openreview.net/forum?id=rTCJ29pkuA)] 🔥
24. INFER: A Neural-symbolic Model For Extrapolation Reasoning on Temporal Knowledge Graph (ICLR 2025, Poster) [[Paper](https://openreview.net/forum?id=ExHUtB2vnz)]
25. CHAINSFORMER: Numerical Reasoning on Knowledge Graphs from a Chain Perspective (ICDE 2025) [[Paper](https://arxiv.org/abs/2504.14282)] 🌟
26. Improving Complex Reasoning over Knowledge Graph with Logic-Aware Curriculum Tuning (AAAI 2025, Technical Tracks) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/33405)]
27. Decoding on Graphs: Faithful and Sound Reasoning on Knowledge Graphs through Generation of Well-Formed Chains (ACL 2025)
28. FedEAN: Entity-Aware Adversarial Negative Sampling for Federated Knowledge Graph Reasoning (TKDE 2024) 🌟
29. Mixture of Length and Pruning Experts for Knowledge Graphs Reasoning (EMNLP 2025)
30. Certainty in Uncertainty: Reasoning over Uncertain Knowledge Graphs with Statistical Guarantees (EMNLP 2025)
31. Historically Relevant Event Structuring for Temporal Knowledge Graph Reasoning (ICDE 2025) [[Paper](https://arxiv.org/abs/2405.10621)] 🌟
32. A Generative Adaptive Replay Continual Learning Model for Temporal Knowledge Graph Reasoning (ACL 2025) [[Paper](https://arxiv.org/pdf/2506.04083)]

__KG Reasoning for LLM, or LLM for KG Reasoning__ 🔥
1. REASONING ON GRAPHS: FAITHFUL AND INTERPRETABLE LARGE LANGUAGE MODEL REASONING (ICLR 2024) [[Paper](https://arxiv.org/pdf/2310.01061.pdf)] [[Discussion](https://www.linkedin.com/posts/jay-jiebing-yu-ph-d-7b97a8_llm-knowledgegraph-trustworthyai-activity-7116434650113208320-1RJb/)]
2. KG-GPT: A General Framework for Reasoning on Knowledge Graphs Using Large Language Models (EMNLP 2023) [[Paper](https://aclanthology.org/2023.findings-emnlp.631/)]
3. LLM-based Typed Hyperresolution for Commonsense Reasoning with Knowledge Bases (ICLR 2025, poster) [[Paper](https://openreview.net/forum?id=wNobG8bV5Q)]
4. Graph-constrained Reasoning: Faithful Reasoning on Knowledge Graphs with Large Language Models (ICML 2025)
5. KG-Agent: An Efficient Autonomous Agent Framework for Complex Reasoning over Knowledge Graph (ACL 2025) [[Paper](https://aclanthology.org/2025.acl-long.468.pdf)]
6. CuriousLLM: Elevating Multi-Document Question Answering with LLM-Enhanced Knowledge Graph Reasoning (NAACL 2025)
7. A New Pipeline for Knowledge Graph Reasoning Enhanced by Large Language Models Without Fine-Tuning (EMNLP 2024) [[Paper](https://aclanthology.org/2024.emnlp-main.81.pdf)]
8. Large Language Models-guided Dynamic Adaptation for Temporal Knowledge Graph Reasoning (NeurIPS 2024) [[Paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/0fd17409385ab9304e5019c6a6eb327a-Abstract-Conference.html)]
9. SymAgent: A Neural-Symbolic Self-Learning Agent Framework for Complex Reasoning over Knowledge Graphs (WWW 2025) [[Paper](https://dl.acm.org/doi/abs/10.1145/3696410.3714768)]
10. Enhancing Domain-Specific Knowledge Graph Reasoning via Metapath-Based Large Model Prompt Learning (Electronics 2025)
11. Knowledge Crosswords: Geometric Knowledge Reasoning with Large Language Models (ACL 2024 - Findings) [[Paper](https://aclanthology.org/2024.findings-acl.154/)]
12. Graph-constrained Reasoning: Faithful Reasoning on Knowledge Graphs with Large Language Models (ICML 2025) [[Paper](https://arxiv.org/pdf/2410.13080)] [[Discussion (Chinese)](https://mp.weixin.qq.com/s/hKNZPyUBkmiOd0GtOL6epg)]
13. LightPROF: A Lightweight Reasoning Framework for Large Language Model on Knowledge Graph [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/34510)] [[Discussion (Chinese)](https://mp.weixin.qq.com/s/hfok-6bgmLdRC04N9lCrgA)]
14. Judge and Improve: Towards a Better Reasoning of Knowledge Graphs with Large Language Models (EMNLP 2025)
15. REASONING OF LARGE LANGUAGE MODELS OVER KNOWLEDGE GRAPHS WITH SUPER-RELATIONS (ICLR 2025) [[Paper](https://openreview.net/pdf?id=rTCJ29pkuA)]
16. PathMind: A Retrieve-Prioritize-Reason Framework for Knowledge Graph Reasoning with Large Language Models (AAAI 2026) [[Paper](https://arxiv.org/pdf/2511.14256)]

### 📝 Rule Mining and Path Finding in KGs
__General Papers__
1. RuDiK: Rule Discovery in Knowledge Bases (VLDB 2018) [[PDF](http://www.vldb.org/pvldb/vol11/p1946-ortona.pdf), demo] 🌟
2. Discovering Diversified Paths in Knowledge Bases (VLDB 2018) [[PDF](http://www.vldb.org/pvldb/vol11/p2002-aebeloe.pdf), demo] 🌟
3. Robust Discovery of Positive and Negative Rules in Knowledge Bases (ICDE 2018) [[PDF](http://www.eurecom.fr/fr/publication/5321/download/data-publi-5321_2.pdf)] 🌟
4. An Embedding-Based Approach to Rule Learning in Knowledge Graphs [[Paper](https://ieeexplore.ieee.org/document/8839576/)] (TKDE 2021) 🌟
5. Learn to Explain Efficiently via Neural Logic Inductive Learning (ICLR 2020) [[Paper](https://openreview.net/forum?id=SJlh8CEYDB)]
6. TILP: Differentiable Learning of Temporal Logical Rules on Knowledge Graphs (ICLR 2023) [[Paper](https://openreview.net/forum?id=_X12NmQKvX)]

__Rule Mining or Path Finding in KGs with LLM__ 🔥
1. ChatRule: Mining Logical Rules with Large Language Models for Knowledge Graph Reasoning (PAKDD 2025) [[Github](https://github.com/RManLuo/ChatRule)] [[Paper](https://arxiv.org/pdf/2309.01538)]
> * LLM-based Rule Generator in End2end rule mining.
2. Paths-over-Graph: Knowledge Graph Empowered Large Language Model Reasoning (WWW 2025) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3696410.3714892)]

### 📝 KG Embedding-based Node Classification
1. LLM-Guided Explanation Generation for Knowledge Graph Embedding-Based Node Classification (ACLARR 2025 - Openreview) [[Paper](https://openreview.net/forum?id=vSucHYb4oh)]


### 📊 Benchmarks
1. FB13 [[Paper](https://proceedings.neurips.cc/paper/2013/file/b337e84de8752b27eda3a12363109e80-Paper.pdf)]
2. FB15K [[Paper](https://proceedings.neurips.cc/paper/2013/file/1cecc7a77928ca8133fa24680a88d2f9-Paper.pdf)]
3. FB15K237 [[Paper](https://aclanthology.org/D15-1174/)]
4. WN11 [[Paper](https://proceedings.neurips.cc/paper/2013/file/b337e84de8752b27eda3a12363109e80-Paper.pdf)]
5. WN18 [[Paper](https://proceedings.neurips.cc/paper/2013/file/1cecc7a77928ca8133fa24680a88d2f9-Paper.pdf)]
6. WN18RR [[Paper](https://arxiv.org/abs/1707.01476)]
 

