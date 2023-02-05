# pyBibX

## Introduction

A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus**, **WOS (Web of Science)** and **PubMed** scientific databases. 

General Capabilities:
- a) Works with **Scopus**, **WOS** and  **PubMed** files 
- b) Identification and Removal of duplicates
- c) Identification of documents per type
- d) Generates an **EDA** (Exploratory Data Analysis) Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
- e) Creates an **ID** (Identification) for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
- f) Creates a **WordCloud** from the Abstracts, Titles, Authors Keywords or Keywords Plus
- g) Creates a **N-Gram Bar Plot (interactive plot)** from the Abstracts, Titles, Authors Keywords or Keywords Plus
- h) Creates a **Projection** of the documents based on the Abstracts, Titles, Authors Keywords or Keywords Plus
- i) Creates an **Evolution Plot** based on Abstracts, Titles, Sources, Authors Keywords or Keywords Plus
- j) Creates a **Sankey Plot (interactive plot)** with any combination of the following keys: Authors, Countries, Institutions, Journals, Auhors_Keywords, Keywords_Plus, and/or Languages
- k) Creates a **TreeMap** from the Authors, Countries, Institutions, Journals, Auhors_Keywords, or Keywords_Plus
- l) Creates an **Authors Productivity Plot (interactive plot)** It informs for each year the documents (IDs) published for each author
- m) Creates a **Bar Plot**  for the following statistics: Documents per Year, Citations per Year, Past Citations per Year, Lotka's Law, Sources per Documents, Sources per Citations, Authors per Documents, Authors per Citations, Authors per H-Index, Bradford's Law (Core Sources 1, 2 or 3), Institutions per Documents, Institutions per Citations, Countries per Documents, Countries per Citations, Language per Documents, Keywords Plus per Documents and Authors' Keywords per Documents

Network Capabilities:
- a) **Citation Analysis (interactive plot)** between Documents (Blue Nodes) and Citations (Red Nodes). Documents and Citations can be highlighted for better visualization
- b) **Collaboration Analysis (interactive plot)** between Authors, Countries, Institutions or **Adjacency Analysis (interactive plot)** between Authors' Keywords or Keywords Plus. Collaboration and Adjacency can be highlighted for better visualization
- c) **Similarity Analysis (interactive plot)** can be performed using coupling or cocitation methods
- d) **World MAP Collaboration Analysis (interactive plot)** between Countries in a Map

NLP (Natural Language Processing) Capabilities:
- a) **Topic Modelling** using BERTopic to cluster documents by theme
- b) Visualize topics distribution
- c) Visualize topics by the most representative words
- d) Visualize documents projection and clusterization by topic
- e) Visualize topics heatmap
- f) Find the most representative documents from each theme
- g) Find the most representative topics according to a word
- i) **Abstractive Text Summarization** using PEGASUS on a set of selected documents or all documents
- j) **Extractive Text Summarization** using BERT on a set of selected documents or all documents

Correction and Manipulation Capabilities:
- a) Filter the .bib file by Year, Sources, Bradford Law Cores, Countries, and/or Languages
- b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
- c) Merge different or same database files one at a time. The preference of information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)

## Usage

1. Install
```bash
pip install pyBibX
```

2. Try it in **Colab**:

- Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
- Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
- Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
- Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
- Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
- Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
- Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))

# Acknowledgement 
This section indicates the libraries that inspired pyBibX

* BERT (https://smrzr.io/)
- a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
- b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165

* BERTopic (https://maartengr.github.io/BERTopic/index.html)
- a) Github: https://github.com/MaartenGr/BERTopic
- b) Paper: GROOTENDORST, M. (2022). BERTopic: Neural Topic Modeling with a Class-based TF-IDF Procedure. arXiv. doi: https://doi.org/10.48550/arXiv.2203.05794

* Bibliometrix (https://www.bibliometrix.org/home/)
- a) Github: https://github.com/massimoaria/bibliometrix
- b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007

* Metaknowledge (http://www.networkslab.org/metaknowledge)
- a) Github: https://github.com/UWNETLAB/metaknowledge
- b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.

* PEGASUS (https://ai.googleblog.com/2020/06/pegasus-state-of-art-model-for.html?m=1)
- a) Github: https://github.com/huggingface/transformers
- b) Paper: ZHANG, J,; ZHAO, Y.; SALEH, M.; LIU, P.J. (2019). PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization. arXiv. doi: https://doi.org/10.48550/arXiv.1912.08777

And to all the people that helped to improve or correct the code. Thank you very much!

* Fabio Ribeiro von Glehn (29.DECEMBER.2022) - UFG - Federal University of Goias (Brazil)
