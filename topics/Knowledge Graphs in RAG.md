## Knowledge Graphs in RAG (Retrieval Augmented Generation)

```
Note: The definition of KGs may be different in each RAG work. Usually there are 3 types of KGs.
1. Eentity-level KG, while each node represents an entitiy or a concept, and each link represents the semantic relation or self-defined relation between a pair of nodes (e.g., whether they are extracted from the same document). `fine-grained`
2. Metadata-level KG, while each node represents the metadata of a document chunk (e.g., the topic or description of the document chunk), and each link represents self-defined relation between a pair of nodes (e.g., the correlation bewteen the topics). `middle-grained`
3. Document chunk-level KG, while each node represents a document chunk, and each link represents the context sequence of the nodes. `coarse-grained` 
* This is aligned with the of LLM+KG inference:
> Compared with neural networks the captures complex distribution of knowledge, graphs of entities may not be scientifically optimal as a knowledge model.
> But graphs can record the connection among document chunks or the tapologies of entity concepts, to facilitate the *retrieval sequence* of llm inference. 
```

### 📝 Traditional RAG Frameworks 

It is highly recommended that you understand the basic concepts of RAG, and get familiar with one or more of the following frameworks first.

#### RAG surveys
1. A Survey on Multimodal Retrieval-Augmented Generation (Arxiv 2025) [[Paper](https://arxiv.org/pdf/2504.08748)] [[Discussion (Chinese)](https://cloud.tencent.com/developer/news/2441489)] `MRAG`
> * It summerizes the development of MRAG1.0, MRAG2.0 and MRAG3.0, with discussion about the extraction, parsing, planning and retrival.
2. Retrieving Multimodal Information for Augmented Generation: A Survey (Arxiv 2023) [[Paper](https://arxiv.org/pdf/2504.08748)] `MRAG`
3. Ask in Any Modality: A Comprehensive Survey on Multimodal Retrieval-Augmented Generation (Arxiv 2025) [[Paper](https://arxiv.org/abs/2502.08826)] [[Github](https://github.com/llm-lab-org/Multimodal-RAG-Survey)] [[Discussion (Chinese)](https://zhuanlan.zhihu.com/p/29346473723)] `MRAG`

#### The popular RAG works
1. AnythingLLM (RAG + AI Agent) [[Github](https://github.com/Mintplex-Labs/anything-llm/blob/master/README.md)] - Default VDB: LanceDB
2. MaxKB [[Github](https://github.com/1Panel-dev/MaxKB)] - Default VDB: PostgreSQL + pgvector
3. RagFlow (streamlined RAG workflow based on deep document understanding) [[Github](https://github.com/infiniflow/ragflow)] - Default VDB: Elasticsearch
4. Dify (agentic AI workflow, RAG pipeline, agent capabilities, model management, ...) [[Github](https://github.com/langgenius/dify/)] - VDB: Elasticsearch / TiDB? ([[can refer to yaml](https://github.com/langgenius/dify/blob/main/docker/docker-compose.yaml)])
5. FastGPT (data processing, RAG retrieval, and visual AI workflow orchestration) [[Github](https://github.com/labring/FastGPT/blob/main/README_en.md)] - VDB: MongoDB + PostgreSQL (PG Vector)/Milvus
6. LangChain-Chatchat/Langchain-ChatGLM (local knowledge based LLM RAG and Agent) [[Github](https://github.com/chatchat-space/Langchain-Chatchat)] Default DB:sqlite?
7. QAnything (a local knowledge base question-answering system designed to support a wide range of file formats and databases, from 网易有道速读) [[Github](https://github.com/netease-youdao/QAnything)]
8. Quivr (Opiniated RAG) [[Github](https://github.com/QuivrHQ/quivr)] - Any Vectorstore: PGVector, Faiss
9. RAG-GPT [[GitHub](https://github.com/gpt-open/rag-gpt)]
10. Verba - [[GitHub](https://github.com/weaviate/Verba)] VDB：Weaviate
11. FlashRAG：6 pre-processed benchmark RAG datasets and 16 state-of-the-art RAG algorithms [[GitHub](https://github.com/RUC-NLPIR/FlashRAG)] Support multimodal RAG
12. kotaemon: An open-source clean & customizable RAG UI for chatting with your documents. [[GitHub](https://github.com/Cinnamon/kotaemon)]
13. RAGapp：Agentic RAG, Built using LlamaIndex [[GitHub](https://github.com/ragapp/ragapp)]
14. TurboRAG: KVCache+ Chunked text [[Paper](https://arxiv.org/abs/2410.07590)] [[GitHub](https://github.com/MooreThreads/TurboRAG)]
15. Ten: a voice agent framework to create conversational AI. TEN also facilitates the integration of AI with audio-visual tools, databases, monitoring systems, RAG, and more. [[GitHub](https://github.com/TEN-framework/ten_framework)]
16. AutoRAG: An Open-Source Framework for RAG Evaluation & Optimization with AutoML-Style Automation [[Github](https://github.com/Marker-Inc-Korea/AutoRAG)]
17. All RAG Techniques [[Github](https://github.com/liu673/rag-all-techniques)] - A series of simple and clear demos!! Strongly recommended.
18. Sycamore: AI-powered document processing engine for ETL, RAG, LLM-based applications, and analytics on unstructured data. [[Github](https://github.com/aryn-ai/sycamore/tree/main)]

#### Some good discussions/surveys/tutorials/blogs for beginners to know more about RAG and Graph RAG
1. Retrieval-Augmented Generation for Large Language Models: A Survey (Arxiv, Mar 2024) [[Paper](https://arxiv.org/pdf/2312.10997)] [[Notes for OpenRAG Base](https://mp.weixin.qq.com/s/MZ4jSH1torrEpYGTLTkiEw)]
2. Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks (NeurIPS 2020) [[Paper](https://arxiv.org/pdf/2005.11401.pdf)]
3. A Survey of Graph Retrieval-Augmented Generation for Customized Large Language Models (Arxiv, Jan 2025) [[Paper](https://github.com/DEEP-PolyU/Awesome-GraphRAG)]
> My thoughts!:
> * This may be different from multi-modal RAG, where the context is in multiple modalities (e.g., image, text, video, ...) represented as embedding, and the query is based on fuzzy serach in vector db. If we need to query the knowledge in KGs, we need to rely on other query engine, such as SPAEQL on graphs.
> * Graph RAG/KAG may be more valuable in domain-specific area.
> * However, although the evaluation results on research benchmarks of multi-hop QA proves that KAG works, I am still wondering whether KAG really works in real-world scenarios, since building accurate domain-specific KG is very costly. Purely employing the exisiting information extraction methods (e.g., various tools for OpenIE) cannot output a KG with 100% correct and reliable knowledge, which may lead to hallusiciasion as well. Maybe the KAG work (Arxiv 2024) is a good example to start this research, since it successfully applied KAG to two professional knowledge Q&A tasks of the industrial downstream tasks in the Ant Group.
> * The keypoint of Graph RAG/KAG should be **the wiseful integration** of the benefits of unstructured information and structured information.
4. Knowledge Graph RAG Query Engine [[Link](https://docs.llamaindex.ai/en/stable/examples/query_engine/knowledge_graph_rag_query_engine.html)]
5. GraphRAG: Unlocking LLM discovery on narrative private data (Feb 2024, Microsoft) [[Link](https://www.microsoft.com/en-us/research/blog/graphrag-unlocking-llm-discovery-on-narrative-private-data/)]
6. Going Meta - Ep 22: RAG with Knowledge Graphs (from Neo4j) [[YouTube](https://www.youtube.com/watch?v=9DxwgIKVSHY)]
7. A very clear blog (in Chinese) to demonstrate Graph RAG: 7 种查询策略教你用好 Graph RAG 探索知识图谱 [[Blog](https://www.cnblogs.com/nebulagraph/p/17882072.html)], which also provides valuable references:
> * Graph RAG LlamaIndex Workshop：[[Blog](https://colab.research.google.com/drive/1tLjOg2ZQuIClfuWrAC2LdiZHCov8oUbs?usp=sharing)]
> * Knowledge Graph Index：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/index_structs/knowledge_graph/KnowledgeGraphDemo.html#knowledge-graph-index)]
> * Knowledge Graph Query Engine：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/query_engine/knowledge_graph_query_engine.html)]
> * Knowledge Graph RAG Query Engine：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/query_engine/knowledge_graph_rag_query_engine.html)]
> * Custom Retriever combining KG Index and VectorStore Index：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/index_structs/knowledge_graph/KnowledgeGraphIndex_vs_VectorStoreIndex_vs_CustomIndex_combined.html)]
> * LlamaIndex Webinar: Graph Databases, Knowledge Graphs, and RAG with Wey (NebulaGraph)：[[Link](https://www.youtube.com/watch?v=bPoNCkjDmco)]
> * Enhancing Large Language Models with Knowledge Graphs: The Role of Graph Algorithms
8. ActiveRAG (a new topic!) [[Notes in Chinese](https://mp.weixin.qq.com/s/K8V4z4e2ziJA1wfiCAxq_g)]

### 📝 KG-RAG, or GraphRAG
```
Based on the granularity of KGs, we classify the Graph RAG works into the following two types.
1. Works that use Coarse-grained KG
* These works first construct a KG based on input documents, then query or summerize on the KG. They usually require KG construction.
* Note: The definitions of nodes and edges of "KG" vary in different works. The nodes may be entities, nouns, document metadata, or document chunk summary; while the edges may be the semantic relations bewteen the nodes, or self-defined relations such as "co-occurrence in the same document chunk" or "appeared in the same document".
2. Works that use Fine-grained KG
* These works conduct query or reasoning on predifinded external graph (usually as input). They do not require KG construction.
```
#### (1) Overview, Surveys and Tutorials
1. LEGO-GraphRAG: Modularizing Graph-based Retrieval-Augmented Generation for Design Space Exploration (VLDB 2025) [[Paper](https://vldb.org/pvldb/volumes/18/paper/LEGO-GraphRAG%3A%20Modularizing%20Graph-based%20Retrieval-Augmented%20Generation%20for%20Design%20Space%20Exploration)] 🌟
2. Graph Retrieval-Augmented Generation: A Survey (Arxiv, Aug 2024; Accepted in ACM Transactions on Information Systems 2025) [[Paper](https://arxiv.org/pdf/2408.08921)]
3. Graph-based Approaches and Functionalities in Retrieval-Augmented Generation: A Comprehensive Survey (Arxiv, Jan 2026) [[Paper](https://arxiv.org/pdf/2504.10499)]
<img width="871" height="324" alt="Screenshot 2026-01-26 at 4 45 00 PM" src="https://github.com/user-attachments/assets/9664a92f-0574-47c7-a87d-400a42fc25ae" />
5. A Survey of Graph Retrieval-Augmented Generation for Customized Large Language Models (Arxiv, Jan 2025) [[Paper](https://arxiv.org/abs/2501.13958)]

#### (2) Coarse-grained KG

1. A good work for beginners: Convert any Corpus of Text into a Graph of Knowledge [[Github](https://github.com/rahulnyk/knowledge_graph)] 🔥🔥🔥
2. **GraphRAG (Microsoft)**: From Local to Global: A Graph RAG Approach to Query-Focused Summarization (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2404.16130)] [[GitHub](https://github.com/microsoft/graphrag)]
> * The main target is to solve a query focused summarization (QFS) task, rather than an explicit retrieval task. Therefore the goal of knowledge extraction and graph construction is to group the closely related entity entities, but not to build a perfect knowledge graph.
> * No reasoning or path finding, just community detection!
> * Advanced: **LazyGraphRAG**, which defers LLM use (not in the extraction part, but only in the query part) and dramatically increase the efficiency of answer generation. [[Source](https://www.microsoft.com/en-us/research/blog/lazygraphrag-setting-a-new-standard-for-quality-and-cost/)] [[Discussion (Chinese)](https://mp.weixin.qq.com/s?__biz=MzI3ODE5Mzc1Ng==&mid=2247493514&idx=1&sn=588c7388d247fc34771c8ab76aa0f2ce&scene=21#wechat_redirect)]
> * GraphRAG-Local-UI/GraphRAG-Ollama-UI,  an adaptation of Microsoft's GraphRAG, tailored to support local models and featuring a comprehensive interactive user interface ecosystem. [[GitHub](https://github.com/severian42/GraphRAG-Local-UI)] 🔥
4. **RAPTOR**: Recursive Abstractive Processing for Tree-Organized Retrieval (ICLR 2024) [[Paper](https://arxiv.org/pdf/2401.18059)] `hybrid search on graph`
5. **KGP**: Knowledge Graph Prompting for Multi-Document Question Answering (AAAI 2024) [[Paper](https://arxiv.org/pdf/2308.11730)] `graph query based on KNN`
6. **EraRAG**: Efficient and Incremental Retrieval-Augmented Generation for Growing Corpora (Arxiv 2025 June) [[Paper](https://arxiv.org/pdf/2506.20963)] `incremental update of the graph`
7. **E^2GraphRAG**: Streamlining Graph-based RAG for High Efficiency and Effectiveness (Arxiv 2025 May) [[Paper](https://arxiv.org/pdf/2505.24226)] `efficient search on the graph`
8. **GRAG**: Graph Retrieval-Augmented Generation (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2405.16506)] `text graph`
9. **GNN-RAG**: Graph Neural Retrieval for Large Language Model Reasoning (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2405.20139)]

#### (3) Fine-grained KG

1. **ToG**: Think-on-Graph: Deep and Responsible Reasoning of Large Language Model on Knowledge Graph (ICLR 2024) [[Paper](https://arxiv.org/pdf/2307.07697)] 🔥
> * Very good motivation of why using KG reasoning instead of LLM inference + graph query.
2. **ToG 2.0**: Think-on-Graph 2.0: Deep and Faithful Large Language Model Reasoning with Knowledge-guided Retrieval Augmented Generation (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2407.10805)]
> * Provides more pruning strategies for ToG.
3. **RoG**: Reasoning on Graphs: Faithful and Interpretable Large Language Model Reasoning (ICLR 2024) [[Paper](https://openreview.net/forum?id=ZGNWW7xZ6Q)] 🔥
4. **PoG**: Paths-over-graph: Knowledge graph empowered large language model reasoning (WWW 2025) [[Github](https://github.com/SteveTANTAN/PoG)]
6. **DALK**: Dynamic Co-Augmentation of LLMs and KG to answer Alzheimer's Disease Questions with Scientific Literature  (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2405.04819)]
7. **HippoRAG**: Neurobiologically Inspired Long-Term Memory for Large Language Models [[Paper](https://arxiv.org/pdf/2405.14831)]
8. **HippoRAG 2**: From RAG to Memory: Non-Parametric Continual Learning for Large Language Models (ICML 2025) [[Paper](https://mp.weixin.qq.com/s/Gq6FTFMacjO3CpW3NtawSg)]
9. **G-Retriever**: Retrieval-Augmented Generation for Textual Graph Understanding and Question Answering (NeuRIPS 2024 poster) [[Paper](https://openreview.net/forum?id=MPJ3oXtTZl)]
10. **SUGRE**: Knowledge graph-augmented language models for knowledge-grounded dialogue generation (Arxiv 2023) [[Paper](https://arxiv.org/pdf/2305.18846)]
11. **GNN-RAG**: Graph Neural Retrieval for Efficient Large Language Model Reasoning on Knowledge Graphs (ACL 2025) [[Paper](https://aclanthology.org/2025.findings-acl.856.pdf)]
12. **KAG**: Boosting LLMs in Professional Domains via Knowledge Augmented Generation [[Paper](https://arxiv.org/pdf/2409.13731)] 🔥
> * (1) LLM-friendly knowledge representation, (2) mutual-indexing between knowledge graphs and original chunks, (3) logical-form-guided hybrid reasoning engine, (4) knowledge alignment with semantic reasoning, and (5) model capability enhancement for KAG.
> * Compared with RAG, achieving a relative improvement of 19.6% on hotpotQA and 33.5% on 2wiki in terms of F1 score.
> * Applied KAG to two professional knowledge Q&A tasks of Ant Group, including E-Government Q&A and E-Health Q&A, achieving significant improvement in professionalism compared to RAG methods.
13. **Graph RAG-Tool Fusion**: [[Paper](https://arxiv.org/pdf/2502.07223)] [[Notes (Chinese)](https://mp.weixin.qq.com/s/0yLAr_xcLr_1-EI_Np3qig)]
> * The construction of the "tool KG" seems to be very time-consuming.
14. **KG2RAG**: Knowledge Graph-Guided Retrieval Augmented Generation (NAACL 2025, From Alibaba) [[Paper]([Knowledge Graph-Guided Retrieval Augmented Generation](https://arxiv.org/pdf/2502.06864))] [[Github](https://github.com/nju-websoft/KG2RAG)] `but document-chunk related and users need to extract the graph`
15. **KG-INFUSED RAG**: AUGMENTING CORPUS-BASED RAG WITH EXTERNAL KNOWLEDGE GRAPHS (Arxiv 2025) [[Paper](https://arxiv.org/pdf/2506.09542)]
> * It incorporates pre-existing large-scale KGs into RAG and applies spreading activation to enhance both retrieval and generation.
16. **ReMindRAG**: Low-Cost LLM-Guided Knowledge Graph Traversal for Efficient RAG (Arxiv 2025) [[Paper](https://arxiv.org/abs/2510.13193)]
> * It employs an LLM-guided graph traversal featuring node exploration, node exploitation, and, most notably, memory replay, to improve both system effectiveness and cost efficiency. Specifically, REMINDRAG memorizes traversal experience within KG edge embeddings, mirroring the way LLMs "memorize" world knowledge within their parameters, but in a train-free manner.
17. KG-RAG: Enhancing GUI Agent Decision-Making via Knowledge Graph-Driven Retrieval-Augmented Generation (EMNLP 2025) [[Paper](https://aclanthology.org/2025.emnlp-main.274.pdf)]
18. Knowledge Graph Retrieval-Augmented Generation for LLM-based Recommendation (ACL 2025) [[Paper](https://aclanthology.org/2025.acl-long.1317.pdf)]
19. Hierarchical Planning for Complex Tasks with Knowledge Graph-RAG and Symbolic Verification (ICML 2025) [[Paper](https://icml.cc/virtual/2025/poster/43660)]

#### (3) Multi-level gained KG
1. **RAG-Anything**: ALL-IN-ONE RAG FRAMEWORK,  a comprehensive All-in-One Multimodal Document Processing RAG system built on LightRAG [[Paper](https://arxiv.org/pdf/2510.12323)] [[Github](https://github.com/HKUDS/RAG-Anything)] 
* **LightRAG**: Simple and Fast Retrieval-Augmented Generation (submitted to ICLR 2025) [[Open Review](https://openreview.net/forum?id=bbVH40jy7f)][[GitHub](https://github.com/HKUDS/LightRAG)] 🔥
2. **PIKE-RAG**: sPecIalized KnowledgE and Rationale Augmented Generation (Microsoft, Arxiv 2025) [[Paper](
https://arxiv.org/abs/2501.11551)] [[Github](https://github.com/microsoft/PIKE-RAG)]

#### (4) Fine-grained graph to represent procedure knowledge ("how-to" graph), not declarative knowledge ("what-is" graph)
1. InstructRAG: Leveraging Retrieval-Augmented Generation on Instruction Graphs for LLM-Based Task Planning (SIGIR 2025)

#### (5) Unclassified (still working on these!)

1. Biomedical knowledge graph-enhanced prompt generation for large language models (Nov 2023) [[Paper](https://arxiv.org/pdf/2311.17330.pdf)]
> * A task-agnostic Knowledge Graph-based Retrieval Augmented Generation (KG-RAG) framework by leveraging the massive biomedical KG SPOKE with LLMs such as Llama-2-13b, GPT-3.5-Turbo and GPT-4, to generate meaningful biomedical text rooted in established knowledge.
19. Retrieval-augmented Generation across Heterogeneous Knowledge (NAACL 2022) [[Paper](https://aclanthology.org/2022.naacl-srw.7/)]
20. Knowledge Graph Integration and Self-Verification for Comprehensive Retrieval-Augmented Generation (2024 KDD Cup CRAG Workshop) [[Paper](https://openreview.net/forum?id=457wTt0ngj)]
21. Graphusion: A RAG Framework for Knowledge Graph Construction with a Global Perspective (Arxiv 2024-10) [[Paper](https://arxiv.org/abs/2410.17600)] [[Notes(Chinese)]()]
22. LongRAG: A Dual-Perspective Retrieval-Augmented Generation Paradigm for Long-Context Question Answering (Arxiv 2024-10) [[Paper](https://arxiv.org/abs/2410.18050)] [[Github](https://github.com/QingFei1/LongRAG)]
23. KRAGEN: a knowledge graph-enhanced RAG framework for biomedical problem solving using large language models (Bioinformatics 2024) [[Paper](https://academic.oup.com/bioinformatics/article/40/6/btae353/7687047)]
24. MedRAG: Enhancing Retrieval-augmented Generation with Knowledge Graph-Elicited Reasoning for Healthcare Copilot (WWW 2025 poster) [[Paper](https://openreview.net/forum?id=7C6cd95qvH#discussion)]
25. Knowledge Graph-Driven Retrieval-Augmented Generation: Integrating Deepseek-R1 with Weaviate for Advanced Chatbot Applications (Arxiv 2025) [[Paper](https://arxiv.org/pdf/2502.11108)]
26. A Systematic Exploration of Knowledge Graph Alignment with Large Language Models in Retrieval Augmented Generation (AAAI 2025) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/34716)] ⭐
27. Hierarchical Planning for Complex Tasks with Knowledge Graph-RAG and Symbolic Verification (ICML 2025) [[Paper](https://arxiv.org/pdf/2504.04578)]
28. Advancing Feature Extraction in Healthcare through the Integration of Knowledge Graphs and Large Language Models (AAAI 2025) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/35224)]
29. SimGRAG: Leveraging Similar Subgraphs for Knowledge Graphs Driven Retrieval-Augmented Generation (ACL 2025)
30. FRAG: A Flexible Modular Framework for Retrieval-Augmented Generation based on Knowledge Graphs (ACL 2025)
31. Distill-SynthKG: Distilling Knowledge Graph Synthesis Workflow for Improved Coverage and Efficiency (submitted to ACL 2025) [[Paper](https://openreview.net/forum?id=kRpq4ONlXz)]
32. RD-P: A Trustworthy Retrieval-Augmented Prompter with Knowledge Graphs for LLMs (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679659)]
33. HyKGE: A Hypothesis Knowledge Graph Enhanced RAG Framework for Accurate and Reliable Medical LLMs Responses (ACL 2025)
35. GNN-RAG: Graph Neural Retrieval for Efficient Large Language Model Reasoning on Knowledge Graphs (ACL 2025, Findings) [[Paper](https://aclanthology.org/2025.findings-acl.856/)]
36. EventRAG: Enhancing LLM Generation with Event Knowledge Graphs (ACL 2025, Findings) [[Paper](https://aclanthology.org/2025.acl-long.830/)]
37. OG-RAG: Ontology-Grounded Retrieval-Augmented Generation For Large Language Models (Arxiv 2024, Microsoft) [[Paper](https://arxiv.org/html/2412.15235v1)] [[Github](https://github.com/microsoft/ograg2?tab=readme-ov-file)]
38. HybGRAG: Hybrid Retrieval-Augmented Generation on Textual and Relational Knowledge Bases (Arxiv 2024, Amazon) [[Paper](https://arxiv.org/pdf/2412.16311)]

### 📊 RAG benchmarks

Fact Retrieval: `Note: Most of the works use multi-hop QA dataset for evaluation.`
1. HotPotQA
2. MultiHop-RAG
3. MT-Bench

### Other related topics
Query Focused Summerization (QFS):
1. Document Summarization with Latent Queries (TACL 2022) [[Paper](https://aclanthology.org/2022.tacl-1.36/)]
