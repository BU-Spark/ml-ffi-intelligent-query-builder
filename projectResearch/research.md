This document is intended to track and explain our research progress toward our project. 

Papers found for general purposes are:

- "Seq2SQL: Generating Structured Queries from Natural Language using Reinforcement Learning" by Wang et al. (2018) 
    This paper introduces a model that learns to generate SQL queries from natural language input using a combination of sequence-to-sequence neural networks and reinforcement learning. 
- "Spider: A Large-Scale Human-Labeled Dataset for Complex and Cross-Domain Semantic Parsing and Text-to-SQL Task" by Yu et al. (2018) 
    This paper presents a dataset and a model that can generate SQL queries from natural language input for a variety of tasks, including complex queries and cross-domain queries.
- "Learning Structured Text Representations" by Matthew E. Peters et al. (2018) proposes a model for learning structured text representations based on constituency parsing. The model uses a self-attention mechanism to incorporate context and a tree-LSTM to model the hierarchical structure of the input.
- "A Fast and Accurate Dependency Parser using Neural Networks" by Danqi Chen and Christopher D. Manning (2014) introduces a fast and accurate dependency parser based on neural networks. The model is trained on large-scale datasets and uses a transition-based parsing algorithm.

Papers for converting Natrual language to MongoDB query language.

- "MANS: Mapping Natural Language to Structured Query Language for MongoDB" by Rishabh Bhardwaj et al. (2019)
    This paper presents a system for mapping natural language queries to MQL queries. The system consists of two components: a semantic parser and a query executor. The semantic parser uses a combination of handcrafted rules and machine learning techniques to parse the natural language query and generate an intermediate query representation. The query executor then maps this intermediate representation to the corresponding MQL query using a set of predefined mapping rules.

- "Natural Language to MongoDB Query Translation" by Hussain et al. (2019)
    This paper proposes a system for translating natural language queries to MQL queries using a combination of rule-based and machine learning techniques. The system first tokenizes and parses the natural language query using a rule-based parser, and then generates an intermediate query representation using a set of predefined rules. Finally, a machine learning model is used to map the intermediate representation to the corresponding MQL query.

Open Source Projects found:

- [Mongooseim](https://github.com/esl/mongooseim)

- [NaQL](https://github.com/shrinidhiraj/NaQL)

- [Stanford SQL-Net](https://github.com/stanfordnlp/stanfordnlp)


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



