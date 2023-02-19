# Project Document

## OsamaDabb, fjgao2buedu, vjain25, HZ2001, eamonniknafs, 2023-Feb-16 v0.1.0-dev_


## Overview

_A brief summary of the project based on initial research and stakeholder meetings. To the best of your abilities, 
explain at a high level the stakeholders’ desired outcome for the project as well as the potential business value or 
impact this project will have if successfully completed._



1. Situation and current issues
2. Key Questions
    1. What language is the NL(natural language) text written in?
    2. Will the database schema change overtime?
3. Hypothesis: Overview of how it could be done
4. Impact -- need further communication with the client


### A. Problem Statement: 

Vianey is a database which stors information from various industries and clients in JSON and spreadsheet format. We want to achieve the function that given a piece of plain text of human natural language, we shall generate a logical query that would obtain the data from Vianey database as desired.


### B. Checklist for project completion

_Provide a bulleted list of the concrete deliverables and artifacts that, when complete, define the completion of the
 project._



1. Deliverable 1
2. Deliverable 2


### C. Provide a solution in terms of human actions to confirm if the task is within the scope of automation through AI. 

_To assist in outlining the steps needed to achieve our final goal, outline the AI-less process that we are trying to 
automate with Machine Learning. Provide as much detail as possible._


### D. Outline a path to operationalization.

Operationlization is as important as the query tool we to build. This is because any technology is useless if people are unable to use it. There are several possible ways of operationalize the tool. First, creating a basic terminal interface that allows people to obtain data and generate output files would be sufficient for staff who have tech backgrounds; adding on to this, we could also containerize the tool into a Docker image for easier deployments. Second, we can deploy the tool in to a server, and create a web app which links to the database. By running the data query tool as a serverless function call, we are able to return and display the data on the web page for beter user experience. This solution will help more staff who does not have sufficient technical background to use this tool. 

## Resources

General Resources 
- https://odsc.medium.com/20-open-datasets-for-natural-language-processing-538fbfaf8e38

### Data Sets


* [WikiSQL](https://github.com/salesforce/WikiSQL)
* [The Blog Authorship Corpus](https://u.cs.biu.ac.il/~koppel/BlogCorpus.htm)


### References


1. [Seq2SQL: Generating Structured Queries from Natural Language using Reinforcement Learning](https://arxiv.org/abs/1709.00103)

## Weekly Meeting Updates

_Keep track of ongoing meetings in a google doc and link it to this markdown_

Example meeting notes [google doc](https://docs.google.com/document/d/1EQbzWQMvNOFHZhj7xVXqPxkXgTaWG6kHKtYo5y-USVo/edit?usp=sharing). You can create a copy of this document for your project and update the meeting document as the project progresses.
