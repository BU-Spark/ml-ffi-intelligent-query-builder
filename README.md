# ml-ffi-intelligent-query-builder

## Table of Contents
1. [Introduction](#introduction)
2. [Background & Research](#background&research)
3. [Installation Instuctions](#installation-instuctions)
4. [Sample Usage](#sample-usage)
5. [Data](#data)
6. [Risks and Limitations](#risks-and-limitations)
7. [Evaluation](#evaluation)
8. [Potential Improvements](#potential-improvements)
9. [More Information](#more-information)

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

### Use Instructions

On [this link](https://huggingface.co/spaces/spark-ds549/DS_549_Spring2023_FFI_Project), you will find an input UI where you can insert your OpenAI personal key and organization key as well as the English query that you want converted. If you do not have an organization key, type "None" for that field. After pressing submit, the MongoDB query should be outputted on the right. 

OpenAI's free personal API keys only allow a fixed number of queries. We recommending joining BU Spark's organization on OpenAI as keys generated from there will have a far higher number of queries available.

### Prerequisite
[requirements](requirements.txt)

### Project Structure:
- /src/ : contains the full project pipeline (Deployment.ipynb), EDA (EDA.ipynb), and the four csv files the we are using as a mock dataset (customer_data.csv, driver_data.csv, order_data.csv, cust_service_data.csv)
- /Project Research/ : contains all preliminary research done in the early development stage. 

### Deployment
[Deployment](src/Deployment.ipynb)

## Risks and Limitations
>This section identifies foreseeable harms and misunderstandings.
The entered content in the field "Plain Text Query" is passed as is to OpenAI SQL Translate API.

## Evaluation

[Proof_of_Concept](src/Proof_of_Concept.ipynb)

In the Proof of Concept, at the bottom you will see a few sample queries followed by what the computer returned for those queries. Under that, you will see the manually written expected queries. The computer creates a set of valid queries with two points to note. As pointed out in the Proof of Concept, one of the queries has a redundant statement that isn't inaccurate but just extraneous. Another point to note was that one should be careful when using words like "last year" or "this month" because the computer doesn't necessarily know the current time and date, as seen in the last query. 

## Potential Improvements
>This section provides information on potential improvements.

Continue with using OpenAI SQL translate:
1.  For better information security, encrypt recignized entities with random nouns and pass it to API, then replace the nouns back in the returned SQL query. 

Or replace API with custom trained model:
1. Train model for SQL translate.

## More Information
### Research
TODO: Briefly summarize research and point to long-form research files
[research](project-research/research.md)

### EDA
[FFI_EDA-2](src/FFI_EDA-2.ipynb)

## Add Users

To add yourself to the repository, open a Pull Request modifying `COLLABORATORS`, entering your GitHub username in a newline.

All Pull Requests must follow the Pull Request Template, with a title formatted like such `[Project Name]: <Descriptive Title>`

## [Project Outline](./project-structure/project-document.md)
