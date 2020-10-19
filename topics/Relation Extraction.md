__Tutorial:__
1. A SURVEY ON RELATION EXTRACTION (CMU) [[Slides](http://www.cs.cmu.edu/~nbach/papers/A-survey-on-Relation-Extraction-Slides.pdf)]
2. Relation Extraction: CSE 517: Natural Language Processing [[Slides](https://courses.cs.washington.edu/courses/cse517/13wi/slides/cse517wi13-RelationExtraction.pdf)]
3. Relation Extraction II: CSE 517: Natural Language Processing [[Slides](https://courses.cs.washington.edu/courses/cse517/13wi/slides/cse517wi13-RelationExtractionII.pdf)]

__Papers:__
1. CoType: Joint Extraction of Typed Entities and Relations with Knowledge Bases (CoType, WWW2017)[[Notes]](
https://blog.csdn.net/hqc888688/article/details/73559365)
2. Knowledge-Based Weak Supervision for Information Extraction of Overlapping Relations [[Code](http://aiweb.cs.washington.edu/ai/raphaelh/mr/)][[Slides](https://www.slideserve.com/anila/knowledge-based-weak-supervision-for-information-extraction-of-overlapping-relations)]
> * Recently, researchers have developed multi- instance learning algorithms to combat the noisy training data that can come from heuristic labeling, but their models assume relations are disjoint . for example they cannot extract the pair Founded(Jobs, Apple) and CEO-of(Jobs, Apple). This paper presents a novel approach for multi-instance learning with overlapping relations that combines a sentence-level extraction model with a simple, corpus-level component for aggregating the individual facts. 
3. Modeling missing data in distant supervision for information extraction (ACL2013) missing data problem(?)
4. Neural Relation Extraction with Selective Attention over Instances (ACL 2016) [[Paper](http://www.aclweb.org/anthology/P16-1200)][[Code](https://github.com/thunlp/OpenNRE)][[Blog](https://zhuanlan.zhihu.com/p/22666876)]
> * Fix the problem of distant supervised relation extraction
> * Employs CNN to embed the semantics of sentences, then builds sentence-level attention over multi- ple instances, which is expected to dynamically reduce the weights of those noisy instances (major contribution). Notes in group meeting.
5. Multi-instance Multi-label Learning for Relation Extraction (EMMLP-CoNLL 2012)[[Paper](https://www.aclweb.org/anthology/D12-1042)]
6. Snuba: Automating Weak Supervision to Label Training Data (VLDB 2019) 🌟
7. Improving Neural Relation Extraction with Implicit Mutual Relations [[Video](https://www.google.com/url?q=https://drive.google.com/open?id%3D1Ksh1lBwJ0V2nopiLoh-Uk5eofJW6uRrA&sa=D&ust=1587488616483000&usg=AFQjCNEPrROfm72JmChuKgls7cAo2fniOA)][[Slides](https://www.google.com/url?q=https://drive.google.com/open?id%3D1hIfhz0qfPu9p44kWfhhywj_D8EF9eGX5&sa=D&ust=1587488616483000&usg=AFQjCNFpDtYPPYI16sI05NBwoLqUt8jtog)][[Paper](https://conferences.computer.org/icde/2020/pdfs/ICDE2020-5acyuqhpJ6L9P042wmjY1p/290300b021/290300b021.pdf)] (ICDE 2020) 🌟
8. Snorkel: rapid training data creation with weak supervision (VLDBJ 2020) 🌟
9. Snorkel: Fast Training Set Generation for Information Extraction (SIGMOD 2017) 🌟