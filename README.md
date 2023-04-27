# ml-ffi-intelligent-query-builder

## Table of Contents
1. [Introduction](#introduction)
2. [Installation Instuctions](#installation-instuctions)
3. [Sample Usage](#sample-usage)
4. [Data](#data)
5. [Risks and Limitations](#risks-and-limitations)
6. [Evaluation](#evaluation)
7. [Recommendations](#recommendations)
8. [More Information](#more-information)

## Introduction
This repository contains a software method to process natrual language (English preferred) into mongoDB queries. This project is mainly built for Vianey, Freedom for Immigrants project. Vianey is a database which stores information from various industries and clients in JSON and spreadsheet format. By following the pipeline provided in this file or following the API guide, one should be able to produce a logical mongoDB query by entering correct parameters.

A more accurate description can be found in the path [./project-structure/project-document.md](./project-structure/project-document.md).   

Dependencies can be found in ``requirments.txt``, or click [here](./requirements.txt).

## Background & Research
There are few previous research being done in the exact topic as what we are facing, which is converting natural language to NoSQL database, such as MongoDB, queries languages. However, there are existing projects that deals with natural language <==> SQL queries, which determines our route of solving this problem. 

More details could be found in our research file [here](./project-research/research.md)


## Installation Instuctions

To successfully run the pipeline. 
First, make sure you are using python version `≥ python3.8.5`. 

### [Optional] to ensure, create and activate virtual environment for dependency management.
`python3 -m venv .env`  

Activate virtual env:
`source .env/bin/activate`

Then, run:  
`<your python environment> -m pip install requirements.txt` <br>

> note: all other dependencies should be resolved in the Jupyter notebooks. 

### Prerequisite
[requirements](requirements.txt)

### Deployment
[Deployment](src/Deployment.ipynb)

## Sample Usage
how to use

## Data
about data

## Risks and Limitations
This section identifies foreseeable harms and misunderstandings.

## Evaluation

[Proof_of_Concept](src/Proof_of_Concept.ipynb)

In the Proof of Concept, at the bottom you will see a few sample queries followed by what the computer returned for those queries. Under that, you will see the manually written expected queries. The computer creates a set of valid queries with two points to note. As pointed out in the Proof of Concept, one of the queries has a redundant statement that isn't inaccurate but just extraneous. Another point to note was that one should be careful when using words like "last year" or "this month" because the computer doesn't necessarily know the current time and date, as seen in the last query. 


## Recommendations
This section provides information on warnings and potential mitigations.

## More Information
### Research
TODO: Briefly summarize research and point to long-form research files
[research](project-research/research.md)

### EDA
[FFI_EDA-2](src/FFI_EDA-2.ipynb)

## TODO
[BLOOM](https://huggingface.co/bigscience/bloom)

## maybe something else

## Add Users

To add yourself to the repository, open a Pull Request modifying `COLLABORATORS`, entering your GitHub username in a newline.

All Pull Requests must follow the Pull Request Template, with a title formatted like such `[Project Name]: <Descriptive Title>`

## [Project Outline](./project-structure/project-document.md)

Create branch: {yourname}Outline{...} from 'outline'.

Commit changes to your branch.

Merge changes from outline branch to your branch.(?)

**Create pull request!!!** and merge to the outline branch.

Delete your branch after merging. 
