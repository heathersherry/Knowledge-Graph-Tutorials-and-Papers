## Domain-Specific Knowledge Bases

### Tutorials and Surveys
1. Constructing Domain-specific Knowledge Graphs (AAAI 2018) [[Tutorial](https://usc-isi-i2.github.io/AAAI18Tutorial/)]
2. Domain-specific Knowledge Graphs: A survey (2020) [[Paper](https://arxiv.org/pdf/2011.00235.pdf)]

### Papers about General Domain-Specific KB Construction and Refinement
1. Towards the Completion of a Domain-Specific Knowledge Base with Emerging Query Terms [[PDF](https://ieeexplore.ieee.org/abstract/document/8731487)] (ICDE 2019) 🌟 
2. Demonstrating Spindra: A Geographic Knowledge Graph Management System [[PDF](http://www.public.asu.edu/~jiayu2/geospark/publication/spindra-icde2019-demo.pdf), demo] (ICDE 2019) 🌟 
3. Domain Specific Knowledge Graphs as a Service to the Public (KDD 2020, Applied Data Science Track) 🌟 
4. Probase: A Probabilistic Taxonomy for Text Understanding (SIGMOD 2012)🌟
> ProBase : Microsoft Conceptual Graph
> * iterative learning algorithm for extraction and taxonomy construction algorithm
> * a probabilistic framework
> * largest general-purpose taxonomy fully automatically constructed 
5. Semantic Enrichment of Data for AI Applications (DEEM 2021)

### Papers about Different Tasks on Domain-Specific KBs
#### Domain Specific NER
1. Learning Named Entity Tagger using Domain-Specific Dictionary [[Paper](https://arxiv.org/pdf/1809.03599.pdf)] [[Notes](https://blog.csdn.net/Rock_y/article/details/108900106)]
2. A Hybrid Generative/Discriminative Model for Rapid Prototyping of Domain-Specific Named Entity Recognition [[Paper](https://pdfs.semanticscholar.org/d14d/ece78249b2039aa748bf3c7381653224d345.pdf)]

#### Domain Specific EL
1. SHINE+: A General Framework for Domain-Specific Entity Linking with Heterogeneous Information Networks (TKDE 2018) 🌟
2. A Semantic Approach for Entity Linking by Diverse Knowledge Integration incorporating Role-Based Chunking ((ICCIDS 2019)
3. Towards Linking Camouflaged Descriptions to Implicit Products in E-commerce (SIGIR 2020) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3397271.3401067)]
4. Medical Entity Disambiguation using Graph Neural Networks (SIGMOD 2021) 🌟

#### Taxonomies of Domain Specific KBs
1. TiFi: Taxonomy Induction for Fictional Domains? (WWW 2019)

## KBs in Specific Domains

### Product KBs
__Keynotes and Tutorials__
1. Amazon Product Graph [[Slides](http://lunadong.com/talks/PG.pdf)]
2. Self-Driving Product Understanding for Thousands of Categories (By Luna Dong, Keynote at Knowledge Graphs and E-commerce Workshop, San Diego, CA, August 2020) [[Slides](http://lunadong.com/talks/SelfDrivingBG.pptx)]
3. Building a Broad Knowledge Graph for Products (By Luna Dong, Keynote at IEEE International Conference on Data Engineering (ICDE), Macau, China, April 2019) [[Slides](http://lunadong.com/talks/BG.pdf)]

__Papers__
1. AutoKnow: Self-Driving Knowledge Collection for Products of Thousands of Types (KDD 2020, Applied Data Science Track) [[Paper](https://arxiv.org/pdf/2006.13473.pdf)]🌟
2. GoodsKG - a Product Knowledge Graph Project [[GitHub](https://github.com/liuhuanyong/ProductKnowledgeGraph)]
3. AliCoCo: Alibaba E-commerce Cognitive Concept Net (SIGMOD 2020 Industry Track) [[Paper](https://arxiv.org/pdf/2003.13230.pdf)] [[Github](https://github.com/alicogintel/AliCoCo)]🌟
4. Product Knowledge Graph Embedding for E-commerce (WSDM 2020) [[Paper](https://arxiv.org/pdf/1911.12481.pdf)]🌟
5. Towards Knowledge-Based Personalized Product Description Generation in E-commerce [[Paper](https://arxiv.org/pdf/1903.12457.pdf), applied science track] (KDD 2019) 🌟
6. TXtract: Taxonomy-aware knowledge extraction for thousands of product categories (ACL 2020)
7. Automatic validation of textual attribute values in eCommerce Catalog by learning with limited labeled data (KDD 2020) 🌟
8. Octet: Online catalog taxonomy enrichment with self-supervision (KDD 2020) 🌟
9. OpenTag: Open attribute value extraction from product profiles (KDD 2018) 🌟
10. DEXTER: Large-scale discovery and extraction of product specifications on the Web (VLDB 2016) 🌟
11. P-Companion: A principled framework for diversified complementary product recommendation (CIKM 2020)
12. J-Recs: Principled and scalable recommendation justification (ICDM 2020)
13. PAM: Understanding Product Images in Cross Product Category Attribute Extraction (KDD 2021) [[Paper](https://arxiv.org/pdf/2106.04630.pdf)]
14. AliCoCo2: Commonsense Knowledge Extraction, Representation and Application in E-commerce (KDD 2021) 🌟
15. AliCG : Alibaba Conceptual Graph for Semantic Search (KDD 2021) 🌟
16. AliMe KG : Alibaba domain knowledge graph in E-commerce (CIKM 2020)
17. Embedding-based Product Retrieval in Taobao Search (KDD 2021) [[Paper](https://arxiv.org/pdf/2106.09297.pdf)] 🌟
18. Product Knowledge Graph Embedding for E-commerce (WSDM 2020) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3336191.3371778)]

__Datasets__
1.  Web Data Commons - Gold Standard for Product Matching and Product Feature Extraction [[Link](http://webdatacommons.org/productcorpus/)]

### Meidcal KBs
__Papers__

👉 Note: Medical entity linking is also referred to as medical concept normalization (MCN)
1. MedPath: Augmenting Health Risk Prediction via Medical Knowledge Paths (WWW 2021)
> * Personalized KG to provided personalized prediction and explicit reasoning.
> * The major idea is borrowed from MHGRN (multi-hop graph): Scalable Multi-Hop Relational Reasoning for Knowledge-Aware Question Answering (EMNLP 2020) [[Paper](https://arxiv.org/pdf/2005.00646.pdf)] [[Notes in Chinese](https://blog.csdn.net/ld326/article/details/114049909)]
3. Medical Entity Disambiguation using Graph Neural Networks (SIGMOD 2021) 🌟
> * This work introduces `ED-GNN` based on three representative GNNs (GraphSAGE, R-GCN, and MAGNN) for Medical ED. 
> * There are two optimization techniques: (1) a novel strategy to represent entities mentioned in text snippets as a query graph; (2) an effective negative sampling strategy.
4. Property Graph Schema Optimization for Domain-Specific Knowledge Graphs (ICDE 2021) 🌟 
5. MEDTO: Medical Data to Ontology Matching Using Hybrid Graph Neural Networks (KDD 2021) 🌟
6. DETERRENT: Knowledge Guided Graph Attention Network for Detecting Healthcare Misinformation (KDD 2020) 🌟 [[Paper](http://pike.psu.edu/publications/kdd20-deterrent.pdf)] [[GitHub](https://github.com/cuilimeng/DETERRENT)] `Healthcare Misinformation Detection`
> * A novel problem of explainable healthcare misinformation detection (from the web) by leveraging medical knowledge graph to better capture the high-order relations between entities.
> * RGCN (with attention) for KG reasoning + text encoer of articles = learn the representation for each earticle, then formulate a classification problem to distinguish if a news is fake.
> * The support KG: KnowLife: a versatile approach for constructing a large knowledge graph for biomedical sciences [[Paper](https://bmcbioinformatics.biomedcentral.com/track/pdf/10.1186/s12859-015-0549-5.pdf)] [[Website](http://knowlife.mpi-inf.mpg.de)]
> * Similar basic code (text+GRU+RGCN): Learning to Update Knowledge Graphs by Reading News (EMNLP 2019) [[GitHub](https://github.com/esddse/GUpdater)]

__Datasets__
1. PubMed
2. MDX [[Link](https://www.ibm.com/products/micromedex-with-watson)]
3. MIMIC-III [[Reference](https://www.nature.com/articles/sdata201635)]
4. Bio CDR [[Reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4860626/)]
5. NCBI [[Reference](https://pubmed.ncbi.nlm.nih.gov/24393765/)], NCBID [[Reference](https://www.ncbi.nlm.nih.gov/CBBresearch/Dogan/DISEASE/)]
6. ShARe [[Reference](https://aclanthology.org/S14-2007.pdf)]
7. BioCreative [[Reference](https://biocreative.bioinformatics.udel.edu/resources/corpora/biocreative-v-cdr-corpus/)]
8. Summary from NormCo [[Github](https://github.com/IBM/aihn-ucsd/tree/master/NormCo-deep-disease-normalization)]
9. Datasets provided by [[MedType](https://github.com/svjan5/medtype)]: [[WikiMed](https://drive.google.com/u/0/uc?export=download&confirm=seZN&id=16suJCinjfYhw1u1S-gPFmGFQZD331u7I)] and [[PubMedDS](https://drive.google.com/u/0/uc?export=download&confirm=kB20&id=16mEFpCHhFGuQ7zYRAp2PP3XbAFq9MwoM)]
10. Unified Medical Language System (UMLS): 4.2 million biomedical concepts, with 127 types
> * There is a UMLS Semantic Network for concept mapping to semantic types?
11. MedMetions [[Reference](https://arxiv.org/pdf/1902.09476.pdf)]


__Tools__
1. `BioBERT for NER` BioBERT: a pre-trained biomedical language representation model for biomedical text mining [[Paper](https://arxiv.org/ftp/arxiv/papers/1901/1901.08746.pdf)] [[GitHub](https://github.com/dmis-lab/biobert)]
2. `DeepMatcher for EM`: Deep Learning for Entity Matching: A Design Space Exploration (SIGMOD 2018) [[PDF](http://pages.cs.wisc.edu/~anhai/papers1/deepmatcher-sigmod18.pdf)] [[Code and Data](https://github.com/anhaidgroup/deepmatcher)] 🌟
3. `NCEL for EL`: Neural Collective Entity Linking (COLING 2018) [[Paper](https://arxiv.org/pdf/1811.08603.pdf)] [[Github](https://github.com/TaoMiner/NCEL)]
4. `SciSpacy (as neural med-linker)`: SciSpaCy： Fast and Robust Models for Biomedical Natural Language Processing (arxiv 2019)  [[GitHub](https://allenai.github.io/scispacy/)]
5. `cTAKES for medical entity linker` (map named entities to UMLS concepts)  [[Reference](https://cwiki.apache.org/confluence/display/CTAKES/cTAKES+4.0+-+LVG)]
6. `Quick-UMLS for medical entity linker`
7. `MetaMap for medical entity linker` (map biomedical mentions in text to UMLS concepts) [[Tool](https://lhncbc.nlm.nih.gov/ii/tools/MetaMap.html)]
> * `MetaMapLite`: reimplements baisc MetaMap with an additional emphasis on real-time processing and competitive performance [[Tool](https://lhncbc.nlm.nih.gov/ii/tools/MetaMap/Docs/README_MetaMapLite_3.6.html)]
8. `QuickUMLS`


__People__
1. Fatma Özcan [[DBLP](https://dblp.org/pid/o/FatmaOzcan.html)]
2. Lei Chuan [[Website](https://leichuan.github.io/publications/)]

### Personalized KB
1. Personalized Knowledge Graph Summarization: From the Cloud to Your Pocket (ICDM 2019 Best Paper) [[Paper](https://ieeexplore.ieee.org/document/8970788)]
> * Knapsack, submodula objective function,  (1 − {1}{e})-approximation algorithm
3. What is Normal, What is Strange, and What is Missing in a Knowledge Graph: Unified Characterization via Inductive Summarization (WWW 2020) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3366423.3380189)]

### Event KGs
1. Searching News Articles Using an Event Knowledge Graph Leveraged by Wikidata (WWW 2019) [[Paper](https://arxiv.org/pdf/1904.05557.pdf)]
2. NewsLink: Empowering Intuitive News Search with Knowledge Graphs (ICDE 2021)
3. ASER: A Large-scale Eventuality Knowledge Graph (WWW 2020) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3366423.3380107)] [[Code](https://github.com/HKUST-KnowComp/ASER)]

### Opinion Graphs
1. Constructing Explainable Opinion Graphs from Reviews (WWW 2021) [[Paper](https://arxiv.org/pdf/2006.00119.pdf)] [[Code](https://github.com/megagonlabs/explainit)]

### Others
1. Knowledge-aware Assessment of Severity of Suicide Risk for Early Intervention (WWW 2019)
2. FoodKG: A Semantics-Driven Knowledge Graph for Food Recommendation (ISWC 2019) [[Github](https://foodkg.github.io/foodkg.html)]

