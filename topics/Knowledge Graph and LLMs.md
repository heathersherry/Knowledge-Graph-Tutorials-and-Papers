## KG and LLM

### 📝 Overviews, Surveys, Tutorials and Summary
1. Github Repo: KG-LLM-Papers [[Link](https://github.com/zjukg/KG-LLM-Papers)]
2. Github Repo: Awesome LLM-KGs [[Link](https://github.com/RManLuo/Awesome-LLM-KG)]
3. The Journey to A Knowledgeable Assistant with Retrieval-Augmented Generation (RAG) (WSDM 2024 and SIGMOD 2024 keynote, by Luna Dong in Meta) 🌟
4. LLM+KG Workshop, VLDB 2024 [[Link](https://seucoin.github.io/workshop/llmkg/)]
* Talk 1 – Integrating Knowledge Graph with Large Language Model: From the Perspective of Knowledge Engineering (Prof Qi)
> * Introduction of KG and LLM
> * KG for LLM (1) pretraining (2) as prompt (e.g., KAPING) (3) fine-tuning (4) inference (reduce the hallucination) (5) RAG (6) knowledge update or edit (7) knowledge fusion (8) knowledge validation (as benchmark) (9) future: learning of symbolic knowledge, benchmark, improve the interpretable reasoning of llm
> * LLM for KG (1) entity and relation extraction (in-context learning & SFT) (2) triple generation (3) ontology matching (e.g., olala) (4) entity alignment (e.g., chatea) (5) KBQA (e.g., ELLMKGQA framework) (6) ontology reasoning (data construction: subsumption checking + instance checking) (7) KG reasoning (kg embedding is enhanced, e.g., KoPA)
> * KG&LLM integration (1) knowledge service platform based on KG&LLM Integration (2) OpenKG + Tool + Application
* The summary of the other talks. [[My notes](https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/issues/12)]
5. 1st Workshop on Knowledge Graphs and Large Language Models (KaLLM 2024, from ACL) [[Link](https://aclanthology.org/volumes/2024.kallm-1/)]
6. Knowledge Graphs Meet Multi-Modal Learning: A Comprehensive Survey [[Paper](https://arxiv.org/abs/2402.05391)]
7. OneGraph: A KG constructed by LLM [[Website](http://onegraph.openkg.cn/)] [[Data Download](http://data.openkg.cn/dataset/onegraphv1)]

### 📝 Research Papers
__Discussion and Research about Knowledge Graphs and LLMs__
1. The Future of Knowledge Graphs in a World of Large Language Models, given by Denny Vrandečić, Post-conference recording of the keynote for May 11 at the Knowledge Graph Conference 2023 in New York, NY. [[Video](https://www.youtube.com/watch?v=WqYBx2gB6vA)]
2. Language Models as Knowledge Bases? (EMNLP 2019) [[Paper](https://aclanthology.org/D19-1250.pdf)]
3. Bridging the Gap: Integrating Knowledge Graphs and Large Language Models (Arango DB) [[Video](https://www.youtube.com/watch?v=qCT1a2jdpk4)]
4. Uniting Large Language Models and Knowledge Graphs for Enhanced Knowledge Representation (Big Data LDN 2023) [[Video](https://www.youtube.com/watch?v=CEaDSOh_AoM)]
5. Language Models are Open Knowledge Graphs (ICLR 2021, Rejected) [[Paper](https://openreview.net/forum?id=aRTRjVPkm-)]
6. JAKET: Joint Pre-training of Knowledge Graph and Language Understanding (AAAI 2022) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/21417/21166)]
7. Language Models sounds the Death Knell of Knowledge Graphs (Arxiv 2023) [[Paper](https://arxiv.org/abs/2301.03980)]
8. ChatGPT versus Traditional Question Answering for Knowledge Graphs: Current Status and Future Directions Towards Knowledge Graph Chatbots (Arxiv 2023) [[Paper](https://arxiv.org/abs/2302.06466)]
> * ⭐ Interesting!! Key point: ChatGPT is trained on information from different data sources. Thus, it does not generalize to unseen domain information.
> * Advanced KG Chatbots could be developed by incorporating capabilities of language models, such as ChatGPT, in question understanding, robustness, and explainability, with the
outstanding capabilities of a QA system, such as KGQAN, in incorporating recent information and generality across different domains.
5. Towards InnoGraph: A Knowledge Graph for AI Innovation (WWW 2023) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3543873.3587614)]
6. ChatGPT下的知识图谱审视：一次关于必然影响、未来方向的讨论实录与总结 [[Link](https://www.kuxai.com/article/814)]
7. Augmented Language Models: a Survey, by MetaAI (Arxiv, Feb 2023) [[Paper](https://arxiv.org/pdf/2302.07842.pdf)]
> * it is often necessary to process structured information when interacting with tools like a knowledge base.
8. Let's Chat to Find the APIs: Connecting Human, LLM and Knowledge Graph through AI Chain (ASE 2023, Top Conf in Software Engineering) [[Paper](https://ieeexplore.ieee.org/abstract/document/10298399)]
9. Head-to-Tail: How Knowledgeable are Large Language Models (LLM)? A.K.A. Will LLMs Replace Knowledge Graphs? (NAACL 2024) [[Paper](https://arxiv.org/pdf/2308.10168.pdf)] - Xin Luna Dong from Meta 🔥
10. Unifying Large Language Models and Knowledge Graphs: A Roadmap (TKDE, July 2024) [[Paper](https://ieeexplore.ieee.org/abstract/document/10387715)] 🌟
11. Large Language Models as Reliable Knowledge Bases? (Arxiv, Jul 2024 - from University of Edinburgh and Huawei Edinburgh Research Center) [[Paper](https://arxiv.org/pdf/2407.13578)]
> This study defines criteria that a reliable LLM-as-KB should meet, focusing on factuality and consistency, and covering both seen and unseen knowledge.
12. Llm-tikg: Threat intelligence knowledge graph construction utilizing large language model (Computers & Security, 2024) [[Paper](https://www.sciencedirect.com/science/article/pii/S0167404824003043)]
13. Large Language Models and Knowledge Graphs: Opportunities and Challenges (Arxiv, Aug 2023) [[Paper](https://arxiv.org/pdf/2308.06374)] [[Notes (Chinese)](https://hub.baai.ac.cn/view/29492)]
14. MKGL: Mastery of a Three-Word Language (NeurIPS 2024 Spotlight) [[Paper](https://openreview.net/forum?id=eqMNwXvOqn)]
>   0. Main target: LLMs to carry out knowledge graph completion.
>   1. They investigate the integration of LLMs with KGs by introducing a specialized KG Language (KGL), where a sentence precisely consists of an entity noun, a relation verb, and ends with another entity noun.
>   2. Conclusions: (1) LLMs can achieve fluency in KGL, drastically reducing errors compared to conventional KG embedding methods on KG completion. (2) The enhanced LLM shows exceptional competence in generating accurate three-word sentences from an initial entity and interpreting new unseen terms out of KGs.

__LLMs for Knowledge Graphs__
1. Enhancing Knowledge Graph Construction Using Large Language Models (Arxiv 2023) [[Paper](https://arxiv.org/pdf/2305.04676.pdf)]
2. Complex Logical Reasoning over Knowledge Graphs using Large Language Models (Arxiv 2023) [[Paper(https://arxiv.org/pdf/2305.01157)]
3. Enhanced Story Comprehension for Large Language Models through Dynamic Document-Based Knowledge Graphs (AAAI 2022) [[Paper](https://cdn.aaai.org/ojs/21286/21286-13-25299-1-2-20220628.pdf)]
4. Fusing topology contexts and logical rules in language models for knowledge graph completion (Information Fusion 2022) [[Paper](https://www.sciencedirect.com/science/article/pii/S1566253522001592)]
5. From Discrimination to Generation: Knowledge Graph Completion with Generative Transformer (WWW 2022) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3487553.3524238)]
6. Path Language Modeling over Knowledge Graphsfor Explainable Recommendation (WWW 2022) [[Paper](https://dl.acm.org/doi/abs/10.1145/3485447.3511937)]
7. GraphGPT [[Github](https://github.com/varunshenoy/GraphGPT)]
8. CodeKGC: Code Language Model for Generative Knowledge Graph Construction (Arxiv, April 2023) [[Paper](https://arxiv.org/abs/2304.09048)]
9. LLMs for Knowledge Graph Construction and Reasoning: Recent Capabilities and Future Opportunities (Arxiv, May 2023) [[Paper](https://arxiv.org/pdf/2305.13168.pdf)]
10. Think-on-Graph: Deep and Responsible Reasoning of Large Language Model on Knowledge Graph (ICLR 2024 poster) [[Paper](https://openreview.net/forum?id=nnVO1PvbTv)]
> * A new LLM-KG integrating paradigm which treats the LLM as an agent to interactively explore related entities and relations on KGs and perform reasoning based on the retrieved knowledge.
> * The authors of paper 11 (below) comments on the openreview panel.
11. Don’t Generate, Discriminate: A Proposal for Grounding Language Models to Real-World Environments (ACL 2023) [[Paper](https://arxiv.org/pdf/2212.09736.pdf)]
> * Pangu consists of a symbolic agent and a neural LM working in a concerted fashion: The agent explores the environment to incrementally construct valid plans, and the LM evaluates the plausibility of the candidate plans to
guide the search process.
> * The evaluation is conducted on KBQA.
12. LLM-assisted Knowledge Graph Engineering: Experiments with ChatGPT (AIDRST 2023) [[Paper](https://link.springer.com/chapter/10.1007/978-3-658-43705-3_8)]
13. Making Large Language Models Perform Better in Knowledge Graph Completion (Arxiv 2023, but with 30+ citations) [[Paper](https://arxiv.org/pdf/2310.06671v2)]
14. Assessing the evolution of llm capabilities for knowledge graph engineering in 2023 (ESWC 2024) [[Paper](https://2024.eswc-conferences.org/wp-content/uploads/2024/04/ESWC_2024_paper_275.pdf)]
15. Language Models-enhanced Semantic Topology Representation Learning For Temporal Knowledge Graph Extrapolation (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679602)]
16. LLMs for knowledge graph construction and reasoning: recent capabilities and future opportunities (WWW journal 2024) [[Paper](https://link.springer.com/article/10.1007/s11280-024-01297-w)]
17. Collaborative System Synergizing Human Expertise and Large-scale Language Models for Legal Knowledge Graph Construction (CEUR-WS 2024) [[Paper](https://ceur-ws.org/Vol-3828/paper9.pdf)]
18. SAC-KG: Exploiting Large Language Models as Skilled Automatic Constructors for Domain Knowledge Graph (ACL 2024) [[Paper](https://aclanthology.org/2024.acl-long.238/)] [[Notes (Chinese)](https://mp.weixin.qq.com/s/kxkQDspKeRTw-CveR2trWw?token=1056117110&lang=zh_CN)]
19. UrbanKGent: A Unified Large Language Model Agent Framework for Urban Knowledge Graph Construction (NeurIPS 2024) [[Paper](https://arxiv.org/pdf/2402.06861)]
20. A Prompt-Based Knowledge Graph Foundation Model for Universal In-Context Reasoning (NeurIPS 2024) [[Paper](https://arxiv.org/pdf/2410.12288)]
>   LLM for KG reasoning
21. Editing Language Model-based Knowledge Graph Embeddings (AAAI 2024) [[Paper](https://arxiv.org/pdf/2301.10405)]
>   Update KG embedding for data freshness
22. Language Models over Large-Scale Knowledge Base: on Capacity, Flexibility and Reasoning for New Facts (COLING 2025)
23. Construction and Canonicalization of Economic Knowledge Graphs with LLMs (KGSWC 2024) [[Link](https://books.google.com.hk/books?hl=zh-CN&lr=&id=3yhGEQAAQBAJ&oi=fnd&pg=PA334&ots=KPSlLdVk8m&sig=HW4PzpubB902d1_dLgwv_UWpIGY&redir_esc=y#v=onepage&q&f=false)]
24. Utilizing Language Models For Synthetic Knowledge Graph Generation (ICLR 2025 Workshop Data Problems) [[Paper](https://openreview.net/forum?id=IutH9tRtMI)]
25. Finetuning Generative Large Language Models with Discrimination Instructions for Knowledge Graph Completion (ISWC 2024) [[Paper](https://arxiv.org/pdf/2407.16127)] 

__Knowledge Graphs for LLMs__
1. Using Knowledge Graph data in Large Language Models (Keynote) [[Video](https://www.youtube.com/watch?v=SHHHJXwHeWM)]
2. SKILL: Structured Knowledge Infusion for Large Language Models (NAACL 2022, by Google Research) [[Paper](https://aclanthology.org/2022.naacl-main.113.pdf)]
3. Enriching contextualized language model from knowledge graph for biomedical information extraction (Briefings in Bioinformatics) [[Paper](https://academic.oup.com/bib/article/22/3/bbaa110/5854405)]
4. Barack's Wife Hillary: Using Knowledge-Graphs for Fact-Aware Language Modeling (ACL 2019) [[Paper](https://arxiv.org/pdf/1906.07241.pdf)]
> * knowledge graph language model (KGLM): a neural language model with mechanisms for selecting and copying facts from a knowledge graph that are relevant to the context.
5. Improving Commonsense in Vision-Language Models via Knowledge Graph Riddles (Arxiv 2022) [[Paper](https://arxiv.org/abs/2211.16504)]
6. Give Us the Facts: Enhancing Large Language Models with Knowledge Graphs for Fact-aware Language Modeling (TKDE 2024) [[Paper](https://arxiv.org/pdf/2306.11489.pdf)]
7. Knowledge Graph Based Synthetic Corpus Generation for Knowledge-Enhanced Language Model Pre-training (NAACL 2021) [[Paper](https://aclanthology.org/2021.naacl-main.278/)]
8. GraphAdapter: Tuning Vision-Language Models With Dual Knowledge Graph (NeurIPS 2023) [[Papers](https://proceedings.neurips.cc/paper_files/paper/2023/hash/2b25c39788e5cf11d3541de433ebf4c0-Abstract-Conference.html)] --> KGs for VLMs
9. Mitigating Large Language Model Hallucinations via Autonomous Knowledge Graph-Based Retrofitting (AAAI 2024) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/29770)]
10. RD-P: A Trustworthy Retrieval-Augmented Prompter with Knowledge Graphs for LLMs (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679659)]
11. Tree-of-Traversals: A Zero-Shot Reasoning Algorithm for Augmenting Black-box Language Models with Knowledge Graphs (ACL 2024) [[Paper](https://arxiv.org/abs/2407.21358)] [[Notes](https://mp.weixin.qq.com/s?__biz=MzU2NjAxNDYwMg==&mid=2247507048&idx=1&sn=8ebfe3c9a0f7593e6453994574b5ba57&chksm=fcb07b8dcbc7f29b4d33080d7f144f097d9f056bff75ff053d86c4c9f0007f48210481ce4f1e&token=1932359749&lang=zh_CN#rd)]
>   A new dataset: MusicBrainz-x-Wikidata, which contains 109 questions that require reasoning with information from both MusicBrainz and Wikidata.
12. Knowledge Graph Finetuning Enhances Knowledge Manipulation in Large Language Models (ICLR 2025 Poster, Jieping Ye) [[Paper](https://openreview.net/forum?id=oMFOKjwaRS)]
13. Structuring Benchmark into Knowledge Graphs to Assist Large Language Models in Retrieving and Designing Models (ICLR 2025 Poster, Xiaofang Zhou and Lei Chen) [[Paper](https://openreview.net/forum?id=49fIu0yDJ4)]
14. KBLaM: Knowledge Base augmented Language Model (ICLR 2025, Poster) [[Paper](https://openreview.net/forum?id=aLsMzkTej9)]
15. Aligning Complex Knowledge Graph Question Answering as Knowledge-Aware Constrained Code Generation (COLING 2025) [[Paper](https://aclanthology.org/2025.coling-main.267.pdf)]


__LLMs and Knowledge Graphs for Other Tasks (e.g., Information Extraction, Question generation)__
1. ChatGraph: Interpretable Text Classification by Converting ChatGPT Knowledge to Graphs (Arxiv, May 2023) [[Paper](https://arxiv.org/pdf/2305.03513.pdf)]
2. KG-BART: Knowledge Graph-Augmented BART for Generative Commonsense Reasoning (AAAI 2021) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/16796)]
3. QA-GNN: Reasoning with Language Models and Knowledge Graphs for Question Answering (NAACL 2021) [[Paper](https://aclanthology.org/2021.naacl-main.45/)]
4. Knowledge Graph-Based Chatbot With GPT-3 and Neo4j (from Neo4j) [[Link](https://neo4j.com/developer-blog/knowledge-graph-based-chatbot-with-gpt-3-and-neo4j/)]
5. Integrate LLM workflows with Knowledge Graph using Neo4j and APOC [[Link](https://towardsdatascience.com/integrate-llm-workflows-with-knowledge-graph-using-neo4j-and-apoc-27ef7e9900a2)] ⭐
> * Solution 1: use LLMs to generate a Cypher statement that can be used to retrieve connected information from the database.
> * Solution 2: use the connection information to enrich the text embedding representations. Additionally, the enhanced information can be retrieved at query time to provide additional context to the LLM from which it can base its response. (used in this project)
6. FLEEK: Factual Error Detection and Correction with Evidence Retrieved from External Knowledge (EMNLP 2023) [[Paper](https://arxiv.org/pdf/2310.17119.pdf)]
7. KGLink: A column type annotation method that combines knowledge graph and pre-trained language model (ICDE 2024) [[Paper](https://arxiv.org/pdf/2406.00318)] ⭐
8. Contextualization Distillation from Large Language Model for Knowledge Graph Completion (ACL 2024) [[Paper](https://arxiv.org/pdf/2402.01729)]
9. From Superficial to Deep: Integrating External Knowledge for Follow-up Question Generation Using Knowledge Graph and LLM (COLING 2025)
10. CogMG: Collaborative Augmentation Between Large Language Model and Knowledge Graph (ACL 2024) [[Paper](https://aclanthology.org/2024.acl-demos.35.pdf)] [[Notes (Chinese)](https://mp.weixin.qq.com/s/5NrkHqoZMNdyTWKVPNgXTA?token=1754278729&lang=zh_CN)]
> * KGs can be employed to address the hallusiasion in LLMs. Howevers, KGs may be (1) incomplete, or (2) knowledge inconsistant while applied with information extraction techniques. LLM helps to address this two issues. Therefore, a CogMG framework is proposed for the collaborative augmentation between LLM and KGs.
11. Advancing Feature Extraction in Healthcare through the Integration of Knowledge Graphs and Large Language Models (AAAI 2025) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/35224)]
12. LLM-based Typed Hyperresolution for Commonsense Reasoning with Knowledge Bases (ICLR 2025, poster) [[Paper](https://openreview.net/forum?id=wNobG8bV5Q)]
13. LLM is Knowledge Graph Reasoner: LLM’s Intuition-Aware Knowledge Graph Reasoning for Cold-Start Sequential Recommendation (ECIR 2025) [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-88711-6_17)] 



__RAG (Retrieval augmented generation) and Knowledge Graphs/Graph RAG/KAG__

💡 Traditional RAG Frameworks - It is highly recommended that you get familiar with one or more of the following frameworks first：
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

💡 Some good papers/surveys for beginners to know more about RAG and Graph RAG:
1. Retrieval-Augmented Generation for Large Language Models: A Survey (Arxiv, Mar 2024) [[Paper](https://arxiv.org/pdf/2312.10997)] [[Notes for OpenRAG Base](https://mp.weixin.qq.com/s/MZ4jSH1torrEpYGTLTkiEw)]
2. Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks (NeurIPS 2020) [[Paper](https://arxiv.org/pdf/2005.11401.pdf)]
3. A Survey of Graph Retrieval-Augmented Generation for Customized Large Language Models (Arxiv, Jan 2025) [[Paper](https://github.com/DEEP-PolyU/Awesome-GraphRAG)]
> My thoughts!:
> * This may be different from multi-modal RAG, where the context is in multiple modalities (e.g., image, text, video, ...) represented as embedding, and the query is based on fuzzy serach in vector db. If we need to query the knowledge in KGs, we need to rely on other query engine, such as SPAEQL on graphs.
> * Graph RAG/KAG may be more valuable in domain-specific area.
> * However, although the evaluation results on research benchmarks of multi-hop QA proves that KAG works, I am still wondering whether KAG really works in real-world scenarios, since building accurate domain-specific KG is very costly. Purely employing the exisiting information extraction methods (e.g., various tools for OpenIE) cannot output a KG with 100% correct and reliable knowledge, which may lead to hallusiciasion as well. Maybe the KAG work (Arxiv 2024) is a good example to start this research, since it successfully applied KAG to two professional knowledge Q&A tasks of the industrial downstream tasks in the Ant Group.
> * The keypoint of Graph RAG/KAG should be **the wiseful integration** of the benefits of unstructured information and structured information.

💡 There are some pioneer works that **use KGs** to enhance the performance of the RAG system in multi-hop and cross-paragraph tasks. Strong reasoning capabilities have been introduced into the RAG technical framework.
1. **GraphRAG (Microsoft)**: From Local to Global: A Graph RAG Approach to Query-Focused Summarization (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2404.16130)] [[GitHub](https://github.com/microsoft/graphrag)]
> * GraphRAG-Local-UI/GraphRAG-Ollama-UI,  an adaptation of Microsoft's GraphRAG, tailored to support local models and featuring a comprehensive interactive user interface ecosystem. [[GitHub](https://github.com/severian42/GraphRAG-Local-UI)]
2. **DALK**: Dynamic Co-Augmentation of LLMs and KG to answer Alzheimer's Disease Questions with Scientific Literature  (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2405.04819)]
3. **SUGRE**: Knowledge graph-augmented language models for knowledge-grounded dialogue generation (Arxiv 2023) [[Paper](https://arxiv.org/pdf/2305.18846)]
4. **ToG 2.0**: Think-on-Graph 2.0: Deep and Faithful Large Language Model Reasoning with Knowledge-guided Retrieval Augmented Generation (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2407.10805)]
5. **GRAG**: Graph Retrieval-Augmented Generation (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2405.16506)]
6. **GNN-RAG**: Graph Neural Retrieval for Large Language Model Reasoning (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2405.20139)]
7. **HippoRAG**: Neurobiologically Inspired Long-Term Memory for Large Language Models [[Paper](https://arxiv.org/pdf/2405.14831)]
8. **OpenSPG**, a knowledge graph engine developed by Ant Group in collaboration with OpenKG [[Website](https://spg.openkg.cn/)] [[Github](https://github.com/OpenSPG/openspg/tree/master)] ⭐
> * an open engine for knowledge graph designed and implemented on the basis of SPG framework, which provides explicit semantic representations, logical rule definitions, operator frameworks (construction, inference) and other capabilities for the domain knowledge graphs, and supports pluggable adaptation of basic engines and algorithmic services by various vendors to build customized solutions.
9. **KAG**: Boosting LLMs in Professional Domains via Knowledge Augmented Generation [[Paper](https://arxiv.org/pdf/2409.13731)] ⭐
> * (1) LLM-friendly knowledge representation, (2) mutual-indexing between knowledge graphs and original chunks, (3) logical-form-guided hybrid reasoning engine, (4) knowledge alignment with semantic reasoning, and (5) model capability enhancement for KAG.
> * Compared with RAG, achieving a relative improvement of 19.6% on hotpotQA and 33.5% on 2wiki in terms of F1 score.
> * Applied KAG to two professional knowledge Q&A tasks of Ant Group, including E-Government Q&A and E-Health Q&A, achieving significant improvement in professionalism compared to RAG methods.
10. **LightRAG**: Simple and Fast Retrieval-Augmented Generation (submitted to ICLR 2025) [[Open Review](https://openreview.net/forum?id=bbVH40jy7f)][[GitHub](https://github.com/HKUDS/LightRAG)] 🔥
11. **PIKE-RAG**: sPecIalized KnowledgE and Rationale Augmented Generation (Microsoft, Arxiv 2025) [[Paper](
https://arxiv.org/abs/2501.11551)] [[Github](https://github.com/microsoft/PIKE-RAG)]
12. **LazyGraphRAG**: Setting a new standard for quality and cost - Microsoft Research (Microsoft, Nov 2024) [[Source](https://www.microsoft.com/en-us/research/blog/lazygraphrag-setting-a-new-standard-for-quality-and-cost/)] [[Discussion (Chinese)](https://mp.weixin.qq.com/s?__biz=MzI3ODE5Mzc1Ng==&mid=2247493514&idx=1&sn=588c7388d247fc34771c8ab76aa0f2ce&scene=21#wechat_redirect)]
13. **Graph RAG-Tool Fusion** [[Paper](https://arxiv.org/pdf/2502.07223)] [[Notes (Chinese)](https://mp.weixin.qq.com/s/0yLAr_xcLr_1-EI_Np3qig)]
>   * The construction of the "tool KG" seems to be very time-consuming.


💡 Here are some general research works for KG+RAG:
1. Knowledge Graph RAG Query Engine [[Link](https://docs.llamaindex.ai/en/stable/examples/query_engine/knowledge_graph_rag_query_engine.html)]
2. GraphRAG: Unlocking LLM discovery on narrative private data (Feb 2024, Microsoft) [[Link](https://www.microsoft.com/en-us/research/blog/graphrag-unlocking-llm-discovery-on-narrative-private-data/)]
3. Going Meta - Ep 22: RAG with Knowledge Graphs (from Neo4j) [[YouTube](https://www.youtube.com/watch?v=9DxwgIKVSHY)]
4. A very clear blog (in Chinese) to demonstrate Graph RAG: 7 种查询策略教你用好 Graph RAG 探索知识图谱 [[Blog](https://www.cnblogs.com/nebulagraph/p/17882072.html)], which also provides valuable references:
> * Graph RAG LlamaIndex Workshop：[[Blog](https://colab.research.google.com/drive/1tLjOg2ZQuIClfuWrAC2LdiZHCov8oUbs?usp=sharing)]
> * Knowledge Graph Index：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/index_structs/knowledge_graph/KnowledgeGraphDemo.html#knowledge-graph-index)]
> * Knowledge Graph Query Engine：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/query_engine/knowledge_graph_query_engine.html)]
> * Knowledge Graph RAG Query Engine：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/query_engine/knowledge_graph_rag_query_engine.html)]
> * Custom Retriever combining KG Index and VectorStore Index：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/index_structs/knowledge_graph/KnowledgeGraphIndex_vs_VectorStoreIndex_vs_CustomIndex_combined.html)]
> * LlamaIndex Webinar: Graph Databases, Knowledge Graphs, and RAG with Wey (NebulaGraph)：[[Link](https://www.youtube.com/watch?v=bPoNCkjDmco)]
> * Enhancing Large Language Models with Knowledge Graphs: The Role of Graph Algorithms
5. Biomedical knowledge graph-enhanced prompt generation for large language models (Nov 2023) [[Paper](https://arxiv.org/pdf/2311.17330.pdf)]
> * A task-agnostic Knowledge Graph-based Retrieval Augmented Generation (KG-RAG) framework by leveraging the massive biomedical KG SPOKE with LLMs such as Llama-2-13b, GPT-3.5-Turbo and GPT-4, to generate meaningful biomedical text rooted in established knowledge.
6. ActiveRAG (a new topic!) [[Notes in Chinese](https://mp.weixin.qq.com/s/K8V4z4e2ziJA1wfiCAxq_g)]
7. Retrieval-augmented Generation across Heterogeneous Knowledge (NAACL 2022) [[Paper](https://aclanthology.org/2022.naacl-srw.7/)]
8. GraphRAG by Microsoft [[GitHub repo](https://github.com/microsoft/graphrag)] ⭐
> * It uses knowledge graph memory structures to enhance LLM outputs
9. Knowledge Graph Integration and Self-Verification for Comprehensive Retrieval-Augmented Generation (2024 KDD Cup CRAG Workshop) [[Paper](https://openreview.net/forum?id=457wTt0ngj)]
10. Graphusion: A RAG Framework for Knowledge Graph Construction with a Global Perspective (Arxiv 2024-10) [[Paper](https://arxiv.org/abs/2410.17600)] [[Notes(Chinese)]()]
11. LongRAG: A Dual-Perspective Retrieval-Augmented Generation Paradigm for Long-Context Question Answering (Arxiv 2024-10) [[Paper](https://arxiv.org/abs/2410.18050)] [[Github](https://github.com/QingFei1/LongRAG)]
12. KRAGEN: a knowledge graph-enhanced RAG framework for biomedical problem solving using large language models (Bioinformatics 2024) [[Paper](https://academic.oup.com/bioinformatics/article/40/6/btae353/7687047)]
13. MedRAG: Enhancing Retrieval-augmented Generation with Knowledge Graph-Elicited Reasoning for Healthcare Copilot (WWW 2025 poster) [[Paper](https://openreview.net/forum?id=7C6cd95qvH#discussion)]
14. Knowledge Graph-Driven Retrieval-Augmented Generation: Integrating Deepseek-R1 with Weaviate for Advanced Chatbot Applications (Arxiv 2025) [[Paper](https://arxiv.org/pdf/2502.11108)]
15. A Systematic Exploration of Knowledge Graph Alignment with Large Language Models in Retrieval Augmented Generation (AAAI 2025) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/34716)] ⭐
16. Hierarchical Planning for Complex Tasks with Knowledge Graph-RAG and Symbolic Verification (ICML 2025) [[Paper](https://arxiv.org/pdf/2504.04578)]

__Prompting and Knowledge Graphs__
1. Knowledge Graph Prompting for Multi-Document Question Answering (AAAI 2024) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/29889)]
2. KG-prompt: Interpretable knowledge graph prompt for pre-trained language models (Knowledge-Based Systems, 2025) [[Paper](https://www.sciencedirect.com/science/article/pii/S0950705125001650)]
3. KnowGPT: Knowledge Graph based Prompting for Large Language Models (NeurIPS 2024) [[Paper](https://proceedings.neurips.cc/paper_files/paper/2024/file/0b8705a611ed1ce19cdb759031078705-Paper-Conference.pdf)]
> * 3 existing challenges for KG-enhanced LLMs：huge search space, high API costs, and laborious prompt engineering.
> * KnowGPT enhance LLMs with domain knowledge. It contains a knowledge extraction module to extract the most informative knowledge from KGs, and a context-aware prompt construction module to automatically convert extracted knowledge into effective prompts.

__VLMs and Knowledge Graphs__
1. GraphAdapter: Tuning Vision-Language Models With Dual Knowledge Graph (NeurIPS 2023 poster) [[OpenReview](https://openreview.net/forum?id=YmEDnMynuO&noteId=0rFYtJNqHc)]

__Related Works and Discussion (maybe they are not directly related to both KG and LLM, but they give us some insights!)__
1. ReGen: Reinforcement Learning for Text and Knowledge Base Generation using Pretrained Language Models (Arxiv 2021) [[Paper](https://arxiv.org/pdf/2108.12472.pdf)]
> From Graph to Text
2. Tutorial: Knowledge-Driven Vision-Language Encoding (CVPR 2023) [[Link](https://blender.cs.illinois.edu/tutorial/KnowledgeVLP/)]
3. How Large Language Models Will Disrupt Data Management (VLDB 2023) [[Paper](https://dl.acm.org/doi/abs/10.14778/3611479.3611527?casa_token=R7i7B4vpWogAAAAA:gYDDYu_4iVROViIGQOkNl3y8k4Ap3NE3B99Pjya6pIpmhRlpF-22PbOn_vIRV67bshk1vmTHRzowTQ)] ⭐

### 📊 Tools, Datasets, and Benchmarks
1. Open RAG, an opensource RAG KB. [[Link](https://openrag.notion.site/Open-RAG-c41b2a4dcdea4527a7c1cd998e763595)]
2. A Benchmark to Understand the Role of Knowledge Graphs on Large Language Model's Accuracy for Question Answering on Enterprise SQL Databases (GRADES-NDA 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3661304.3661901)]
3. OneEval: A benchmark for LLM+KB tasks. [[Details (Chinese)](https://mp.weixin.qq.com/s/BeKah91_texXN3s1WAOcKg)] [[Website](http://oneeval.openkg.cn/)]
> * 4 types of Knowledge (text, table, KG, code) + 6 key areas (general, medical, politics, science, law, programming)
