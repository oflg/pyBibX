# pyBibX

## Introduction

A Bibliometric and Scientometric python library that uses the .bib file generated by the Scopus or WOS (Web of Science) scientific databases. 

General Capabilities:
- a) Works with **Scopus** or **WOS** .bib files
- b) Identification and Removal of duplicates
- c) Generates an **EDA** (Exploratory Data Analysis) Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
- d) Creates an **ID** (Identification) for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
- e) Creates a **WordCloud** from the Abstracts, Titles, Authors Keywords or Keywords Plus
- f) Creates a **N-Gram Bar Plot (interactive plot)** from the Abstracts, Titles, Authors Keywords or Keywords Plus
- g) Creates a **Projection** of the documents based on the Abstracts, Titles, Authors Keywords or Keywords Plus
- h) Creates a **Evolution Plot** based on Abstracts, Titles, Sources, Authors Keywords or Keywords Plus
- i) Creates a **Sankey Plot (interactive plot)** with any combination of the following keys: Authors, Countries, Institutions, Journals, Auhors_Keywords, Keywords_Plus, and/or Languages
- j) Creates a **TreeMap** from the Authors, Countries, Institutions, Journals, Auhors_Keywords, or Keywords_Plus
- k) Creates an **Authors Productivity Plot (interactive plot)** It informs for each year the documents (IDs) published for each author
- l) Creates a **Bar Plot**  for the following statistics: Documents per Year, Citations per Year, Past Citations per Year, Lotka's Law, Sources per Documents, Sources per Citations, Authors per Documents, Authors per Citations, Authors per H-Index, Bradford's Law (Core Sources 1, 2 or 3), Institutions per Documents, Institutions per Citations, Countries per Documents, Countries per Citations, Language per Documents, Keywords Plus per Documents and Authors' Keywords per Documents

Network Capabilities:
- a) **Citation Analysis (interactive plot)** between Documents (Blue Nodes) and Citations (Red Nodes). Documents and Citations can be highlighted for better visualization
- b) **Collaboration Analysis (interactive plot)** between Authors, Countries, Institutions or **Adjacency Analysis (interactive plot)** between Authors' Keywords or Keywords Plus. Collaboration and Adjacency can be highlighted for better visualization
- c) **Similarity Analysis (interactive plot)** can be performed using coupling or cocitation methods
- d) **World MAP Collaboration Analysis (interactive plot)** between Countries in a Map

NLP (Natural Language Processing) Capabilities:
- a) **Topic Modelling** using BERTopic to cluster documents by theme
- b) Visualize topics distribution
- c) Visualize topics by the most representative words
- d) Visualize topics heatmap
- e) Visualize documents projection and clusterization by topic
- f) Find the most representative documents from each theme
- g) Find the most representative documents according to a word or set of words

Correction and Manipulation Capabilities:
- a) Filter the .bib file by Year, Sources, Bradford Law Cores, Countries, and/or Languages
- b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 

## Usage

1. Install
```bash
pip install pyBibX
```

2. Try it in **Colab**:

- Example 01: 'Scopus'   .bib file ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
- Example 02: 'WOS'      .bib file ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
- Example 03: 'Your Own' .bib file ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))

# Acknowledgement 
This section indicates the libraries that inspired pyBibX

* BERTopic (https://maartengr.github.io/BERTopic/index.html)
- a) Github: https://github.com/MaartenGr/BERTopic
- b) Paper: GROOTENDORST, M. (2022). BERTopic: Neural Topic Modeling with a Class-based TF-IDF Procedure. arXiv. doi: https://doi.org/10.48550/arXiv.2203.05794

* Bibliometrix (https://www.bibliometrix.org/home/)
- a) Github: https://github.com/massimoaria/bibliometrix
- b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007

* Metaknowledge (http://www.networkslab.org/metaknowledge)
- a) Github: https://github.com/UWNETLAB/metaknowledge
- b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
