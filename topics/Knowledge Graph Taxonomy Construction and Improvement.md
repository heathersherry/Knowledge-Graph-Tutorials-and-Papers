### The Construction and Improvement of Taxonomy and Ontology

#### The traditional ontology in KGs (ontology = only the semantic layer)
* The ontology serves as a semantic schema in KGs, usually recorded in the form of `.owl` in RDF graphs. It represents the structure of a graph. 
* In summary, Knowledge Graph = Ontology (schema) + Graph Database (instances).
1. Top-k Graph Summarization on Large Hierarchical DAGs
2. SetExpan: Corpus-Based Set Expansion via Context Feature Selection and Rank Ensemble Jiaming
3. Customized Organization of Social Media Contents using Focused Topic Hierarchy Xingwei
4. Taxonomy Induction Using Hypernym Subsequences Amit
5. Probase: a probabilistic taxonomy for text understanding
6. Extending an Event-type Ontology: Adding Verbs and Classes Using Fine-tuned LLMs Suggestions (ACL 2023) [[Paper](https://aclanthology.org/2023.law-1.9/)]
7. Scientific Knowledge Graph and Ontology Generation using Open Large Language Models (NeurIPS 2024) [[Paper](https://openreview.net/pdf?id=kHsfqBhZjC)]
8. OG-RAG: Ontology-Grounded Retrieval-Augmented Generation For Large Language Models (EMNLP 2025) [[Paper](https://arxiv.org/html/2412.15235v1)] [[GitHub](https://github.com/microsoft/ograg2)]

#### The Palantir Ontology (ontology = semantic + kinect + dynamic)
* It seems that the concept of "Ontology" in Palantir is quite popular nowadays.
* However, there are **critical differences** between the Palantir Ontology and the ontology in general KGs. Please **do not refer them as the same concept**.
> * The ontology in Palantir has 3 layers, semantic + kinect + dynamic, while the ontology in general KGs only refers to the semantic layer.
> * The kenectic layer in Palantir Ontology is to bind/link the dynamic data from external data sources (e.g., Spark or Flink tables) to the schema layer, and to support manual or passive operations to update the schema. It facilitates the data investigation in militaries and financial areas where information or intelligence updates frequently.
> * The dynamic layer in Palantir Ontology is to maintain a service that evoke actions or functions while the states of the data linked to the schema staisfy certain predefined conditions. For example, while the White Blood Cell (WBC) reaches predefined threshold, the dynamic layer will be triggered to call a risk analysis procedure and set off potential alarm pipeline. That's why Palantir Ontology is quite popular in military, CIA and medical industry.
> * However, general KGs is to provide well-defined schema or classfication for the triples, entities and relations stored in KG. Compared with the "Ontology Graph" in Palantir, the general KG is more like a static "snapshot" of knowledge.
1. Palantir’s AI Strategy: Path to AI Dominance From Defense to Enterprise [[Link](https://www.klover.ai/palantir-ai-strategy-path-to-ai-dominance-from-defense-to-enterprise/)]
2. Palantir Ontology Architecture [[Link](https://www.palantir.com/docs/foundry/object-backend/overview/)]

#### The Microsoft Fabric Ontology (ontology = semantic + kinect)
* There are also **critical differences** between the Microsoft Fabric Ontology and the ontology in general KGs.
* The Microsoft Fabric Ontology is very close to the ontology in general KGs (a semantic layer!). BUT it also supports linking/binding to data (a kinect layer!).
1. What is ontology (preview)? [[Link](https://learn.microsoft.com/en-us/fabric/iq/ontology/tutorial-0-introduction?pivots=semantic-model)]
