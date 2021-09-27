## Knowledge Graph Enhanced Machine Learning

### Surveys and Tutorials
1. Informed Machine Learning – A Taxonomy and Survey of Integrating Prior Knowledge into Learning Systems (TKDE 2021) [[Paper](https://arxiv.org/pdf/1903.12394.pdf)] 🌟
<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/kg_ml.png" width="400" class="center" />

### KG Integrated in Hypothesis Set (e.g., the definition of a neural network’s architecture and hyper-parameters, or choosing model structure)
<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/kg_hs.png" width="400" class="center" />

#### (1) GNN + KGs as external sources

1. The more you know: Using knowledge graphs for image classification (CVPR 2017) [[Paper](https://arxiv.org/pdf/1612.04844.pdf)] [[Notes](https://vitalab.github.io/article/2017/09/15/deepGraph.html)]
> * Inference about a particular object is facilitated by using relations to other objects in an image.
> * [Visual Genome](https://visualgenome.org/) is used as a source of the KG. "Specifically, we counted how often an object/object relationship or object/attribute pair occurred in the training set, and pruned any edges that had fewer than 200 instances. This leaves us with a graph over all of the images with each edge being a common relationship." Therefore, this is not the common knowledge graphs.
2. Symbolic graph reasoning meets convolutions (NIPS 2018)
> * A graph reasoning layer can be inserted into any neural network, which enhances the representations in a given layer by propagating through a given knowledge graph.

#### (2) Attention mechanisms on a knowledge graph in order to enhance features
1. Knowledge enhanced contextual word representations (EMNLP 2019)
> * Attention on related knowledge graph embedding can support the training of word embeddings.
2. Commonsense knowledge aware conversation generation with graph attention (IJCAI 2018)
> * Use attention on KG to facilitate the understanding and generation of conversational text.

#### (3) Others
1. Object Detection Meets Knowledge Graphs (IJCAI 2017)
> * This paper proposes a novel framework of knowledge-aware object detection, which enables the integration of external knowledge graphs into any object detection algorithm. 
> * The framework employs semantic consistency to quantify and generalize knowledge, which improves object detection through a re-optimization process to achieve better consistency with background knowledge.
> * [MIT ConceptNet](https://conceptnet.io) is used as a source of the KG. [[Reference](http://alumni.media.mit.edu/~hugo/publications/papers/BTTJ-ConceptNet.pdf)]

### KG Integrated in Training Data
The distant-supervision based training data augmentation works
1. Distant supervision for relation extraction without labeled data (ACL 2009)

### KG Integrated Learning Algorithms
1. Knowledge-powered deep learning for word embedding (Joint European Conf. machine learning and knowledge discovery in databases. Springer, 2014)
> * Known relations among words can be utilized as augmented contexts when computing word embeddings such as word2vec training.

### KG Integrated in Final Hypothesis
These works use the knowledge graphs to indicate whether the prediction is consistent with available knowledge.
1. Explicit retrofitting of distributional word vectors (ACL 2018)
> * Post-process word embeddings based on KG
> * Similar work: Counter-fitting word vectors to linguistic constraints (arxiv)
2. Object detection meets knowledge graphs (IJCAI 2017)
> * Predicted probabilities of a learning system can be refined using semantic consistency measures derived form KGs

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
