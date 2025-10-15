## Knowledge Graphs in Agent Memory (people may use "Memory Graph" instead of "Knowledge Graph")
```
Personally, there are a few keypoints that memory graph should focus on:
1. The freshness of the graph, since people's interest changes from time to time (also considered by Mem0-g and Graphiti),
2. The correctness of the entity extraction for memory, especially in multi-modal scenarios when users may use less words as instructions.
We can only guess the preference of users based on the acceptance rates of the model output such as video/figure generation.
3. The correctness of the entity matching, or the dicision of whether using the matched memory entities or not in a new scenario.
```
### General Papers and works
1. **Memory** [[Github](https://github.com/kingjulio8238/Memary/tree/main)]
> * Memary uses a graph database to store knoweldge.
> * Llama Index was used to add nodes into the graph store based on documents.
> * Perplexity (mistral-7b-instruct model) was used for external queries.
2. **ZEP**: A TEMPORAL KNOWLEDGE GRAPH ARCHITECTURE FOR AGENT MEMORY (ZepAI, Arxiv 2025) [[Paper](https://arxiv.org/pdf/2501.13956)] 🔥 HOT!
> * Zep implements three search functions: cosine semantic similarity search (ϕcos), Okapi BM25 full-text search (ϕbm25), and breadth-first search (ϕbfs). The first two functions utilize Neo4j’s implementation of Lucene.
> * **Graphiti**：Build Real-Time Knowledge Graphs for AI Agents [[Github](https://github.com/getzep/graphiti/tree/main)]
3. **AriGraph**: Learning Knowledge Graph World Models with Episodic Memory for LLM Agents (Arxiv 2024) [[Paper](https://arxiv.org/pdf/2407.04363)] [[Github](https://github.com/AIRI-Institute/AriGraph)] hot!
> *  Retrieval from the AriGraph memory consists of two procedures: (1) a semantic search returns the most relevant triplets (semantic edges) and (2) an episodic search that, given extracted triplets, returns the most relevant episodic vertices
4. **M3-Agent**: Seeing, Listening, Remembering, and Reasoning: A Multimodal Agent with Long-Term Memory (ByteDance, ACL 2025) [[Paper](https://arxiv.org/pdf/2508.09736)] 🔥 HOT!
5. **Mem0** and **Mem0-g**: Building Production-Ready AI Agents with Scalable Long-Term Memory (mem0AI, Arxiv 2025) [[Paper](https://arxiv.org/pdf/2504.19413)] [[Github](https://github.com/mem0ai/mem0)]🔥 HOT!
> * Aliyun's architecture for Mem0 (discussion in Chinese) [[Link](https://help.aliyun.com/zh/polardb/polardb-for-postgresql/ai-agent-long-memory-solution#edba335440jp6)]
5. **LightRAG**: Simple and Fast Retrieval-Augmented Generation [[Github](https://github.com/HKUDS/LightRAG)] 🔥 HOT!

### 3.3 KG for Other Tasks in Agent 
1. SciToolAgent: a knowledge-graph-driven scientific agent for multitool integration (Nature computational science 2025) [[Paper](https://www.nature.com/articles/s43588-025-00849-y)]
