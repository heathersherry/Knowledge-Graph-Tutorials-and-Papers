
## Entity Linking and Entity Disambiguation

### 1. Summary

__Surveys and Analysis__
1. Entity Linking with a Knowledge Base: Issues, Techniques, and Solutions (TKDE 2014) [[Paper](https://ieeexplore.ieee.org/abstract/document/6823700)] 🌟
2. Neural Entity Linking: A Survey of Models based on Deep Learning (2020) [[Paper](https://arxiv.org/pdf/2006.00575.pdf)]
> * a survey of state-of-the-art neural entity linking models
> * a survey of entity embedding techniques;
> * a discussion of recent domain-independent (zero-shot) and cross-lingual EL approaches;
> * a survey of EL applications to modeling word representations.
3. Error analysis of the well known DeepED model [[Link](https://github.com/dalab/deep-ed)]
4. Towards holistic Entity Linking: Survey and directions (Information Systems 2021) [[Link](https://www.sciencedirect.com/science/article/pii/S0306437920300958?casa_token=8iDZglH_xVgAAAAA:rHgcXMsLXdOCgSae1LEOH3Lc9LXEPyfcp9W40vRAIbEsPOxMWoAAHSi8q0M-ewkvpHWo5lB6czFS)]
5. Neural Collective Entity Linking (COLING 2018) [[Paper](https://arxiv.org/pdf/1811.08603.pdf)]

__Notes and Discussions for Entity Linking__
1. Candiate Entity Ranking [[Notes](https://www.jianshu.com/p/90e2c7a5c9f5)]
2. NLP-progress for Entity Linking [[Notes](http://nlpprogress.com/english/entity_linking.html)] [[GitHub](https://github.com/sebastianruder/NLP-progress/blob/master/english/entity_linking.md)]
3. Recent Trend for Entity Linking [[Notes](https://github.com/izuna385/EntityLinking_RecentTrend)]
4. Summary of Entity Linking [[Notes 1](http://pelhans.com/2019/02/22/entity_linking/)] [[Notes 2, check the appendices here](https://fyubang.com/2019/12/30/entity-linking/)]
5. Entity Coherence in Entity Linking [[Blog](https://blog.csdn.net/u010960155/article/details/106387771)]


### 2. General Papers
1. Zero-Shot Entity Linking by Reading Entity Descriptions (ACL 2019) [[Paper](https://www.aclweb.org/anthology/P19-1335.pdf)][[Code and Datasets](https://github.com/lajanugen/zeshel)]
2. Keyphrase Overlap Relatedness for Entity Disambiguation (CIKM 2012), LSH 🌟
3. Old is Gold: Linguistic Driven Approach for Entity and Relation Linking of Short Text (NAACL 2019), with Relation Linking
4. Improving Entity Linking by Modeling Latent Relations between Mentions (ACL 2018)
5. Entity Linking for Tweets (ACL 2013)
6. Pangloss: Fast Entity Linking in Noisy Text Environments (KDD 2018) [[Presentation](https://www.kdd.org/kdd2018/accepted-papers/view/pangloss-fast-entity-linking-in-noisy-text-environments)] 🌟
7. THINKER - Entity Linking System for Turkish Language (TKDE 2018) 🌟
8. SHINE+: A General Framework for Domain-Specific Entity Linking with Heterogeneous Information Networks (TKDE 2018) 🌟
9. SVM ensembles for named entity disambiguation (Computing, 102(4), 2020) [[Paper](https://link.springer.com/article/10.1007/s00607-019-00748-x)]
10. Attention-Based Joint Entity Linking with Entity Embedding (Information 10.2, 2019)
11. Entity Disambiguation Leveraging Multi-Perspective Attention (IEEE Access 2019)
12. CLEEK: A Chinese Long-text Corpus for Entity Linking (LREC 2020)
13. A Novel Approach for Analyzing Entity Linking Between Words and Entities for a Knowledge Base Using an Attention-Based Bilinear Joint Learning and Weighted Summation Model (IEEE Access 2019)
14. Fast and accurate entity linking via graph embedding (GRADES-NDA'19) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3327964.3328499)] [[Slides](https://www.slideshare.net/necstlab/fast-and-accurate-entity-linking-via-graph-embedding)]
15. A contrastive deep learning approach for entity linkage (ICDM 2020)
16. REL: An Entity Linker Standing on the Shoulders of Giants (SIGIR 2020) [[GitHub, API and Code](https://github.com/informagi/REL)] 
17. A probabilistic model for linking named entities in web text with heterogeneous information networks（SIGMOD 2014）[[Paper](https://dl.acm.org/doi/10.1145/2588555.2593676)] 🌟
18. Read, Retrospect, Select: An MRC Framework to Short Text Entity Linking (AAAI 2021) [[Paper](https://arxiv.org/pdf/2101.02394v1.pdf)]
19. Pivot-based Candidate Retrieval for Cross-lingual Entity Linking (WWW 2021) [[Video](http://videolectures.net/www2021_liu_candidate_retrieval/)]
20. Medical Entity Disambiguation using Graph Neural Networks (SIGMOD 2021) 🌟

### 3. About Coherence among Entities
__Global Coherence__
1. Relational Inference for Wikification (ACL 2013)
2. Robust Disambiguation of Named Entities in Text (EMNLP 2011)
3. Liege: Link Entities in Web Lists with Knowledge Base (KDD 2012)🌟
4. Collective entity linking in web text: A graph-based method (SIGIR 2011)
5. Collective Annotation of Wikipedia Entities in Web Text (KDD 2009)🌟
6. Local and Global Algorithms for Disambiguation to Wikipedia (ACL 2011)
7. Learning entity representation for entity disambiguation (ACL 2013)
8. Robust named entity disambiguation with random walks (Semantic Web 2018)
9. Graph ranking for collective named entity disambiguation (ACL 2014)
10. Personalized page rank for named entity disambiguation (ACL 2015)
11. Collective entity resolution with multi-focal attention (2016)
12. To link or not to link? a study on end-to-end tweet entity linking (NAACL 2013)
13. An entity-topic model for entity linking (EMNLP 2012)
14. Deep joint entity disambiguation with local neural attention (EMNLP 2017)
15. Improving entity linking by modeling latent relations between mentions (ACL 2018)
16. Neural Collective Entity Linking Based on Recurrent Random Walk Network Learning (IJCAI 2019), introduces external knowledge to model the semantic interdependence between different EL decisions
17. ELDEN: Improved Entity Linking using Densified Knowledge Graphs (NAACL-HLT 2018) [[Paper](https://www.aclweb.org/anthology/N18-1167.pdf)][[Code](https://github.com/priyaradhakrishnan0/ELDEN)], supervised EL system
18. KBPearl: A Knowledge Base Population System Supported by Joint Entity and Relation Linking (VLDB 2020) [[Paper](http://www.vldb.org/pvldb/vol13/p1035-lin.pdf)], with relation linking 🌟
19. Joint Embedding in Named Entity Linking on Sentence Level [[Paper](https://arxiv.org/pdf/2002.04936.pdf)]
20. Improving Entity Linking by Modeling Latent Relations between Mentions (ACL 2018) [[Paper](https://www.aclweb.org/anthology/P18-1148.pdf)]
21. Short text understanding through lexical-semantic analysis (ICDE 2015) (*Best Paper Award*) 🌟  [[Paper](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1056.5887&rep=rep1&type=pdf)]
22. A collective entity linking algorithm with parallel computing on large-scale knowledge base (The Journal of Supercomputing, 2020) [[Paper](https://link.springer.com/article/10.1007/s11227-019-03046-7)]
23. A Novel Path-based Entity Relatedness Measure for Efficient Collective Entity Linking (ISWC 2020)
24. Collective disambiguation in entity linking based on topic coherence in semantic graphs (2020) [[Paper](https://citius.usc.es/sites/default/files/publicacions_preprints/2019_kbs_v5_ans.pdf)]
25. Collective List-Only Entity Linking: A Graph-Based Approach (IEEE Access 2018) [[Paper](https://ieeexplore.ieee.org/document/8320777)]


__Relax the Global Coherence Assumption__
1. Joint entity linking with deep reinforcement learning (WWW 2019) [[Paper](https://arxiv.org/pdf/1902.00330.pdf)]
> Reinforcement learning, apply LSTM to be able to maintain long term memory for previous decisions.
2. Learning Dynamic Context Augmentation for Global Entity Linking (DCA, ACL 2019) [[Paper]](https://www.aclweb.org/anthology/D19-1026.pdf)
> Reinforcement learning, previous decisions are collected as dynamic context to improve the following predictions.
3. Global Entity Disambiguation with Pretrained Contextualized Embeddings of Words and Entities (2020) [[Paper]](https://www.researchgate.net/profile/Ikuya_Yamada/publication/340461536_Global_Entity_Disambiguation_with_Pretrained_Contextualized_Embeddings_of_Words_and_Entities/links/5e8b538fa6fdcca789fbc854/Global-Entity-Disambiguation-with-Pretrained-Contextualized-Embeddings-of-Words-and-Entities.pdf)
> * BERT+MLM.
> * Note: Paper 1,2,3 address ED as a sequential decision task that disambiguates mentions one by one, and uses words and already disambiguated entities to disambiguate new mentions.
4. Joint Learning of Local and Global Features for Entity Linking via Neural Networks (COLING 2016), [[Paper](https://www.aclweb.org/anthology/C16-1218.pdf)], CNN+RNN
> * Global-RNN utilizes convolutional neural networks to induce the representations for local contexts and takes advantage of recurrent neural networks to adaptively compress variable length sequences of predictions for global constraints.
5. Dynamic Graph Convolutional Networks for Entity Linking (WWW 2020) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3366423.3380192)]
> * Resorts to GNN to automatically decide the relevant linked nodes and then generate the global feature vector for every node.
> * Then a score function is proposed to directly utilize the feature to compute the ranking score and do not need other additional inference steps
6. Pair-Linking for Collective Entity Disambiguation: Two Could Be Better Than All (TKDE 2018) [[Paper](https://arxiv.org/pdf/1802.01074.pdf)]🌟 
> * With a demo: CoNEREL: Collective Information Extraction in News Articles (SIGIR 2018 demo) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3209978.3210165)]
8. CoNEREL: Collective Information Extraction in News Articles (SIGIR 2018, demo of Paper 6) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3209978.3210165)]
9. KBPearl: A Knowledge Base Population System Supported by Joint Entity and Relation Linking (VLDB 2020) 🌟
10. Joint Entity Linking for Web Tables with Hybrid Semantic Matching (ICCS 2020)
> * Converts table entity linking into a sequence decision problem and uses hybrid semantic features to disambiguate the mentions in web tables
11. Using Knowledge Base Semantics in Context-Aware Entity Linking (DocEng 2019) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3342558.3345393)]
> * Supervised CEL. Retained the sum, max@1,max@2 and max@3 as global contextual features, which can be seen as a kind of flexibility in selecting and aggregating the relatedness score.
12. High Quality Candidate Generation and Sequential Graph Attention Network for Entity Linking (WWW 2020) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3366423.3380146)] [[Code](https://github.com/fangzheng123/SGEL)] [[Video](https://www.youtube.com/watch?v=1A15SUukjM0&feature=youtu.be&list=PLJNwhMK_V7Ey1YFclcpycanlrwBXhCqYU)], BERT+SeqGAT
> * Graph-based models treat all candidate entities equally which may introduce much noise information
> * Sequence models can only observe previous referred entities, ignoring the relevance between the current mention and its subsequent entities
> * Contribution: (1) propose a multi-strategy based candidate generation method to generate high recall candidate sets; (2) design a Sequential Graph Attention Network (SeqGAT) which combines the advantages of graph and sequence methods
> * The same first author as "Joint entity linking with deep reinforcement learning (WWW 2019)"
13. LoG: a locally-global model for entity disambiguation (WWW 2021) [[Paper](https://link.springer.com/article/10.1007/s11280-020-00845-4)]
> * Derives meaningful local neighbors for each mention in a more linguistic way by utilizing dependency parse tree.
> * Locates key sentences in the document and then detect keywords at sentence level, and integrates the topical coherence with both mention neighbors and keywords for ED.
> * Employs neural ED approach which combines basic deep neural network model with Graph Attention Network (GAT) to utilize local features and global features.
14. Neural collective entity linking (COLING 2018) [[Paper](https://arxiv.org/pdf/1811.08603.pdf)]
> * Topical coherence only need to hold among neighboring mentions
15. TENET: Joint Entity and Relation Linking with Coherence Relaxation (SIGMOD 2021) 🌟

__Some related works__
1. Evaluating the Impact of Knowledge Graph Context on Entity Disambiguation Models (CIKM 2020, short) [[Paper]](https://arxiv.org/pdf/2008.05190.pdf)
> * Employ SPASQL to fetch triples of target entities and incorporate the triples as kg context in pre-trained ED models. DCA is used as baselines on the AIDA-CONLL dataset.
2. Attention-based Deep Reinforcement Learning Model for Pair-Wise Interaction Recommendation (ICISCE 2019)
> * Claim that the one-pass sequential decision should consider both positive feedback and negative feedback.


### 4. Entity Linking with Type Info

<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/EL_with_type.png" width="400"/>

1. Improving Entity Linking through Semantic Reinforced Entity Embeddings (ACL 2020) [[Paper]](https://www.aclweb.org/anthology/2020.acl-main.612.pdf) [[Data and Code]](https://github.com/fhou80/EntEmb/) [[Details]](https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/issues/1)
> * Fine-grained semantic types of entities can let the linking models learn contextual commonality about semantic relatedness.
> * fine-grained semantic words appear frequently as apposition (e.g., _Defense contractor_ Raytheon), coreference (e.g., the _company_) or anonymous mentions (e.g., _American defense firms_). These fine-grained types of entities can help capture local contexts and relations of entities.
2. Improving Entity Linking by Modeling Latent Entity Type Information (AAAI 2020) [[Paper](cuiqingcai.com/977.html)]
> * Conduct error analysis of the well known DeepED1 model (Ganea and Hofmann 2017) on the development set of AIDA-CoNLL, and found that more than half of their error cases fall into the category of type errors where the predicted entity’s type is different from the golden entity’s type.
> * Inject latent entity type information into the entity embeddings by modeling the immediate context surrounding the mention.
> * Apply pre-trained BERT to represent the entity context.
3. A joint model for entity analysis: Coreference, typing, and linking (TACL 2014)
4. Joint entity recognition and disambiguation (EMNLP 2015)
5. J-nerd: joint named entity recognition and disambiguation with rich linguistic features (TACL 2016)
> * Paper 3,4,5 integrate type information into the entity linking task by jointly NER+EL, which captures the mutual dependency between them using structured CRF. These methods mainly differ in the design of hand-engineered features.
6.  Joint learning of named entity recognition and entity linking. (ACL: Student Research Workshop, 2019)
> * Multi-task learning using learned features by extending Stack-LSTM.
> * Paper 3,4,5,6 rely on extensive annotation of the type of mentions
7. DeepType: Multilingual Entity Linking by Neural Type System Evolution (AAAI 2018) [[Paper](https://arxiv.org/pdf/1802.01021.pdf)]

### 5. Meta EL
Note: how to combine the outputs of multiple EL tools for providing a unified set of entity annotations?
1. Better Together - An Ensemble Learner for Combining the Results of Ready-made Entity Linking Systems (SAC 2020) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3341105.3373883)]
2. A Novel Ensemble Method for Named Entity Recognition and Disambiguation Based on Neural Network (ISWC 2018)
3. MicroNeel: Combining NLP Tools to Perform Named Entity Detection and Linking on Microposts (Final Workshop 7 December 2016, Naples. 2016)
4. Combining open source annotators for entity linking through weighted voting (SEM 2015)
5. Joint posterior revision of NLP annotations via ontological knowledge (IJCAI 2018) [[Paper](https://www.ijcai.org/Proceedings/2018/0600.pdf)] [[Slides](https://marcorospocher.com/files/slides/2018scc_slides.pdf)] [[Details](https://pikes.fbk.eu/jpark.html)] 🌟
6. (Extended Version of Paper 5) Knowledge-driven joint posterior revision of named entity classification and linking (Journal of Web Semantics, 2020) [[Paper](https://www.sciencedirect.com/science/article/pii/S1570826820300500)]
7. (Extended reading for Paper 5, same research group) An Ontology-Driven Probabilistic Soft Logic Approach to Improve NLP Entity Annotations (ISWC 2018) [[Slides](https://marcorospocher.com/files/slides/2018iswc_research_slides.pdf)]


### 6. Joint NER and EL

<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/joint%20NER%20and%20EL.png" width="400"/>

<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/joint_NER_EL.png" width="800"/>

1. Joint Learning of Named Entity Recognition and Entity Linking (ACL 2019) [[Paper](https://www.aclweb.org/anthology/P19-2026.pdf)] [[Notes 1](https://blog.csdn.net/m0_37991005/article/details/108936874)] [[Notes 2](http://blog.sciencenet.cn/blog-205121-1210999.html)] [[Notes 3](http://pelhans.com/2019/09/28/named_entity_recognition/#joint-learning-of-named-entity-recognition-and-entity-linking)] [[Notes 4](https://www.pianshen.com/article/96391996423/)] 
> * Multi-task learning of NER and EL based on Stack-LSTM approach.
> * Supervised EL system with learned features.
> * Future extension: training entity contextual embeddings and extend it to be cross-lingual.
2. Re-ranking for joint named-entity recognition and linking (CIKM 2013) [[Paper](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.398.9086&rep=rep1&type=pdf)]
> * The reranking model then chooses among the set of all possible mention and entity link labelings for the whole phrase to determine the best choice. It can use features for known relationships between the television channel ABC and the television program The_View to encourage these as outputs. For efficiency, we use the pipeline models to prune the set of all possible candidate mentions and entity links to a manageable size while maintaining high recall. The reranking model can then use more sophisticated features for collective classification over this pruned set.
> * Rely on existing NER tools. Only NER is beneficial to EL, not vice versa.
> * Hand-engineered features.
> * Uses a large number of heuristically obtained Noun phrase (NP) chunks and word n-grams as additional input to the EL stage.
3. To link or not to link? a study on end-to-end tweet entity linking (NAACL 2013)
> * Only suitable for short-text such as tweets.
4. Joint entity recognition and disambiguation (EMNLP 2015) [[Paper](https://www.aclweb.org/anthology/D15-1104.pdf)]
> * NER is beneficial to EL. EL is also beneficial to NER.
> * Supervised EL system.
> * Hand-engineered features.
5. J-nerd: joint named entity recognition and disambiguation with rich linguistic features (TACL 2016) [[Paper](https://www.aclweb.org/anthology/Q16-1016.pdf)] [[Code](http://download.mpi-inf.mpg.de/d5/tk/jnerd-tacl.zip)]
> * Supervised, non-linear probabilistic graphical model that captures mention spans, mention types, and the mapping of mentions to entities in a knowledge base. 
> * Hand-engineered features.
> * Relies on fully labeled training data where each tagged entity needs to have an NER and EL label.
6. A Joint Model for Entity Analysis: Coreference, Typing, and Linking (TACL 2014) [[Paper](https://www.aclweb.org/anthology/Q14-1037.pdf)] [[System](http://nlp.cs.berkeley.edu/projects/entity.shtml)] [[GitHub](https://github.com/gregdurrett/berkeley-entity)]
> * Joint learning of entity typing, EL, and coreference.
> * Hand-engineered features.
7. Contextualized End-to-End Neural Entity Linking [[Paper](https://arxiv.org/pdf/1911.03834.pdf)]
> * An end-to-end differentiable neural EL model that jointly performs MD and ED, based on BERT, while eliminating external knowledge so that we can study the impact of external knowledge to the EL model.
> * Other version: "YELM: End-to-End Contextualized Entity Linking" (2019) [[Paper](https://arxiv.org/pdf/1911.03834.pdf)]
8. Noise-robust Named Entity Understanding for Virtual Assistants [[Paper](https://arxiv.org/pdf/2005.14408.pdf)]
> * Combining NER and EL information in a joint reranking module for noisy spoken language queries in the context of a digital voice assistant, our proposed framework improves accuracy in both tasks.
9. End-to-End Neural Entity Linking (CoNLL 2018) [[Paper](https://www.aclweb.org/anthology/K18-1050.pdf)] [[Code](https://github.com/dalab/end2end_neural_el)] [[Notes 1](https://blog.csdn.net/u010960155/article/details/106387771)] [[Notes 2](http://pelhans.com/2019/02/22/entity_linking/#end-to-end-neural-entity-linking)]
> * The main idea is to consider all possible spans as potential mentions and learn contextual similarity scores over their entity candidates that are useful for both MD and ED decisions.
10. Lightweight Multilingual Entity Extraction and Linking (EMNLP 2017) [[Paper](https://dl.acm.org/doi/10.1145/3018661.3018724)] [[Code](https://github.com/yahoo/FEL)] 🌟

### 7. Unlinkable Mention Predication
__General__
1. No Noun Phrase Left Behind: Detecting and Typing Unlinkable Entities (EMNLP-ACL 2012)
> * Main idea: Train a classifier wuth features primarily derived from a timestamped corpus
> * Main contribution: usage patterns di er across time between in-KB entities and out-of-KB entities and they operationalize this idea by computing the best  t line (least-squares regression ) for usage over time. 
2. Entity Linking at Web Scale (AKBC-WEKEX 2012)
> * Explores handling these unlinkable entities over 3 steps: Detect Entities, Predict Types, Disambiguation
3. The Birth of Collective Memories: Analyzing Emerging Entities in Text streams (JASIST 2018)
> * Track entities that emerge in public discourse (unstructured text) to gain insights into how these are added to Wikipedia.

__Unsupervised__
1. Using encyclopedic knowledge for named entity disambiguation (2006) [[PDF](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/70.pdf)]
2. Nlpr_kbp in tac 2009 kbp track: A two-stage method to entity linking (TAC workshop 2009)
3. LCC approaches to knowledge base population at TAC 2010 (TAC workshop 2010)
4. Linking entities to a knowledge base with query expansion (EMNLP 2011)
5. LINDEN: Linking named entities with knowledge base via semantic knowledge (WWW 2012)
6. Linking named entities in tweets with knowledge base via user interest modeling (KDD 2013)
7. Tagme: On-the-fly annotation of short text fragments (by wikipedia entities) (CIKM 2010)
8. From names to entities using thematic context distance (CIKM 2011)
9. Mining evidences for named entity disambiguation (KDD 2013)
> * Paper 1-9: If the score of a mention is smaller than a NIL threshold, then this mention is predicted as unlinkable. The threshold is learned from the training data.
10. Novel Entity Discovery from Web Tables (WWW 2020) [[PDF](https://dl.acm.org/doi/pdf/10.1145/3366423.3380205)]
> * A feature-based method, the first endeavor on mining the unlinked cells in web tables.
> * Identifies not only out-of-KB (“novel”) information but also novel aliases for in-KB (“known”) entities
11. Exploring Multiple Feature Spaces for Novel Entity Discovery (AAAI 2016)
> Discover novel entities in news and Web data by exploring multiple feature spaces, including context, neural embedding, topical, query and lexical spaces
12. The Birth of Collective Memories: Analyzing Emerging Entities in Text streams (JASIST 69, 2018)
> * Track entities that emerge in public discourse to gain insights into how these are added to Wikipedia.
13. Knowledge-driven joint posterior revision of named entity classification and linking (Journal of Web Semantics, 2020) [[Paper](https://www.sciencedirect.com/science/article/pii/S1570826820300500)]

__Supervised__
1. NUS-I2R: Learning a combined system for entity linking (TAC workshop 2010)
3. LCC approaches to knowledge base population at TAC 2010 (TAC workshop 2010)
4. I2R-NUS-MSRA at TAC 2011: Entity linking (TAC workshop 2011)
5. Entity linking with effective acronym expansion, instance selection and topic modeling (IJCAI 2011)
6. Cross-lingual cross-document coreference with entity linking (TAC workshop 2011)
> Utilize the binary classification technique (such as SVM). Positive --> entity_top, Negative --> NIL.
2. Learning to link entities with knowledge base (NAACL 2010)
7. Local and global algorithms for disambiguation to wikipedia (ACL 2011)
> * Design some features for for unlinkable mention prediction, such as the score of the top-ranked candidate and whether the entity mention is detected by some NER as a named entity.
8. Entity disambiguation for knowledge base population (COLING 2010) [[Paper](https://www.cs.jhu.edu/~mdredze/publications/entity_linking_coling.pdf)]
9. HLTCOE efforts in entity linking at TAC KBP 2010 (TAC workshop 2011)
> * Incorporate the unlinkable mention prediction process into the entity ranking process. They added a NIL entity into the candidate entity set, and considered NIL as a distinct candidate.
10. A generative entity-mention model for linking entities with knowledge base (ACL 2011)
> * The model assumes that for the entity mention which refers to some specific entity, the probability of this entity mention generated by this specific entity’s model should be significantly higher than the probability of this mention generated by a general language model. 
11. No Noun Phrase Left Behind: Detecting and Typing Unlinkable Entities (EMNLP-CoNLL ’12)
> * Train a classifier with features primarily derived from a timestamped corpus.

### 8. Entity Embeddings (Pre-trained) and Entity Representation for EL
1. Wembedder: Wikidata entity embedding web service [[Intro](https://arxiv.org/pdf/1710.04099.pdf)] [[Github](https://github.com/fnielsen/wembedder)] [[Web service](https://tools.wmflabs.org/wembedder/)]
> * Web service: only the "most similar" service.
2. Pre-trained embeddings for Wikidata [[Link](https://torchbiggraph.readthedocs.io/en/latest/pretrained_embeddings.html)]
3. Pre-trained embeddings [[Link](http://139.129.163.161/index/toolkits)]
> * 100-dimention and 50-dimention, parsed by numpy.memmap. However, I can only read one float (instead of a vector) for each entity. No sure whether there is mistake.
4. EntEval: A Holistic Evaluation Benchmark for Entity Representations (EMNLP 2019) [[Paper](https://arxiv.org/abs/1909.00137)]

### 9. Entity Linking Evaluation Platform
1. Python command-line evaluation scripts for TAC [[GitHub](https://github.com/wikilinks/neleval)]

### 10. Multimodal Entity Linking
1. DRIN: Dynamic Relation Interactive Network for Multimodal Entity Linking (2023) [[Paper](https://arxiv.org/pdf/2310.05589v1.pdf)]
2. Multi-Grained Multimodal Interaction Network for Entity Linking (2023) [[Paper](https://arxiv.org/pdf/2307.09721v1.pdf)]
3. Generative Multimodal Entity Linking (Arxiv 2023) [[Paper](https://arxiv.org/abs/2306.12725)]


### 11. LLM and Entity Linking 🔥🔥🔥
1. Large language models struggle to learn long-tail knowledge (PMLR 2023) [[Paper](https://proceedings.mlr.press/v202/kandpal23a.html)]
2. Exploring the In-context Learning Ability of Large Language Model for Biomedical Concept Linking (Arxiv 2023) [[Paper](https://arxiv.org/abs/2307.01137)]
3. Instructed Language Models with Retrievers Are Powerful Entity Linkers (Arxiv 2023) [[Paper](https://arxiv.org/abs/2311.03250)]
4. Increasing Coverage and Precision of Textual Information in Multilingual Knowledge Graphs (Arxiv 2023) [[Paper](https://arxiv.org/pdf/2311.15781v1.pdf)]
5. Use Large Language Models for Named Entity Disambiguation in Academic Knowledge Graphs (EIMSS 2023) [[Paper]([https://arxiv.org/pdf/2311.15781v1.pdf](https://www.atlantis-press.com/proceedings/eimss-23/125991633))]



### 11. Datasets
1. Reddit Entity Linking Dataset [[Paper](https://arxiv.org/pdf/2101.01228.pdf)]
