---
title: "Instructing and Prompting Large Language Models for Explainable Cross-domain Recommendations"
date: '2024-06-01'
jobDate: 2024
work: [RS, CRS, RECSYS, LLM, CROSSDOMAIN, CDR]
techs: [RS, CRS, RECSYS, LLM, CROSSDOMAIN, CDR]
thumbnail: recsys24long/image.png
projectUrl: paper.pdf
projectname: "Instructing and Prompting Large Language Models for Explainable Cross-domain Recommendations"
---

In this paper, we present a strategy to provide users with explainable cross-domain recommendations (CDR) that exploits large language models (LLMs). Generally speaking, CDR is a task that is hard to tackle, mainly due to *data sparsity* issues. Indeed, CDR models require a large amount of data labeled in both *source* and *target* domains, which are not easy to collect. Accordingly, our approach relies on the intuition that the knowledge that is already encoded in LLMs can be used to more easily bridge the domains and seamlessly provide users with personalized cross-domain suggestions. 

To this end, we designed a pipeline to: *(a)* instruct a LLM to handle a CDR task; *(b)* design a personalized prompt, based on the preferences of the user in a *source* domain, and a list of items to be ranked in *target* domain; *(c)* feed the LLM with the prompt, in both *zero-shot* and *one-shot* settings, and process the answer in order to extract the recommendations and a natural language explanation. As shown in the experimental evaluation, our approach beats several established state-of-the-art baselines for CDR in most of the experimental settings, thus showing the effectiveness of LLMs also in this novel and scarcely investigated scenario.