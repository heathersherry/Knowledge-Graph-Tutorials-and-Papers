## Knowledge Graph Recommendation

### 📝 Tutorials and Surveys
__General Tutorials__
1. Learning and Reasoning on Graph for Recommendation (CIKM 2019 Tutorial) [[GitHub](https://next-nus.github.io/)]
2. Tutorial on Large Language Models for Recommendation (RecSys 2023) [[Paper](https://dl.acm.org/doi/abs/10.1145/3604915.3609494?casa_token=Z1-c53RaQLMAAAAA:XzzOBkKnZYzUlXcb16eBYsNNJJSzi-YCrXymaCOLKfM0uIbjyTTBdr1FX9IZy8-I-ckYvwHxDu40Ug)] 🔥

__Surveys__
1. A Survey on Knowledge Graph-Based Recommender Systems (TKDE 2020) [[Paper](https://arxiv.org/pdf/2003.00911.pdf)][[Notes](https://mp.weixin.qq.com/s/d3rytwQ5Yta_hTGxtqXmvQ)] 🌟
2. KG4RecEval: Does Knowledge Graph Really Matter for Recommender Systems? (ACM Transactions on Information Systems 2025) [[Paper](https://dl.acm.org/doi/abs/10.1145/3713071)]
> * To remove, randomly distort or decrease knowledge does not necessarily decrease recommendation accuracy, even for cold-start users.

### 📝 Research Papers
__General Topics__
1. AKUPM: Attention-Enhanced Knowledge-Aware User Preference Model for Recommendation [[Paper](https://dl.acm.org/citation.cfm?doid=3292500.3330705), applied science track] (KDD 2019) 
2. KGAT: Knowledge Graph Attention Network for Recommendation [[Paper](https://arxiv.org/pdf/1905.07854.pdf), [Presentation](https://www.kdd.org/kdd2019/accepted-papers/view/kgat-knowledge-graph-attention-network-for-recommendation), [Code](https://github.com/xiangwang1223/knowledge_graph_attention_network)] (KDD 2019) 
3. Knowledge-aware Graph Neural Networks with Label Smoothness Regularization for Recommender Systems [[Paper](https://arxiv.org/pdf/1905.04413.pdf), [Presentation](https://www.kdd.org/kdd2019/accepted-papers/view/knowledge-aware-graph-neural-networks-with-label-smoothness-regularization-)] (KDD 2019) 
4. Improving Conversational Recommender Systems via Knowledge Graph based Semantic Fusion (KDD 2020)
5. Reinforced Negative Sampling over Knowledge Graph for Recommendation (WWW 2020)
6. Unifying Knowledge Graph Learning and Recommendation: Towards a Better Understanding of User Preferences (WWW 2019)
7. Jointly Learning Explainable Rules for Recommendation with Knowledge Graph (WWW 2019)
8. Multi-Task Feature Learning for Knowledge Graph Enhanced Recommendation (WWW 2019)
9. Knowledge Graph Convolutional Networks for Recommender Systems (WWW 2019)
10. Towards Knowledge-Based Recommender Dialog System (EMNLP-IJCNLP 2019)
11. Explianable Reasoning over Knowledge Graphs for Recommendation (AAAI 2019)
12. RippleNet: Propagating User Preferences on the Knowledge Graph for Recommender Systems (CIKM 2018)
13. Collaborative knowledge base embedding for recommender systems (KDD 2016) [[Paper](https://dl.acm.org/doi/pdf/10.1145/2939672.2939673)]
14. Dbrec—music recommendations using DBpedia (ISWC 2020)
15. Reinforcement Knowledge Graph Reasoning for Explainable Recommendation (SIGIR 2019) 
16. Multi-modal Knowledge Graphs for Recommender Systems (CIKM 2020) [[Paper](https://zheng-kai.com/paper/cikm_2020_sun.pdf)]
17. Embedding-Based Recommendations on Scholarly Knowledge Graphs (ESWC 2020) [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-49461-2_15)]
18. Recurrent Knowledge Graph Embedding for Effective Recommendation (RecSys 2018) [[Paper](https://yangjiera.github.io/pdf/sun2018recsys.pdf)]
19. Fairness-Aware Explainable Re commendationover Knowledge Graph (SIGIR 2020) [[Paper](https://dl.acm.org/doi/epdf/10.1145/3397271.3401051)]
20. Attentional Graph Convolutional Networks for Knowledge Concept Recommendation in MOOCs in a Heterogeneous View (SIGIR 2020)
21. Interactive Recommender System via Knowledge Graph-enhanced Reinforcement Learning (SIGIR 2020)
22. Multi-Task Feature Learning for Knowledge Graph Enhanced Recommendation (WWW 2019) [[Paper](https://arxiv.org/pdf/1901.08907.pdf)] [[Code](https://github.com/hwwang55/MKR)]
23. RippleNet: Propagating User Preferences on the Knowledge Graph for Recommender Systems (CIKM 2018) [[Paper](https://arxiv.org/pdf/1803.03467.pdf)] 
24. Learning Intents behind Interactions with Knowledge Graph for Recommendation (WWW 2021)
25. Learning Dynamic User Interest Sequence in Knowledge Graphs for Click-Through Rate Prediction (TKDE 2021) [[Paper](https://ieeexplore.ieee.org/document/9409651)]
26. Reinforced Anchor Knowledge Graph Generation for News Recommendation Reasoning (KDD 2021) [[Paper](https://www.microsoft.com/en-us/research/uploads/prod/2021/05/KDD2021-anchorkg.pdf)]
27. DiffKG: Knowledge Graph Diffusion Model for Recommendation (WSDM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3616855.3635850)]
28. AKGNN: Attribute Knowledge Graph Neural Networks Recommendation for Corporate Volunteer Activities (IEEE Transactions on Big Data 2024) [[Paper](https://ieeexplore.ieee.org/abstract/document/10664007)]
29. Knowledge Graph Fine-grained Modeling Network with Contrastive Learning for Recommendation (ACM Transactions on Knowledge Discovery from Data 2025) [[Paper](https://dl.acm.org/doi/abs/10.1145/3744926)]

__Dynamic Senarios (what if the item-user and the KG are updating?)__
* But it seems that there is no good ground truth datasets for evaluation? 😅 ...

__Explainability__
1. Explainable Knowledge Graph-based Recommendation via Deep Reinforcement Learning (arxiv 2019) [[Paper](https://arxiv.org/abs/1906.09506)]
> * Explainability analysis: Fig 2 and Table 3
2. Unifying Knowledge Graph Learning and Recommendation: Towards a Better Understanding of User Preferences (WWW 2019) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3308558.3313705)]
> * Explainability analysis: Case Study in Sec 6.7
3. Explainable recommendation based on knowledge graph and multi-objective optimization (Complex & Intelligent Systems 2021)
> * Multi-objective optimization of recommendation performance and explanability (Pareto solution)
> * Explainability analysis: Table 5, Table 6, Fig 5
4. Fairness-Aware Explainable Recommendation over Knowledge Graphs (SIGIR 2020)
> * Path is the explanation for the recommendation (Fig 1)
> * Explainability analysis: case study in Fig 7 (explainable path)
5. Learning Heterogeneous Knowledge Base Embeddings for Explainable Recommendation (Algorithms 2018)
6. KGAT: Knowledge Graph Attention Network for Recommendation (KDD 2019)
7. Reinforcement knowledge graph reasoning for explainable recommendation (SIGIR 2019)

__Recommendation related to LLM__ 🔥🔥🔥
1. Breaking the Barrier: Utilizing Large Language Models for Industrial Recommendation Systems through an Inferential Knowledge Graph (Arxiv 2024, from Alibaba) [[Paper](https://arxiv.org/pdf/2402.13750.pdf)] [[Blog](https://mp.weixin.qq.com/s/WIFTUHAp4PXX_wx0QMOsHw)]
> * LLMs+Inferential Knowledge Graph: Better understanding and prediction of user perchase.
> * LLM-KERec: (1) There is an entity extractor that extracts unified concept terms from items and user information. (2) To provide cost-effective and reliable prior knowledge, entity pairs are generated based on entity popularity and specific strategies. (3) The LLM determines complementary relationships in each entity pair, and constructs a complementary knowledge graph. (4) A new complementary recall module and an Entity-Entity-Item (E-E-I) weight decision model refine the scoring of the ranking model by using real complementary exposure-click samples.
2. LLM is Knowledge Graph Reasoner: LLM’s Intuition-Aware Knowledge Graph Reasoning for Cold-Start Sequential Recommendation (ECIR 2025) [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-88711-6_17)]
3. KGGLM: A Generative Language Model for Generalizable Knowledge Graph Representation Learning in Recommendation (RecSys 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3640457.3691703)]
4. Knowledge Graph Retrieval-Augmented Generation for LLM-based Recommendation (ACL 2025)

### 💬 Related Reading and Discusssion
1. Explainable Recommendation: A Survey and New Perspectives (Foundations and Trends in Information Retrieval, 2020) [[PDF](https://arxiv.org/pdf/1804.11192.pdf)]
