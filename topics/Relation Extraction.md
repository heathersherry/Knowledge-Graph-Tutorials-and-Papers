## Relation Extraction

### 📝 Tutorial
1. A SURVEY ON RELATION EXTRACTION (CMU) [[Slides](http://www.cs.cmu.edu/~nbach/papers/A-survey-on-Relation-Extraction-Slides.pdf)]
2. Relation Extraction: CSE 517: Natural Language Processing [[Slides](https://courses.cs.washington.edu/courses/cse517/13wi/slides/cse517wi13-RelationExtraction.pdf)]
3. Relation Extraction II: CSE 517: Natural Language Processing [[Slides](https://courses.cs.washington.edu/courses/cse517/13wi/slides/cse517wi13-RelationExtractionII.pdf)]

### 📝 Research Papers
__General topics__
1. CoType: Joint Extraction of Typed Entities and Relations with Knowledge Bases (CoType, WWW2017)[[Notes]](
https://blog.csdn.net/hqc888688/article/details/73559365)
2. Knowledge-Based Weak Supervision for Information Extraction of Overlapping Relations [[Code](http://aiweb.cs.washington.edu/ai/raphaelh/mr/)][[Slides](https://www.slideserve.com/anila/knowledge-based-weak-supervision-for-information-extraction-of-overlapping-relations)]
> * Recently, researchers have developed multi- instance learning algorithms to combat the noisy training data that can come from heuristic labeling, but their models assume relations are disjoint . for example they cannot extract the pair Founded(Jobs, Apple) and CEO-of(Jobs, Apple). This paper presents a novel approach for multi-instance learning with overlapping relations that combines a sentence-level extraction model with a simple, corpus-level component for aggregating the individual facts. 
3. Modeling missing data in distant supervision for information extraction (ACL2013) missing data problem(?)
4. Neural Relation Extraction with Selective Attention over Instances (ACL 2016) [[Paper](http://www.aclweb.org/anthology/P16-1200)][[Code](https://github.com/thunlp/OpenNRE)][[Blog](https://zhuanlan.zhihu.com/p/22666876)]
> * Fix the problem of distant supervised relation extraction
> * Employs CNN to embed the semantics of sentences, then builds sentence-level attention over multi- ple instances, which is expected to dynamically reduce the weights of those noisy instances (major contribution). Notes in group meeting.
5. Multi-instance Multi-label Learning for Relation Extraction (EMMLP-CoNLL 2012)[[Paper](https://www.aclweb.org/anthology/D12-1042)]
6. Snuba: Automating Weak Supervision to Label Training Data (VLDB 2019) 🌟
7. Improving Neural Relation Extraction with Implicit Mutual Relations [[Video](https://www.google.com/url?q=https://drive.google.com/open?id%3D1Ksh1lBwJ0V2nopiLoh-Uk5eofJW6uRrA&sa=D&ust=1587488616483000&usg=AFQjCNEPrROfm72JmChuKgls7cAo2fniOA)][[Slides](https://www.google.com/url?q=https://drive.google.com/open?id%3D1hIfhz0qfPu9p44kWfhhywj_D8EF9eGX5&sa=D&ust=1587488616483000&usg=AFQjCNFpDtYPPYI16sI05NBwoLqUt8jtog)][[Paper](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300b021/290300b021.pdf)] (ICDE 2020) 🌟
8. Snorkel: rapid training data creation with weak supervision (VLDBJ 2020) 🌟
9. Snorkel: Fast Training Set Generation for Information Extraction (SIGMOD 2017) 🌟
10. NERO: A Neural Rule Grounding Framework for Label-Efficient Relation Extraction (WWW 2020) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3366423.3380282)]
> * Explicitly exploit labeling rules over unmatched sentences as supervision for training better RE models
> * The Nero framework has two major modules: (1) The sentence-level relation classifier aims to learn the neural representations of sentences and classify which relation it talks about, which serves as the outcome of Nero. (2) The soft rule matcher: The key intuition behind our soft rule matcher is that the distances between rules and sentences can be modeled by simple cosine computations in a new space transformed from their neural representations (e.g. word embeddings), which can be learned by a contrastive loss. 
11. MCVAE: Margin-based Conditional Variational Autoencoder for Relation Classification and Pattern Generation (WWW 2019)
12. Semi-structured relation extraction (a series of woks conducted by the same author)
> * ZeroShotCeres: Zero-shot relation extraction from semi-structured webpages (ACL 2020)
> * OpenCeres: When open information extraction meets the semi-structured web (NAACL 2019)
> * Ceres: Distantly supervised relation extraction from the semi-structured web (VLDB 2018)
13. RECON: Relation Extraction using Knowledge Graph Context in a Graph Neural Network (WWW 2021)
14. Discovering Correlations between Sparse Features in Distant Supervision for Relation Extraction (WSDM 2019)
15. KnowPrompt: Knowledge-aware Prompt-tuning with Synergestic Optimization for Relation Extraction (WWW 2022) [[Paper](https://arxiv.org/abs/2104.07650)] [[Code](https://github.com/zjunlp/KnowPrompt)]
> * [Related works](https://github.com/thunlp/PromptPapers)
16. Document-Level Relation Extraction Based on Heterogeneous Graph Reasoning (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679899)]
17. Topic-Oriented Open Relation Extraction with A Priori Seed Generation (EMNLP 2024) [[Paper](https://aclanthology.org/2024.emnlp-main.766.pdf)]
18. Improving Data Annotation for Low-Resource Relation Extraction with Logical Rule-Augmented Collaborative Language Models (NAACL 2025) [[Paper](https://aclanthology.org/2025.naacl-long.70/)]
19. Analyzing the Influence of Knowledge Graph Information on Relation Extraction (ESWC 2025) [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-94575-5_25)]
20. Task-Oriented Dynamic Knowledge Distillation for Continuous Few-Shot Relation Extraction (Knowledge Base System 2025) [[Paper](https://www.sciencedirect.com/science/article/pii/S0950705125009591)]
21. End-to-end Learning of Logical Rules for Enhancing Document-level Relation Extraction (ACL 2024) [[Paper](https://aclanthology.org/anthology-files/pdf/acl/2024.acl-long.391.pdf)]
22. Document Level Relationship Extraction based on context feature enhancement (Pattern Recognition Letters 2025) [[Paper](https://www.sciencedirect.com/science/article/pii/S0167865525002582)]
23. Document-Level Relation Extraction with Global Relations and Entity Pair Reasoning (ACL 2025 Findings) [[Paper](https://aclanthology.org/2025.findings-acl.1002/)]

__LLM for RE__ 🔥🔥🔥
1. Revisiting Relation Extraction in the era of Large Language Models (ACL 2023) [[Paper](https://aclanthology.org/2023.acl-long.868.pdf)]
2. Learn or Recall? Revisiting Incremental Learning with Pre-trained Language Models (Arxiv, Dec 2023) [[Paper](https://arxiv.org/pdf/2312.07887v1.pdf)]
3. Taiyi: A Bilingual Fine-Tuned Large Language Model for Diverse Biomedical Tasks (Arxiv, Nov 2023) [[Paper](https://arxiv.org/vc/arxiv/papers/2311/2311.11608v1.pdf)]
> * Datasets: a comprehensive collection of 140 existing biomedical text mining datasets (38 Chinese datasets and 102 English datasets)
> * Tasks: named entity recognition, relation extraction, text classification, question answering tasks
4. Unleashing the Power of Large Language Models in Zero-shot Relation Extraction via Self-Prompting (EMNLP 2024) [[Paper](https://aclanthology.org/2024.findings-emnlp.769.pdf)]

### Datasets, Benchmarks, and Platform for Evaluation
1. __(Dataset) CoNLL__: A Linear Programming Formulation for Global Inference in Natural Language Tasks (ACL 2004)
2. __(Dataset) NYT__: Modeling relations and their mentions without labeled text (ECML/PKDD 2010)
3. __(Platform)__: Benchmarks for RE [[Link](https://paperswithcode.com/task/relation-extraction/latest)]
4. __(Benchmark)__: NCRE: A Benchmark for Document-level Nominal Compound Relation Extraction (COLING 2025) [[Paper](https://aclanthology.org/2025.coling-main.701/)]

### 💬 Interesting Blogs and Discussions
1. 基于神经网络的实体识别和关系抽取联合学习 (in Chinese)[[Link](https://www.cnblogs.com/robert-dlut/p/7710735.html)]
