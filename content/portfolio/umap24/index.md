---
title: "Improving Transformer-based Sequential Conversational Recommendations through Knowledge Graph Embeddings"
date: '2024-06-01'
jobDate: 2024
work: [RS, CRS, UMAP, KG, BERT]
techs: [RS, CRS, UMAP, KG, BERT]
thumbnail: /umap24/image.png
projectUrl: paper.pdf
projectname: "Improving Transformer-based Sequential Conversational Recommendations through Knowledge Graph Embeddings"
---

Conversational Recommender Systems (CRS) have recently drawn attention due to their capacity of delivering personalized recommendations through multi-turn natural language interactions. 
In this paper, we fit into this research line and we introduce a Knowledge-Aware Sequential Conversational Recommender System (KASCRS) that exploits *transformers* and *knowledge graph embeddings* to provide users with recommendations in a conversational setting.

In particular, KASCRS is able to predict a suitable recommendation based on the elements that are mentioned in a conversation between a user and a CRS. To do this, we design a model that: *(i)* encodes each conversation as a sequence of entities that are mentioned in the dialogue (*i.e.*, items and properties), and *(ii)* is trained on a *cloze* task, that is to say, it learns to predict the final element in the sequence -  that corresponds to the item to be recommended - based on the information it has previously seen.

The model has two main hallmarks: first, we exploit Transformers and *self-attention* to capture the sequential dependencies that exist among the entities that are mentioned in the training dialogues, in a way similar to session-based recommender systems. Next, we used *knowledge graphs* (KG) to improve the quality of the representation of the elements mentioned in each sequence. Indeed, we exploit knowledge graph embeddings techniques to pre-train the representation of items and properties, and we fed the input layer of our architecture with the resulting embeddings. In this way, KASCRS integrates both knowledge from the KGs as well as the dependencies and the co-occurrences emerging from conversational data, resulting in a more accurate representation of users and items. Our experiments confirmed this intuition, since KASCRS overcame several state-of-the-art baselines on two different datasets. 
