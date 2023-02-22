# Intelligent Query Builder

## OsamaDabb, fjgao2buedu, vjain25, HZ2001, eamonniknafs
### 2023-Feb-23 v0.1.3-dev_

### [Project description](https://docs.google.com/document/d/1XQ0WxdrtvXnMM5lx3uDSYdlVJYCoXyKLIrG7oPV5uUY)

## Overview

>_A brief summary of the project based on initial research and stakeholder meetings. To the best of your abilities, 
explain at a high level the stakeholders’ desired outcome for the project as well as the potential business value or 
impact this project will have if successfully completed._

Vianey, our database, is used to collect and store information about abuses suffered in immigration detention, requests for support from folks in detention, case management, bond fund, and several other buckets of work. Because our organization stores aggregate data from many different programs, we are often asked to run queries/pull data from a variety of different staff and partners. This is incredibly important, as it is used for various reports and campaigns, but it is very time consuming for staff. We would like for BU Spark! to design a query builder that will intake requests in plain language, turn them into logical queries, and pull the data. 

1. Situation and current issues
    1.Freedom For Immigrants (FFI) is an organization that is devoted to abolishing immigration detention, and fighting against injustices against immigrants. The FFI uses a database known as Vianey to organize case files, bond funds, and other important documents. Since this database stores aggregate data from multiple programs, they are often asked to run queries on the database, which is difficult and time consuming for their employees.
2. Key Questions
    1. What language is the NL(natural language) text written in?
    2. Will the database schema change overtime?
    3. Does the future user of this product know the exact entity names in the database?
    4. Will the future user try to use the exact entity names to build the query text?
    5. How much data is provided? 
    6. Do we need to build more data?
    7. **I think we need more ideas here!**
3. Hypothesis: Overview of how it could be done
    1. A program that is capable of translating plain language into SQL queries and then automatically querying the database for the expected output.
4. Impact -- need further communication with the client

### A. Problem Statement: 

Vianey is a database which stores information from various industries and clients in JSON and spreadsheet format. We want to achieve the function that given a piece of plain text of human natural language, we shall generate a logical query that would obtain the data from Vianey database as desired.

### B. Checklist for project completion

>_Provide a bulleted list of the concrete deliverables and artifacts that, when complete, define the completion of the
 project._

The final product will include two main deliverables:

A model that is able to spot the necessary entities in a plain English-language text request as well as the correlation among them. 
A method to convert the relations from deliverable 1 to an executable query on MongoDB.



### C. Provide a solution in terms of human actions to confirm if the task is within the scope of automation through AI. 

>_To assist in outlining the steps needed to achieve our final goal, outline the AI-less process that we are trying to 
automate with Machine Learning. Provide as much detail as possible._

Currently, when someone wants to operate on the data in the MongoDB database, they construct an SQL query on the fields using the relationships that bring the data together. This requires not only a strong understanding of SQL but also a deep knowledge of the different fields and technicalities of the MongoDB database. This is within the scope of automation of AI because the users know what output they want—they simply need something to simplify the process of pulling that output from the database. An NLP program that can understand the user’s query in normal text and translate it into query language would solve the issue. In simple terms, it is a translator from English to SQL. 

### D. Outline a path to operationalization.

Operationlization is as important as the query tool we to build. This is because any technology is useless if people are unable to use it. There are several possible ways of operationalize the tool. 
1. Creating a basic terminal interface that allows people to obtain data and generate output files would be sufficient for staff who have tech backgrounds; adding on to this, we could also containerize the tool into a Docker image for easier deployments. 
2. We can deploy the tool in to a server, and create a web app which links to the database. By running the data query tool as a serverless function call, we are able to return and display the data on the web page for beter user experience. This solution will help more staff who does not have sufficient technical background to use this tool. 

## Resources

General Resources 
- https://odsc.medium.com/20-open-datasets-for-natural-language-processing-538fbfaf8e38

### Data Sets

* [WikiSQL](https://github.com/salesforce/WikiSQL)
* [The Blog Authorship Corpus](https://u.cs.biu.ac.il/~koppel/BlogCorpus.htm)
* Finegan-Dollak, C., Kummerfeld, J. K., Zhang, L., Ramanathan, K., Sadasivam, S., Zhang, R., & Radev, D. (2018). Improving text-to-sql evaluation methodology. arXiv preprint arXiv:1806.09029. “Paper that discusses the state of the art in text-to-sql querying. Brings up significant points on the how query/question based querying impact the networks robustness against novel inputs. Also provides a labeled dataset to be used in the training of text-to-SQL networks.”
* Tao Yu, Rui Zhang, Kai Yang, Michihiro Yasunaga, Dongxu Wang, Zifan Li, James Ma, Irene Li, Qingning Yao, Shanelle Roman, et al. Spider: A large-scale human-labeled dataset for complex and cross-domain semantic parsing and text-to-sql task. arXiv preprint arXiv:1809.08887, 2018. “Spider—a large-scale, complex and cross-domain semantic parsing and text to-SQL dataset annotated by 11 college students. It consists of 10,181 questions and 5,693 unique complex SQL queries on 200 databases with multiple tables, covering 138 different domains.”


### References

1. [Seq2SQL: Generating Structured Queries from Natural Language using Reinforcement Learning](https://arxiv.org/abs/1709.00103)
2. Victor Zhong, Caiming Xiong, and Richard Socher. Seq2sql: Generating structured queries from natural language using reinforcement learning. CoRR, abs/1709.00103, 2017.
3. Xiaojun Xu, Chang Liu, and Dawn Song. Sqlnet: Generating structured queries from natural language without reinforcement learning. arXiv preprint arXiv:1711.04436, 2017.
4. Scholak, T., Li, R., Bahdanau, D., de Vries, H., & Pal, C. (2020). DuoRAT: towards simpler text-to-SQL models. arXiv preprint arXiv:2010.11119. 
“Simplified Text-to-SQL using relation-aware/vanilla transformers.”

## Docs

### Weekly Meeting Updates

>_Keep track of ongoing meetings in a google doc and link it to this markdown_

[2023-Feb-23](https://docs.google.com/document/d/17G_Ld7xJ7OJ66DFJCCklca7fR4LksfdMrXe1oqRW79Y)

Example meeting notes [google doc](https://docs.google.com/document/d/1EQbzWQMvNOFHZhj7xVXqPxkXgTaWG6kHKtYo5y-USVo/edit?usp=sharing). You can create a copy of this document for your project and update the meeting document as the project progresses.
