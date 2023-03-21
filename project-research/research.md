This document is intended to track and explain our research progress toward our project. 

Papers found for general purposes are:

- ["Seq2SQL: Generating Structured Queries from Natural Language using Reinforcement Learning" by Wang et al. (2018)](https://arxiv.org/pdf/1709.00103.pdf)
    This paper introduces a model that learns to generate SQL queries from natural language input using a combination of sequence-to-sequence neural networks and reinforcement learning. 
- ["Spider: A Large-Scale Human-Labeled Dataset for Complex and Cross-Domain Semantic Parsing and Text-to-SQL Task" by Yu et al. (2018) ](https://aclanthology.org/D18-1425.pdf)
    This paper presents a dataset and a model that can generate SQL queries from natural language input for a variety of tasks, including complex queries and cross-domain queries.
- ["Learning Structured Text Representations" by Matthew E. Peters et al. (2018)](https://arxiv.org/pdf/2201.00490.pdf) proposes a model for learning structured text representations based on constituency parsing. The model uses a self-attention mechanism to incorporate context and a tree-LSTM to model the hierarchical structure of the input.
- ["A Fast and Accurate Dependency Parser using Neural Networks" by Danqi Chen and Christopher D. Manning (2014)](https://aclanthology.org/D14-1082.pdf) introduces a fast and accurate dependency parser based on neural networks. The model is trained on large-scale datasets and uses a transition-based parsing algorithm.
- ["Deep Learning Driven Natural Languages Text to SQL Query Conversion: A Survey"](https://arxiv.org/pdf/2208.04415.pdf)

Papers for converting Natrual language to MongoDB query language.

- ["Querying NoSQL with Deep Learning to Answer Natural Language Questions" by Sebastian Blank](https://www.researchgate.net/publication/329466362_Querying_NoSQL_with_Deep_Learning_to_Answer_Natural_Language_Questions)
- ["Natural Language To NoSQL Query Conversion using Deep Learning" by Pradeep T](https://deliverypdf.ssrn.com/delivery.php?ID=977064095013107093127003094097009104019054002084028050101111093093119017004111103011043053098015118055007099029119118094090027019055041077011069094115100104109081019042085031009081106064086027100090107088086006075023084026065122091106121069074109117106&EXT=pdf&INDEX=TRUE) 
- ["AI-based Question Answering system for NoSQL standard query"](https://ceur-ws.org/Vol-3058/Paper-088.pdf)



Open Source Projects Found:

- [Stanford SQL-Net](https://github.com/stanfordnlp/stanfordnlp)
- [SpaCy](https://spacy.io/) - This is a Python library for natural language processing. It includes tools for part-of-speech tagging, dependency parsing, named entity recognition, and more. It can be used for generating SQL queries from natural language text.
- [Stanza](https://stanfordnlp.github.io/stanza/) (formerly CoreNLP) - This is a natural language processing toolkit developed by the Stanford NLP Group. It includes tools for part-of-speech tagging, named entity recognition, dependency parsing, and more. It can be used for generating SQL queries from natural language text.
- [NLTK](https://www.nltk.org/) - This is a popular Python library for natural language processing. It includes tools for tokenization, stemming, part-of-speech tagging, and more. It can be used for generating SQL queries from natural language text.
- [OPENAI SQL translation](https://platform.openai.com/examples/default-sql-translate)
```
### Postgres SQL tables, with their properties:
#
# Facility(id, name)
# Incidents(id, type, date, content)
#
### Hotline calls in the 2022 in the Golden Gate
SELECT * FROM Incidents WHERE date BETWEEN '2022-01-01' AND '2022-12-31' AND facility_id = 1
```
Tested the openai example for sql translation, the ai can complete the part after SELECT. 
The table property is imagined. The generated query is reasonable, but it can't identify the 'Golden Gate' as a hypothetical facility name.


Other Useful Links:

- [Dependency Parser](https://www.quora.com/Natural-Language-Processing-What-are-some-of-the-best-libraries-starting-points-in-Ruby-for-translating-an-English-sentence-question-to-an-SQL-query-or-NoSQL-map-reduce)
- [Natural Language Processing With Neo4j - Mining Paradigmatic Word Associations](https://www.lyonwj.com/blog/nlp-with-neo4j)



Updated outline:

    Questions answered from the first outline:
    1. What language is the NL(natural language) text written in?
        English, spanish later on.
    2. Will the database schema change overtime?
        Yes, but now we should focus on the initial state of the database, based on the dataset that we are provided.
    3. Does the future user of this product know the exact entity names in the database?

    4. Will the future user try to use the exact entity names to build the query text?

    5. How much data is provided? 
        Sufficient data will be provided. (However, if we want to train the model successfully, we might have to write the query corresponding to the text)
    6. Do we need to build more data?

    Follow up questions after research:
    1.
    2. 



