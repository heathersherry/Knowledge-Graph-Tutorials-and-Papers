## Knowledge Graph Enhanced Machine Learning

### Surveys and Tutorials
1. Informed Machine Learning – A Taxonomy and Survey of Integrating Prior Knowledge into Learning Systems (TKDE 2021) [[Paper](https://arxiv.org/pdf/1903.12394.pdf)] 🌟
<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/kg_ml.png" width="400" class="center" />

### KG Integrated in Hypothesis Set (e.g., the definition of a neural network’s architecture and hyper-parameters, or choosing model structure)
<img src="https://github.com/heathersherry/Knowledge-Graph-Tutorials-and-Papers/blob/master/figures/kg_hs.png" width="400" class="center" />

#### (1) GNN + KGs as external sources

1. The more you know: Using knowledge graphs for image classification (CVPR 2017) [[Paper](https://arxiv.org/pdf/1612.04844.pdf)]
> * Inference about a particular object is facilitated by using relations to other objects in an image.
2. Symbolic graph reasoning meets convolutions (NIPS 2018)
> * A graph reasoning layer can be inserted into any neural network, which enhances the representations in a given layer by propagating through a given knowledge graph.

#### (2) Attention mechanisms on a knowledge graph in order to enhance features
1. Knowledge enhanced contextual word representations (EMNLP 2019)
> * Attention on related knowledge graph embedding can support the training of word embeddings.
2. Commonsense knowledge aware conversation generation with graph attention (IJCAI 2018)
> * Use attention on KG to facilitate the understanding and generation of conversational text.

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

### Knowledge-aware methods in XAI
1. A Survey of Data-driven and Knowledge-aware eXplainable AI (TKDE 2021)


## Related Reading
1. TensorFlow: Neural Structured Learning [[TF](https://www.tensorflow.org/neural_structured_learning)] [[GitHub](https://github.com/tensorflow/neural-structured-learning)]
* train neural networks by leveraging structured signals in addition to feature inputs. Structure can be explicit as represented by a graph, or implicit as induced by adversarial perturbation.
