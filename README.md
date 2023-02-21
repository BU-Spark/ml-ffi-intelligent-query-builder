# ml-ffi-intelligent-query-builder

# Add Users

To add yourself to the repository, open a Pull Request modifying `COLLABORATORS`, entering your GitHub username in a newline.

All Pull Requests must follow the Pull Request Template, with a title formatted like such `[Project Name]: <Descriptive Title>`

# Project Outline

Create branch: {yourname}Outline{Edit}? from 'outline'.

Commit changes to your branch.

Create pull request and merge to the outline branch.

Delete your branch after merging. 

# Overview

Situation and current issues:
Freedom For Immigrants (FFI) is an organization that is devoted to abolishing immigration detention, and fighting against injustices against immigrants. The FFI uses a database known as Vianey to organize case files, bond funds, and other important documents. Since this database stores aggregate data from multiple programs, they are often asked to run queries on the database, which is difficult and time consuming for their employees.

Key Questions

Hypothesis: Overview of how it could be done
A program that is capable of translating plain language into SQL queries and then automatically querying the database for the expected output.
Impact



# A. Problem Statement:
In as direct terms as possible, provide the “Data Science” problem statement version of the overview. Think of this as translating the above into a more technical definition to execute on.

# B. Checklist for project completion

The final product will include two main deliverables:

A model that is able to spot the necessary entities in a plain English-language text request as well as the correlation among them. 
A method to convert the relations from deliverable 1 to an executable query on MongoDB.

# C. Provide a solution in terms of human actions to confirm if the task is within the scope of automation through AI.

Currently, when someone wants to operate on the data in the MongoDB database, they construct an SQL query on the fields using the relationships that bring the data together. This requires not only a strong understanding of SQL but also a deep knowledge of the different fields and technicalities of the MongoDB database. This is within the scope of automation of AI because the users know what output they want—they simply need something to simplify the process of pulling that output from the database. An NLP program that can understand the user’s query in normal text and translate it into query language would solve the issue. In simple terms, it is a translator from English to SQL. 

# D. Outline a path to operationalization.
Data Science Projects should have an operationalized end point in mind from the onset. Briefly describe how you see the tool produced by this project being used by the end user beyond a jupyter notebook or proof of concept. If possible, be specific and call out the relevant technologies

# Resources
Data Sets
- Finegan-Dollak, C., Kummerfeld, J. K., Zhang, L., Ramanathan, K., Sadasivam, S., Zhang, R., & Radev, D. (2018). Improving text-to-sql evaluation methodology. arXiv preprint arXiv:1806.09029. “Paper that discusses the state of the art in text-to-sql querying. Brings up significant points on the how query/question based querying impact the networks robustness against novel inputs. Also provides a labeled dataset to be used in the training of text-to-SQL networks.”
- Tao Yu, Rui Zhang, Kai Yang, Michihiro Yasunaga, Dongxu Wang, Zifan Li, James Ma, Irene Li, Qingning Yao, Shanelle Roman, et al. Spider: A large-scale human-labeled dataset for complex and cross-domain semantic parsing and text-to-sql task. arXiv preprint arXiv:1809.08887, 2018. “Spider—a large-scale, complex and cross-domain semantic parsing and text to-SQL dataset annotated by 11 college students. It consists of 10,181 questions and 5,693 unique complex SQL queries on 200 databases with multiple tables, covering 138 different domains.”

References
- Victor Zhong, Caiming Xiong, and Richard Socher. Seq2sql: Generating structured queries from natural language using reinforcement learning. CoRR, abs/1709.00103, 2017.
- Xiaojun Xu, Chang Liu, and Dawn Song. Sqlnet: Generating structured queries from natural language without reinforcement learning. arXiv preprint arXiv:1711.04436, 2017.
- Scholak, T., Li, R., Bahdanau, D., de Vries, H., & Pal, C. (2020). DuoRAT: towards simpler text-to-SQL models. arXiv preprint arXiv:2010.11119. 
“Simplified Text-to-SQL using relation-aware/vanilla transformers.”

