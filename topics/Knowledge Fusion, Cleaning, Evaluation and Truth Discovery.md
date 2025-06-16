## Knowledge Fusion, Data Fusion, and Truth Discovery

### 📝 Surveys
1. A Survey on Truth Discovery [[Paper](https://www.kdd.org/exploration_files/Article1_17_2.pdf)] 🌟
2. Truth Discovery Algorithms: An Experimental Evaluation [[Paper](https://arxiv.org/pdf/1409.6428.pdf)]
3. A survey on data fusion: what for? in what form? what is next? (Journal of Intelligent Information Systems, 2020) [[Paper](https://link.springer.com/article/10.1007/s10844-020-00627-4)]

### 📝 General Papers
__Data Fusion__
> I think this is a relatively old topic, people are moving to knowledge fusion since 2018.
> Actually there are many interesting small topics. e.g., single truth/multi-truth, copy detection, source reliability. I will classfiy the following papers later.
> However, I think data fusion/knowledge fusion will play an essential role in data processing in the pre-trained dataset in LLMs/LMs.
1. Truth Discovery with Multiple Conflicting Information Providers on the Web (TKDE 2008), the most classical one. 🌟
2. Integrating conflicting data: the role of source dependence (VLDB 2009), the most classical one. 🌟
3. Fusing data with correlations (SIGMOD 2014) 🌟
4. Truth discovery and copying detection in a dynamic world (VLDB 2009) 🌟
5. Global detection of complex copying relationships between sources (VLDB 2010) [[Paper](https://dl.acm.org/doi/pdf/10.14778/1920841.1921008)] 🌟 
6. Online data fusion (VLDB 2011) 🌟
7. Compact explanation of data fusion decisions (WWW 2013)
8. Truth finding on the Deep Web: Is the problem solved? (VLDB 2013) 🌟
9. A Confidence-Aware Approach for Truth Discovery on Long-Tail Data (VLDB 2014) 🌟
10. Dynamic Truth Discovery on Numerical Data (ICDM 2018) 🌟
11. Scaling up Copy Detection (ICDE 2015) 🌟

__Knowledge Fusion, Cleaning and Evaluation__
1. Knowledge Vault: A Web-Scale Approach to Probabilistic Knowledge Fusion (KDD 2014) [[Paper](http://lunadong.com/publication/kv_kdd.pdf)] 🌟
2. From data fusion to knowledge fusion (VLDB 2014) [[Paper](http://lunadong.com/publication/fromDFtoKF_vldb.pdf)] [[Slides](http://lunadong.com/talks/fromDFtoKF.pdf)] 🌟
3. Data X-Ray: A diagnostic tool for data errors (SIGMOD 2015) [[Paper](http://lunadong.com/publication/dataXray_sigmod.pdf)] [[Slides](http://lunadong.com/talks/dataXray_sigmod.pdf)] [[Demo](http://lunadong.com/publication/dataXray_vldbdemo.pdf)] 🌟
4. Knowledge-based trust: estimating the trustworthiness of web sources [[Paper](http://lunadong.com/publication/sonyaTrust_vldb.pdf)] [[Slides](http://lunadong.com/talks/KBT_vldb.pdf)]🌟
5. Knowledge verification for long tail verticals (VLDB 2017) 🌟
6. Efficient knowledge graph accuracy evaluation (VLDB 2019) [[Link](https://arxiv.org/abs/1907.09657)] 🌟
7. MIDAS: Finding the Right Web Sources to Fill Knowledge Gaps (ICDE 2019) 🌟
8. Distilling relations using knowledge bases (VLDBJ 2018) 🌟
> Given a relational table, we study the problem of detecting and repairing erroneous data, as well as marking correct data, using well curated knowledge bases (KBs). We propose detective rules (DRs), a new type of data cleaning rules that can make actionable decisions on relational data, by building connections between a relation and a KB. 
9. HoloDetect: Few-Shot Learning for Error Detection [[PDF](https://arxiv.org/pdf/1904.02285.pdf)], the same team of the HoloClean (SIGMOD 2019) 🌟
10. Unsupervised String Transformation Learning for Entity Consolidation [[PDF](https://cs.uwaterloo.ca/~ilyas/papers/DengICDE2019.pdf)] (ICDE 2019) 🌟
11. Normalization of Duplicate Records from Multiple Sources (TKDE 2019) 🌟
12. Selecting Data to Clean for Fact Checking: Minimizing Uncertainty vs. Maximizing Surprise (VLDB 2020) 🌟
13. Learning Over Dirty Data Without Cleaning [[Paper](https://doi.org/10.1145/3318464.3389708)] (SIGMOD 2020) 🌟
14. CoClean: Collaborative Data Cleaning [[Paper](https://doi.org/10.1145/3318464.3384698)] (SIGMOD 2020, demo) 🌟
15. T-REx: Table Repair Explanations [[Paper](https://doi.org/10.1145/3318464.3384700)] (SIGMOD 2020, demo) 🌟
16. Triple Trustworthiness Measurement for Knowledge Graph (WWW 2019)
17. Tracy: Tracing Facts over Knowledge Graphs and Text (WWW 2019, short)
18. Few-Shot Knowledge Validation using Rules (WWW 2021) [[Paper](https://mott.in/papers/LosterWWW2021COLT.pdf)]
19. Two Heads are Better than One: Zero-shot Cognitive Reasoning via Multi-LLM Knowledge Fusion (CIKM 2024) [[Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679744)] 🔥

__KG Fact Checking__
1. GraphCheck: Breaking Long-Term Text Barriers with Extracted Knowledge Graph-Powered Fact-Checking (ACL 2025)

__Vandalism Detection__
1. Debiasing Vandalism Detection Models at Wikidata (WWW 2019)

__Malicious Participant Detection__
1. Truth discovery for spatio-temporal events from crowdsourced data (VLDB 2017) [[Paper](https://dl.acm.org/doi/pdf/10.14778/3137628.3137662)] 🌟
2. Resolving conflicts in heterogeneous data by truth discovery and source reliability estimation (SIGMOD 2014) [[Paper](https://dl.acm.org/doi/pdf/10.1145/2588555.2610509)] 🌟 (only mention malicious sources in one sentence)
3. Reputation-Aware Data Fusion and Malicious Participant Detection in Mobile Crowdsensing (2018 IEEE International Conference on Big Data (Big Data)) [[Paper](https://ieeexplore.ieee.org/abstract/document/8622335)]

### 📊 Datasets
1. Fusion Datasets [[Link](http://lunadong.com/fusionDataSets.htm)]

### 💬 Notes
1. Data Fusion – Resolving Data Conflicts for Integration [[Tutorial Proposal](http://lunadong.com/publication/fusion_vldbTutorial.pdf)]
2. Data Integration and Machine Learning: A Natural Synergy
