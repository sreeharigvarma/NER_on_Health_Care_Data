# NER on Health Care Data
CRF-based predictive model which can identify disease and treatment from the patient's interaction with doctors or ordering medicines online

## Table of Contents
* [Introduction](#introduction)
* [Problem Statement](#problem-statement)
* [Observation](#observation)
* [Approach](#approach)
* [Model Explanation](#model-explanation)
* [Dataset Explanation](#dataset-explanation)
* [Libraries Used](#libraries-used)
* [Contact](#contact)

## Introduction
A health tech company called **‘BeHealthy’**. They aim to connect the medical communities with millions of patients across the country.
BeHealthy has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions.

## Problem Statement
**BeHealthy** require <font color = 'aqua'>**predictive model**</font> which can <font color = 'lightgreen'>**identify disease and treatment**</font> from the patients interaction with doctor or ordering medicines online

## Observation
- Here, the idea is to extract the **useful information** from the text and in addition to that the **entity of the useful information** also needs to be identified.
- Because the information we are planning to extract from the statement/interactions between doctors and patients is related to medical terms which are not regularly used day-to-day words.

## Approach
- By observing the requirement, it is clearly visible that we have to process the textual sentence and identify the entities like **Disease and Treatment**. We can predict these all requirements using
        -  CRF (Conditional Random Field) classifier
- We will follow the below procedures:
1. Data preprocessing
2. Concept identification
3. Defining the features of CRF
4. Getting the features of words and sentences
5. Defining input and target variables
6. Building the model
7. Evaluating the model
8. Identifying the diseases and predicted treatment using a custom NER

## Model Explanation
1. For Medical Entity Recognition, we are building a CRF model which uses custom NER because the entities we are planning to recognise all are related to medical terminologies.
2. Luckily!! we received the dataset which contains sentences along with labels, labels/tags are very important for Entity recognition. *If your dataset is not labelled, you have to manually label the data for Model Building and Prediction*.

## Dataset Explanation
We have four data files for this activity to proceed, they are
1. Train Sentence Dataset
2. Train Label Dataset
3. Test Sentence Dataset
4. Test Label Dataset

The sentence file contains all interactions between patients and doctors and the Label file contains all entity tags for particular words arranged as per sentence. We need to do a few preprocessing while accessing the dataset we will explore that in further steps

## Libraries Used
1. Pandas - Dataframe, Content storage and processing
2. Regular Expression (re) - Identify the textual pattern
3. SpaCy - NLP, POS tag check
4. Warnings - To avoid warning messages
5. Sklearn_CRFsuite - Model building and Evaluation

## Contact
sreeharipkgvarma@gmail.com
