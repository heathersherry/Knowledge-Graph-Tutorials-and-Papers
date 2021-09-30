## Knowledge Graphs Enhanced Machine Learning 

### Surveys and Tutorials
<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/kg_ml.png" width="400" class="center" />

1. Informed Machine Learning – A Taxonomy and Survey of Integrating Prior Knowledge into Learning Systems (TKDE 2021) [[Paper](https://arxiv.org/pdf/1903.12394.pdf)] 🌟
2. Knowledge graph semantic enhancement of input data for improving AI (IEEE Internet Computing 2020)
3. Exploiting knowledge graphs in industrial products and services: A survey of key aspects, challenges, and future perspectives (Computers in Industry 2021)


### Task 1: KGs Integrated During Pre-processing of Learning

In these works, KGs are utilized to enhance the training data. One popular direction is distant-supervision based training data augmentation for named entity recognition (NER) and relation extraction (You may refer to [[the NER and Entity Typing section](https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/topics/Named%20Entity%20Recoginition%2C%20Entity%20Extraction%20and%20Entity%20Typing.md)] for more details).
> * In general, neural networks take separate (1) training data, (2) knowledge concepts, and (3) related concepts from KGs as input.
> * Most works use the first input layer of the deep neural network architecture as the layer to augment training data with the KG. The remaining layers are application and task specific with loss computed at the last layer of the deep neural network. The end-to-end training of such a network results in learning the relative weighting between the training data and different concepts from the KG to handle the downstream tasks.
> * Chanlleges: (1) different data formats in training data and KG, (2) different weights?, (3) explanability?

1. Distant supervision for relation extraction without labeled data (ACL 2009)

### Task 2: KGs Integrated During In-processing of Learning
### Task 2.1: KGs Integrated in Hypothesis Sets

In these works, KG may be integrated in hypothesis sets, e.g., the definition of a neural network’s architecture and hyper-parameters, or choosing model structure. One classical example is as follows:

<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/kg_hs.png" width="400" class="center" />


#### (1) KGs as external sources

1. The more you know: Using knowledge graphs for image classification (CVPR 2017) [[Paper](https://arxiv.org/pdf/1612.04844.pdf)] [[Notes](https://vitalab.github.io/article/2017/09/15/deepGraph.html)]
> * Inference about a particular object is facilitated by using relations to other objects in an image.
> * [Visual Genome](https://visualgenome.org/) is used as a source of the KG. "Specifically, we counted how often an object/object relationship or object/attribute pair occurred in the training set, and pruned any edges that had fewer than 200 instances. This leaves us with a graph over all of the images with each edge being a common relationship." Therefore, this is not the common knowledge graphs.
2. Symbolic graph reasoning meets convolutions (NIPS 2018)
> * A graph reasoning layer can be inserted into any neural network, which enhances the representations in a given layer by propagating through a given knowledge graph.

Zero-shot learning where KGs are used as external information
1.  Zero-Shot Recognition via Semantic Embeddings and Knowledge Graphs (CVPR 2018)
> * Used the KG to directly generate novel object classifiers
2.  Rethinking Knowledge Graph Propagation for Zero-Shot Learning (CVPR 2019)
3.  Multi-Label Zero-Shot Learning with Structured Knowledge Graphs (CVPR 2018)
4.  Semantics-Preserving Graph Propagation for Zero-Shot Object Detection (IEEE TRANSACTIONS ON IMAGE PROCESSING 2020)
5.  All About Knowledge Graphs for Actions (arxiv 2020) [[Paper](https://arxiv.org/pdf/2008.12432.pdf)]

#### (2) Attention mechanisms on a knowledge graph in order to enhance features
1. Knowledge enhanced contextual word representations (EMNLP 2019)
> * Attention on related knowledge graph embedding can support the training of word embeddings.
2. Commonsense knowledge aware conversation generation with graph attention (IJCAI 2018)
> * Use attention on KG to facilitate the understanding and generation of conversational text.

#### (3) Others
1. Co-training Embeddings of Knowledge Graphs and Entity Descriptions for Cross-lingual Entity Alignment (IJCAI 2018)
2. Deep Reasoning with Knowledge Graph for Social Relationship Understanding (IJCAI 2018)
3. Out of the Box: Reasoning with Graph Convolution Nets for Factual Visual Question Answering (NIPS 2018)
4. Large-Scale Object Classification using Label Relation Graphs (ECCV 2014) [[Paper](https://www.cs.princeton.edu/~jiadeng/paper/deng2014large.pdf)]
* This work introduces semantic relations including mutual exclusion, overlap, and subsumption, as constraints in the loss function to train the classifiers. 
5. Knowledge-Embedded Routing Network for Scene Graph Generation (CVPR 2019)
* This work formally represents the statistical knowledge in the form of a structured graph, and incorporates the graph into deep propagation network as extra guidance. In this way, it can effectively regularize the distribution of possible relationships of object pairs (so that the long-tail relationships are also captured) and thus make prediction less ambiguous.
6. I Know the Relationships: Zero-Shot Action Recognition via Two-Stream Graph Convolutional Networks and Knowledge Graphs (AAAI 2019)
*  A novel ZSAR framework to directly and collectively model all the three types of relationships between action-attribute, action-action, and attribute-attribute by incorporating a knowledge graph in an end-to-end manner. The KG is based on [ConceptNet 5.5](https://arxiv.org/abs/1612.03975).

### Task 2.2: KGs Integrated in Learning Algorithms

These works integrate graph knowledge into learning. Specifically, numerous NLP works (such as those in entity disambiguation and entity linking) utilize the relations between words or entities to learn their embeddings (you may refer the [[Entity Linking and Disambiguation section](https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/topics/Entity%20Linking%20and%20Entity%20Disambiguation.md)] and the [[KG Embedding and Reasoning section](https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/topics/Knowledge%20Graph%20Embedding%2C%20Learning%2C%20Reasoning%2C%20Rule%20Mining%2C%20and%20Path%20Finding.md)] for more details).

1. Knowledge-powered deep learning for word embedding (Joint European Conf. machine learning and knowledge discovery in databases. Springer, 2014)
> * Known relations among words can be utilized as augmented contexts when computing word embeddings such as word2vec training.
2. Rule-enhanced iterative complementation for knowledge graph reasoning (Information Science 2021)
> * A multi-relational GCN with attentive message passing is introduced as the triple discriminator. It acquires the structural information of KGs by aggregating neighbour relations and entities. 

### Task 3: KGs Integrated During Post-processing of Learning

These works use the knowledge graphs in final hypothesis, which indicates whether the prediction is consistent with available knowledge.

1. Explicit retrofitting of distributional word vectors (ACL 2018)
> * Post-process word embeddings based on prior knowledge
> * Similar work: Counter-fitting word vectors to linguistic constraints (arxiv)
2. Object detection meets knowledge graphs (IJCAI 2017)
> * Predicted probabilities of a learning system can be refined using semantic consistency measures derived form KGs
> * This paper proposes a novel framework of knowledge-aware object detection, which enables the integration of external knowledge graphs into any object detection algorithm. 
> * The framework employs semantic consistency to quantify and generalize knowledge, which improves object detection through a re-optimization process to achieve better consistency with background knowledge.
> * [MIT ConceptNet](https://conceptnet.io) is used as a source of the KG. [[Reference](http://alumni.media.mit.edu/~hugo/publications/papers/BTTJ-ConceptNet.pdf)]



## Knowledge-aware methods in XAI
### Surveys and Tutorials
1. A Survey of Data-driven and Knowledge-aware eXplainable AI (TKDE 2021)
> * The second part of this survey discusses the KG based methods

### General Papers
#### Internal rules: consider KG when designing the models (nowadays mainly used in recommendation systems)
1. Entity Suggestion with Conceptual Explanation (IJCAI 2017)

#### External rules: combines KG and reasoning to generate explanations without changing the model structures (produces mapping between input-output behavious)
1. Enabling Trust in Clinical Decision Support Rcommendations through Semantics (CEUR 2019)




## Related Reading
1. TensorFlow: Neural Structured Learning [[TF](https://www.tensorflow.org/neural_structured_learning)] [[GitHub](https://github.com/tensorflow/neural-structured-learning)]
* Train neural networks by leveraging structured signals in addition to feature inputs. Structure can be explicit as represented by a graph, or implicit as induced by adversarial perturbation.
2. Yoshua Bengio: From System 1 Deep Learning to System 2 Deep Learning (NeurIPS 2019) [[Video](https://www.youtube.com/watch?v=T3sxeTgT4qc)]
3. Cognitive Graph for Multi-Hop Reading Comprehension at Scale (ACL 2019) [[GitHub](https://github.com/THUDM/CogQA)] [[Notes](https://zhuanlan.zhihu.com/p/72981392)]
> * Cognitive Graph is not directly equal to Knowledge Graph. You can view CG as a (dynamic, partial, local) KG generated instantly from the query.
