## KG and LLM

### 📝 Overviews, Surveys, Tutorials and Summary
1. Github Repo: KG-LLM-Papers [[Link](https://github.com/zjukg/KG-LLM-Papers)]
2. Github Repo: Awesome LLM-KGs [[Link](https://github.com/RManLuo/Awesome-LLM-KG)]
3. The Journey to A Knowledgeable Assistant with Retrieval-Augmented Generation (RAG) (WSDM 2024 and SIGMOD 2024 keynote, by Luna Dong in Meta) 🌟
4. LLM+KG Workshop, VLDB 2024 [[Link](https://seucoin.github.io/workshop/llmkg/)]

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
9. Head-to-Tail: How Knowledgeable are Large Language Models (LLM)? A.K.A. Will LLMs Replace Knowledge Graphs? (Arxiv 2023) [[Paper](https://arxiv.org/pdf/2308.10168.pdf)]
10. Unifying Large Language Models and Knowledge Graphs: A Roadmap (TKDE, July 2024) [[Paper](https://ieeexplore.ieee.org/abstract/document/10387715)] 🌟


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

__LLMs and Knowledge Graphs for Other Tasks (e.g., Information Extraction)__
1. ChatGraph: Interpretable Text Classification by Converting ChatGPT Knowledge to Graphs (Arxiv, May 2023) [[Paper](https://arxiv.org/pdf/2305.03513.pdf)]
2. KG-BART: Knowledge Graph-Augmented BART for Generative Commonsense Reasoning (AAAI 2021) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/16796)]
3. QA-GNN: Reasoning with Language Models and Knowledge Graphs for Question Answering (NAACL 2021) [[Paper](https://aclanthology.org/2021.naacl-main.45/)]
4. Knowledge Graph-Based Chatbot With GPT-3 and Neo4j (from Neo4j) [[Link](https://neo4j.com/developer-blog/knowledge-graph-based-chatbot-with-gpt-3-and-neo4j/)]
5. Integrate LLM workflows with Knowledge Graph using Neo4j and APOC [[Link](https://towardsdatascience.com/integrate-llm-workflows-with-knowledge-graph-using-neo4j-and-apoc-27ef7e9900a2)] ⭐
> * Solution 1: use LLMs to generate a Cypher statement that can be used to retrieve connected information from the database.
> * Solution 2: use the connection information to enrich the text embedding representations. Additionally, the enhanced information can be retrieved at query time to provide additional context to the LLM from which it can base its response. (used in this project)
6. FLEEK: Factual Error Detection and Correction with Evidence Retrieved from External Knowledge (EMNLP 2023) [[Paper](https://arxiv.org/pdf/2310.17119.pdf)]
7. KGLink: A column type annotation method that combines knowledge graph and pre-trained language model (ICDE 2024) [[Paper](https://arxiv.org/pdf/2406.00318)] ⭐

__RAG (Retrieval augmented generation) and Knowledge Graphs__
> * Note: This may be different from multi-modal RAG, where the context is in multiple modalities (e.g., image, text, video, ...) represented as embedding, and the query is based on fuzzy serach in vector db. If we need to query the knowledge in KGs, we need to rely on other query engine, such as SPAEQL on graphs.
1. (A very good paper for beginners) Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks (NeurIPS 2020) [[Paper](https://arxiv.org/pdf/2005.11401.pdf)]
2. Knowledge Graph RAG Query Engine [[Link](https://docs.llamaindex.ai/en/stable/examples/query_engine/knowledge_graph_rag_query_engine.html)]
3. GraphRAG: Unlocking LLM discovery on narrative private data (Feb 2024, Microsoft) [[Link](https://www.microsoft.com/en-us/research/blog/graphrag-unlocking-llm-discovery-on-narrative-private-data/)]
4. Going Meta - Ep 22: RAG with Knowledge Graphs (from Neo4j) [[YouTube](https://www.youtube.com/watch?v=9DxwgIKVSHY)]
5. A very clear blog (in Chinese) to demonstrate Graph RAG: 7 种查询策略教你用好 Graph RAG 探索知识图谱 [[Blog](https://www.cnblogs.com/nebulagraph/p/17882072.html)], which also provides valuable references:
> * Graph RAG LlamaIndex Workshop：[[Blog](https://colab.research.google.com/drive/1tLjOg2ZQuIClfuWrAC2LdiZHCov8oUbs?usp=sharing)]
> * Knowledge Graph Index：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/index_structs/knowledge_graph/KnowledgeGraphDemo.html#knowledge-graph-index)]
> * Knowledge Graph Query Engine：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/query_engine/knowledge_graph_query_engine.html)]
> * Knowledge Graph RAG Query Engine：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/query_engine/knowledge_graph_rag_query_engine.html)]
> * Custom Retriever combining KG Index and VectorStore Index：[[Link](https://gpt-index.readthedocs.io/en/stable/examples/index_structs/knowledge_graph/KnowledgeGraphIndex_vs_VectorStoreIndex_vs_CustomIndex_combined.html)]
> * LlamaIndex Webinar: Graph Databases, Knowledge Graphs, and RAG with Wey (NebulaGraph)：[[Link](https://www.youtube.com/watch?v=bPoNCkjDmco)]
> * Enhancing Large Language Models with Knowledge Graphs: The Role of Graph Algorithms
6. Biomedical knowledge graph-enhanced prompt generation for large language models (Nov 2023) [[Paper](https://arxiv.org/pdf/2311.17330.pdf)]
> * A task-agnostic Knowledge Graph-based Retrieval Augmented Generation (KG-RAG) framework by leveraging the massive biomedical KG SPOKE with LLMs such as Llama-2-13b, GPT-3.5-Turbo and GPT-4, to generate meaningful biomedical text rooted in established knowledge.
7. ActiveRAG (a new topic!) [[Notes in Chinese](https://mp.weixin.qq.com/s/K8V4z4e2ziJA1wfiCAxq_g)]
8. Retrieval-augmented Generation across Heterogeneous Knowledge (NAACL 2022) [[Paper](https://aclanthology.org/2022.naacl-srw.7/)]
9. GraphRAG by Microsoft [[GitHub repo](https://github.com/microsoft/graphrag)] ⭐
> * It uses knowledge graph memory structures to enhance LLM outputs

__Prompting and Knowledge Graphs__
1. Knowledge Graph Prompting for Multi-Document Question Answering (AAAI 2024) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/29889)]

__Related Works and Discussion (maybe they are not directly related to both KG and LLM, but they give us some insights!)__
1. ReGen: Reinforcement Learning for Text and Knowledge Base Generation using Pretrained Language Models (Arxiv 2021) [[Paper](https://arxiv.org/pdf/2108.12472.pdf)]
> From Graph to Text
2. Tutorial: Knowledge-Driven Vision-Language Encoding (CVPR 2023) [[Link](https://blender.cs.illinois.edu/tutorial/KnowledgeVLP/)]
3. How Large Language Models Will Disrupt Data Management (VLDB 2023) [[Paper](https://dl.acm.org/doi/abs/10.14778/3611479.3611527?casa_token=R7i7B4vpWogAAAAA:gYDDYu_4iVROViIGQOkNl3y8k4Ap3NE3B99Pjya6pIpmhRlpF-22PbOn_vIRV67bshk1vmTHRzowTQ)] ⭐
