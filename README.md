**Explainable Hybrid Document Retrieval for Amharic: Integrating BM25 and XLM-R
Overview**
This repository contains the dataset, source code, and experimental resources associated with the study“Explainable Hybrid Document Retrieval for Amharic: Integrating BM25 and XLM-R.” The work introduces an explainable hybrid information retrieval framework that combines the lexical matching capability of BM25 with the semantic representation power of an Amharic-fine-tuned XLM-R model. To improve transparency, the framework incorporates Local Interpretable Model-Agnostic Explanations (LIME) to explain retrieval decisions. The repository also includes a large-scale, domain-inclusive Amharic information retrieval dataset developed to support research in low-resource information retrieval.



├── models/
│   ├── bm25/
│   ├── xlmr/
│   └── hybrid/

│
├── README.md
└── requirements.txt
**Dataset Description**

The dataset was developed to address the limited availability of large-scale, domain-inclusive resources for Amharic information retrieval. Documents were collected from publicly accessible Ethiopian news sources and organized into query-document relevance pairs and distractor documents for realistic retrieval evaluation.

**Dataset Statistics**
Component	                Count
Queries	                  44,707
Relevant Documents	      44,707
Distractor Documents      19,258
Total Documents        	  63,965

The dataset spans eight domains:
Education
Technology
Religion
Agriculture and Business
Sports
National Affairs
International Affairs
Politics
The inclusion of distractor documents enables rigorous evaluation under realistic retrieval conditions and supports robustness analysis.

**Data Annotation**
Query-document relevance was annotated by domain experts using a three-level relevance scheme:

Label      	Description
2	          Relevant
1          	Partially Relevant
0	          Non-Relevant

Each instance was independently reviewed by two annotators, and disagreements were resolved through majority voting. Inter-annotator agreement, measured using Cohen’s κ, achieved a score of 0.78, indicating substantial agreement.
