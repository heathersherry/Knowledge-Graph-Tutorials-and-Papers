### Discussion and Research for Knowledge Graphs and LLMs
1. The Future of Knowledge Graphs in a World of Large Language Models, given by Denny Vrandečić, Post-conference recording of the keynote for May 11 at the Knowledge Graph Conference 2023 in New York, NY. [[Video](https://www.youtube.com/watch?v=WqYBx2gB6vA)]
2. Language Models as Knowledge Bases? (EMNLP 2019) [[Paper](https://aclanthology.org/D19-1250.pdf)]
3. Language Models are Open Knowledge Graphs (ICLR 2021, Rejected) [[Paper](https://openreview.net/forum?id=aRTRjVPkm-)]
4. JAKET: Joint Pre-training of Knowledge Graph and Language Understanding (AAAI 2022) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/21417/21166)]
5. Language Models sounds the Death Knell of Knowledge Graphs (Arxiv 2023) [[Paper](https://arxiv.org/abs/2301.03980)]
6. ChatGPT versus Traditional Question Answering for Knowledge Graphs: Current Status and Future Directions Towards Knowledge Graph Chatbots (Arxiv 2023) [[Paper](https://arxiv.org/abs/2302.06466)]
> * ⭐ Interesting!! Key point: ChatGPT is trained on information from different data sources. Thus, it does not generalize to unseen domain information.
> * Advanced KG Chatbots could be developed by incorporating capabilities of language models, such as ChatGPT, in question understanding, robustness, and explainability, with the
outstanding capabilities of a QA system, such as KGQAN, in incorporating recent information and generality across different domains.
5. Towards InnoGraph: A Knowledge Graph for AI Innovation (WWW 2023) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3543873.3587614)]
6. ChatGPT下的知识图谱审视：一次关于必然影响、未来方向的讨论实录与总结 [[Link](https://www.kuxai.com/article/814)]
7. Augmented Language Models: a Survey, by MetaAI (Arxiv, Feb 2023) [[Paper](https://arxiv.org/pdf/2302.07842.pdf)]
> * it is often necessary to process structured information when interacting with tools like a knowledge base.
8. 万字长文讲述大模型与知识图谱的关系 [[Link](https://zhuanlan.zhihu.com/p/626433991)]
> Q3: 有了这种大模型以后，知识图谱还有意义吗？
> * 知识图谱是有意义的，因为神经网络目前无法解决或者非常难以解决事实性准确的问题 (Google LaMDA, Deepmind)
> * 专业知识in垂直领域
> * 可以把 GPT 这种更加自由的交互和领域内的专家知识去做更深度的融合。当然也有可能未来把知识图谱通过编码的方式进入到大模型的空间。
> * 大模型参数量很大，没法对它进行重复训练和时效性不好的问题
> 
> Q4: 对于大模型的问题是回答缺乏事实的验证，知识图谱是不是可以来帮助解决问题？就像当年有搜索引擎也用了知识链接的方式去辅助搜索或者做引证。
> * 另一件事情是可以考虑在过程中将知识做卸载，并不需要去过分的将很多的事实性知识去放在模型里面，可以将事实知识放在本身的外部库里，然后通过一个类似于向量数据库，或者说是向量的近邻检索的 reader 的方式去做搭配，最后作为一个整体仍然具有一样的能力，对于时效性和验真性的部分就完全通过外部的数据库系统去考虑。因为对大模型去做更新，或者基于神经的知识编辑，代价还是很高，而且具体应该编辑哪一块还是黑盒，可能会影响其他任务的表现，所以还不如让它外置在外部数据库（或者数据仓库或者数据湖）里，然后通过积累的数据治理和知识验证的数据去作为辅助。这样从工程落地的角度来说，它的可行性和成本可控性会更好。
> * 在需要可控知识或可控逻辑的时候，知识图谱会发挥更大作用；需要更自由的交互任务理解和生成时，大模型发挥更好的作用。
> 
> Q5：知识图谱在大模型中如何去使用？(Summary)

	1. 把知识图谱转化成文本，作为文本语料的一部分，或者说作为比较好的语料，成为训练的一部分去做。
		○ 缺点：对于现在的这类大模型来说，它的训练数据是非常大的，直接通过知识图谱来对预训练模型或者说大模型中的训练数据做知识扩充没有必要。因为数据量已经足够大到能包含这些扩充的知识的。
	2. 把知识图谱本身的结构化信息保留，作为训练的时候的一个特殊的内容或者结构加在大模型里边，
		○ 缺点：不是特别容易，因为对大模型的结构有一些要求，至少 GPT 系列的不大会采用结构，还是通过某种方式转换成文本语料的一部分去做可能会更合适。
	3. Finetune：
		○ 缺点：在 GPT4 这种大级别情况下fine-tune很难，它自己的技术报告里面讲微调成本很高
	4. 外部检索(like今天早上讨论的langchain+neo4j/networkx)
		○ Motivation: You do not need to machine learn Obama's birthday evert time you need it, it costs a lot and does not guarantee correctness. Just query it.
		○ Google LaMDA/New Bing/Meta: ，把知识图谱做一个外部知识库来检索，做一个纯外挂。摆事实、讲道理的时候，摆事实部分去找知识图谱，讲道理部分再用语言模型。
		○ 外部检索存在一些查询的disambiguation问题，可以参考传统graph QA的方法解决
	5. 检索增强的大模型retrieval-augmented language modeling （NLP 2021及2022年十大突破的方向）
		○ 与4比较类似。随着大模型参数量越来越大，外挂知识图谱帮它去解决事实一致性以及时效性的问题。
		○ Example：Deepmind-RETRO, OpenAI-webGPT, Google-LaMDA, FAIR-Blender
	6. 其他小方向：（1）将知识图谱的链式关系和预训练模型进行融合。（2）将知识图谱作为一个约束加到训练模型里面，引入一个额外的任务。比如预训练模型是一个独立的任务，然后再单独用知识图谱训练一个表示学习模型，然后将这两个模型进行交互。通过知识图谱构建的表示学习的任务，是作为一个辅助任务帮助预训练模型进行效果的提升。

### LLMs for Knowledge Graphs
1. Enhancing Knowledge Graph Construction Using Large Language Models (Arxiv 2023) [[Paper](https://arxiv.org/pdf/2305.04676.pdf)]
2. Complex Logical Reasoning over Knowledge Graphs using Large Language Models (Arxiv 2023) [[Paper(https://arxiv.org/pdf/2305.01157)]
3. Enhanced Story Comprehension for Large Language Models through Dynamic Document-Based Knowledge Graphs (AAAI 2022) [[Paper](https://cdn.aaai.org/ojs/21286/21286-13-25299-1-2-20220628.pdf)]
4. Fusing topology contexts and logical rules in language models for knowledge graph completion (Information Fusion 2022) [[Paper](https://www.sciencedirect.com/science/article/pii/S1566253522001592)]
5. From Discrimination to Generation: Knowledge Graph Completion with Generative Transformer (WWW 2022) [[Paper](https://dl.acm.org/doi/pdf/10.1145/3487553.3524238)]
6. Path Language Modeling over Knowledge Graphsfor Explainable Recommendation (WWW 2022) [[Paper](https://dl.acm.org/doi/abs/10.1145/3485447.3511937)]
7. GraphGPT [[Github](https://github.com/varunshenoy/GraphGPT)]
8. CodeKGC: Code Language Model for Generative Knowledge Graph Construction (Arxiv, April 2023) [[Paper](https://arxiv.org/abs/2304.09048)]
9. LLMs for Knowledge Graph Construction and Reasoning: Recent Capabilities and Future Opportunities (Arxiv, May 2023) [[Paper](https://arxiv.org/pdf/2305.13168.pdf)]

### Knowledge Graphs for LLMs
1. Using Knowledge Graph data in Large Language Models (Keynote) [[Video](https://www.youtube.com/watch?v=SHHHJXwHeWM)]
2. SKILL: Structured Knowledge Infusion for Large Language Models (NAACL 2022, by Google Research) [[Paper](https://aclanthology.org/2022.naacl-main.113.pdf)]
3. Enriching contextualized language model from knowledge graph for biomedical information extraction (Briefings in Bioinformatics) [[Paper](https://academic.oup.com/bib/article/22/3/bbaa110/5854405)]
4. Barack's Wife Hillary: Using Knowledge-Graphs for Fact-Aware Language Modeling (ACL 2019) [[Paper](https://arxiv.org/pdf/1906.07241.pdf)]
> * knowledge graph language model (KGLM): a neural language model with mechanisms for selecting and copying facts from a knowledge graph that are relevant to the context.
5. Improving Commonsense in Vision-Language Models via Knowledge Graph Riddles [[Paper](https://arxiv.org/abs/2211.16504)]

### LLMs and Knowledge Graphs for Other Tasks (e.g., Information Extraction)
1. ChatGraph: Interpretable Text Classification by Converting ChatGPT Knowledge to Graphs (Arxiv, May 2023) [[Paper](https://arxiv.org/pdf/2305.03513.pdf)]
2. KG-BART: Knowledge Graph-Augmented BART for Generative Commonsense Reasoning (AAAI 2021) [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/16796)]
3. QA-GNN: Reasoning with Language Models and Knowledge Graphs for Question Answering (NAACL 2021) [[Paper](https://aclanthology.org/2021.naacl-main.45/)]
4. Knowledge Graph-Based Chatbot With GPT-3 and Neo4j (from Neo4j) [[Link](https://neo4j.com/developer-blog/knowledge-graph-based-chatbot-with-gpt-3-and-neo4j/)]
5. Integrate LLM workflows with Knowledge Graph using Neo4j and APOC [[Link](https://towardsdatascience.com/integrate-llm-workflows-with-knowledge-graph-using-neo4j-and-apoc-27ef7e9900a2)] ⭐
> * Solution 1: use LLMs to generate a Cypher statement that can be used to retrieve connected information from the database.
> * Solution 2: use the connection information to enrich the text embedding representations. Additionally, the enhanced information can be retrieved at query time to provide additional context to the LLM from which it can base its response. (used in this project)

### Related Works
1. ReGen: Reinforcement Learning for Text and Knowledge Base Generation using Pretrained Language Models (Arxiv 2021) [[Paper](https://arxiv.org/pdf/2108.12472.pdf)]
> From Graph to Text
2. Tutorial: Knowledge-Driven Vision-Language Encoding (CVPR 2023) [[Link](https://blender.cs.illinois.edu/tutorial/KnowledgeVLP/)]

### Other Resourses
1. Github Repo: KG-LLM-Papers [[Link](https://github.com/zjukg/KG-LLM-Papers)]
2. Github Repo: Awesome LLM-KGs [[Link](https://github.com/RManLuo/Awesome-LLM-KG)]


