## Named Entity Recognition, Entity Extraction and Entity Typing

### 📝 Surveys
1. Named Entity extraction for Knowledge Graphs: A Literature Overview (IEEE Access 2020) [[Paper](https://ieeexplore.ieee.org/abstract/document/8999622/)]
2. A survey of named entity recognition and classification [[Paper](https://nlp.cs.nyu.edu/sekine/papers/li07.pdf)]
3. A Survey on Deep Learning for Named Entity Recognition (TKDE 2018) [[Paper] (https://www.researchgate.net/profile/Aixin_Sun/publication/339990379_A_Survey_on_Deep_Learning_for_Named_Entity_Recognition/links/5e78581c299bf1892c021d50/A-Survey-on-Deep-Learning-for-Named-Entity-Recognition.pdf)] [[Official version](https://ieeexplore.ieee.org/abstract/document/9039685)]🌟

### 📝 Tutorials
1. https://cs230.stanford.edu/blog/namedentity/

### 📝 Research Papers

__General NER or Entity Typing__
1. Knowledge Vault: A Web-Scale Approach to Probabilistic Knowledge Fusion [Knowledge Vault, KDD 2014] 🌟
2. ClusType: Effective Entity Recognition and Typing by Relation Phrase-Based Clustering [ClusType, KDD2015] (Also Relation Clustering) coarse grained entity typing 🌟 
3. Named entity recognition with document-specific KB tag gazetteers (EMNLP 2015)
4. No Noun Phrase Left Behind: Detecting and Typing Unlinkable Entities [EMNLP-CoNLL 2012][[Paper](https://aclweb.org/anthology/D12-1082)]
5. TextCube: Automated Construction and Multidimensional Exploration (VLDB 2019) 🌟
6. Human-in-the-loop ML Systems for Entity Extraction (KDD 2019), regex+DL, weak label+active learning  🌟
7. Automated phrase mining from massive text corpora (TKDE 2018) 🌟
8. Predicting Named Entity Location Using Twitter (ICDE 2018) [[PDF](https://ieeexplore.ieee.org/document/8509245)] prediction of the entity city-level location 🌟
9. How to Invest my Time: Lessons from HITL Entity Extraction [[Presentation](https://www.kdd.org/kdd2019/accepted-papers/view/how-to-invest-my-time-lessons-from-hitl-entity-extraction), applied science track] (KDD 2019) 🌟
10. BOND: Bert-Assisted Open-Domain Named Entity Recognition with Distant Supervision (KDD 2020) 🌟 [[Paper](https://arxiv.org/pdf/2006.15509.pdf)] [[Code and Dataset](https://github.com/cliang1453/BOND)]
11. Adversarial Transfer for Named Entity Boundary Detection with Pointer Networks (IJCAI 2019) [[PDF](https://www.ijcai.org/Proceedings/2019/0702.pdf)]
12. Neural Chinese Named Entity Recognition via CNN-LSTM-CRF and Joint Training with Word Segmentation (WWW 2019)
13. Leverage Lexical Knowledge for Chinese Named Entity Recognition via Collaborative Graph Network (EMNLP 2019)
14. Mis-categorized entities detection [[Paper](https://link.springer.com/article/10.1007/s00778-021-00653-w)] (VLDBJ 2021) 🌟
15. Neural Named Entity Boundary Detection [[Paper](https://ieeexplore.ieee.org/document/9039695/)] (TKDE 2021) 🌟
16. Enhancing Temporal and Geographical Named Entity Recognition in Chinese Ancient Texts with External Time-series Knowledge Bases (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679917)]
17. Knowledge Graph Entity Typing with Curriculum Contrastive Learning (COLING 2025)
18. What can knowledge graph do for few-shot named entity recognition (Journal of Web Semantics 2025)

__Fine-grained NER or Entity Typing__
1. Label Noise Reduction in Entity Typing by Heterogeneous Partial-Label Embedding (PLE, KDD 2016) fine-grained entity typing
2. AFET: Automatic Fine-Grained Entity Typing byHierarchical Partial-Label Embedding (AFET, EMNLP 2016) fine-grained entity typing
3. Neural Joint Learning for Classifying Wikipedia Articles into Fine-Grained Named Entity Types (PACLIC, 2016)
4. Fine-Grained Named Entity Recognition using ELMo and Wikidata (2019) [[Paper]](https://arxiv.org/pdf/1904.10503.pdf)
5. Fine-grained Type Inference in Knowledge Graphs via Probabilistic and Tensor Factorization Methods (WWW 2019)

__Domain Specific NER__
1. A Hybrid Generative/Discriminative Model for Rapid Prototyping of Domain-Specific Named Entity Recognition (2019)
2. Learning Named Entity Tagger using Domain-Specific Dictionary (EMNLP 2018) [[Paper]](https://arxiv.org/pdf/1809.03599.pdf) [[Notes]](https://www.zhihu.com/question/294189189/answer/494208998) [[Code]](https://github.com/shangjingbo1226/AutoNER)

__Nested NER__

<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/nested_NER.png" width="400"/>

1. Nested Named Entity Recognition Revisited (NAACL-HLT 2018)
2. A Neural Layered Model for Nested Named Entity Recognition (NAACL-HLT 2018) [[Code](https://github.com/meizhiju/layered-bilstm-crf)]
3. Nested Named Entity Recognition (Stanford)
4. NNE: A Dataset for Nested Named Entity Recognition in English Newswire (ACL 2019)
5. Nested Named Entity Recognition via Second-best Sequence Learning and Decoding [[Paper](https://arxiv.org/pdf/1909.02250.pdf)]

__LLM for NER__ 🔥🔥🔥
1. GPT-NER: Named Entity Recognition via Large Language Models (Arxiv 2023, I think this is the first paper that brings LLM to NER) [[Paper](https://arxiv.org/abs/2304.10428)] [[Blog (in Chinese)](https://blog.csdn.net/HERODING23/article/details/130476395)]
2. Spacy-llm: Integrating LLMs into structured NLP pipelines [[Github](https://github.com/explosion/spacy-llm)]
3. Empirical Study of Zero-Shot NER with ChatGPT (Arxiv 2023) [[Paper](https://arxiv.org/abs/2310.10035)]
4. Self-Improving for Zero-Shot Named Entity Recognition with Large Language Models (Arxiv 2023, by the same team of paper 3) [[Paper](https://arxiv.org/pdf/2311.08921v1.pdf)]

### 🛠️ Awesome Tools/Repos 
1. BERT coarse-grained NER [[GitHub](https://github.com/kamalkraj/BERT-NER)]
2. BERT fine-grained NER [[GitHub](https://github.com/conv1d/bert-fine-grained-ner)]
3. CLUENER2020, fine-grained NER [[GitHub](https://github.com/CLUEbenchmark/CLUENER20200)]
4. Chinese fine-grained NER [[GitHub](https://github.com/sigamani/ner)]
5. Figer, fine-grained NER [[GitHub](https://github.com/xiaoling/figer)]
6. Legal, fine-grained NER [[GitHub](https://github.com/elenanereiss/Legal-Entity-Recognition)]
1. TagMe [[Python API](https://pypi.org/project/tagme/)] [[API](https://tagme.d4science.org/tagme/)] [[GitHub1](https://github.com/marcocor/tagme-python)] [[GitHub2](https://github.com/gammaliu/tagme)]
2. Stanford NER [[Link](https://nlp.stanford.edu/software/CRF-NER.html)]
3. DBpedia Spotlight [[Link](https://www.dbpedia-spotlight.org/)]
4. NLTK Tagger [[Link](https://www.nltk.org/book/ch05.html)]
5. SpaCy [[Link1](https://spacy.io/api/annotation#section-named-entities)] [[Link2](https://towardsdatascience.com/named-entity-recognition-with-nltk-and-spacy-8c4a7d88e7da)]
   > * spacy-llm [[Link](https://github.com/explosion/spacy-llm)]
7. EARL (including Relation Linking) [[Link](https://github.com/AskNowQA/EARL)]
8. Falcon (including Relatoin Linking) [[DBpedia version](https://github.com/AhmadSakor/falcon)] [[Wikidata version](https://github.com/SDM-TIB/falcon2.0)] 
9. MonkeyLearn [[Link](https://monkeylearn.com/blog/named-entity-recognition-python/)]
10. GERBIL - General Entity Annotator Benchmark [[Link](http://gerbil.aksw.org/gerbil/)]
11. PIKES [[Link](http://pikes.fbk.eu)]
