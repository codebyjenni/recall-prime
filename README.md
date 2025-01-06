# The Construct Validity of Social Power Recall Manipulations: Evidence from Text Analysis
Submission for **Academy of Management 2025**

---

## Table of Contents
1. [Abstract](#abstract)
2. [Studies Overview](#studies-overview)

---

## Abstract
How individuals with high or low power think, feel, and act is a core focus in organizational behavior and social psychology research. Many studies use power recall manipulations, asking participants to recall and write about a time they possessed or lacked power. While previous work has validated this method through manipulation checks and successful predictions, we argue that this is insufficient. We systematically assess both the recall experience and the produced text using memory characteristics scales and automated text analysis (compliance, sentiment, dictionary analyses, and topic modeling). Across multiple samples, we find: (1) 12.71% of participants write text that large language models flag as inconsistent with instructions, varying by platform and condition; (2) sentiment analysis reveals expected differences but with substantial variation and non-negative values for low-power conditions; (3) topic modeling shows both high- and low-power participants focus on professional topics, but low-power participants more frequently discuss personal relationships, health crises, and financial issues; (4) memory scales show low-power scenarios evoke more negative emotions, greater perceived importance, and more distant memories. These findings highlight distinct differences in recall experiences and event types between high- and low-power participants.

---

## Studies Overview

### Datasets
- **Dataset 1**: Publicly accessible data on the Open Science Framework (OSF) repository that used power recall prime manipulations based on Galinsky et al.’s (2003) studies. Additional file drawer studies were also included in this data source. This combined dataset contains 8400 responses.
- **Dataset 2**: Power recall prime manipulation study using instructions from Galinsky et al.’s (2003) paper on Prolific Academic to control for any instructional variance that could be found in the first combined dataset and to offer a more contemporary test of compliance rates. This second dataset contains 802 responses. 

### Study 1: Participant Compliance of Power Recall Prime Prompts
- **Objective:** Assess participant compliance rate of power recall manipulations by adapting an automated classification task described in [Gilardi, Alizadeh, and Kubli (2023)](https://www.pnas.org/doi/10.1073/pnas.2305016120) by using the ChatGPT API. 
- **Methods:** Compliance with the power recall prime instructions was coded using a process inspired by the automated coding tasks. We utilize the OpenAI API with the “gpt-3.5 turbo” model to determine the relevance of text responses to the power recall prime manipulations. 
- **Findings:** There are many irrelevant text responses (between 6-12%). Irrelevant texts included gibberish, non-response , and non-adherence with power recall instruction.

### Study 2: Sentiment Analysis
- **Objective:** Analyze the sentiment scores from participants’ power recall responses to evaluate whether the power manipulations influence participants’ emotional responses in a manner consistent with existing power theories.  
- **Methods:** We used a Valence Aware Dictionary and sEntiment Reasoner (VADER), a model specifically designed to capture sentiment with nuanced understanding of context and language [(Hutto & Gilbert, 2014)](https://ojs.aaai.org/index.php/icwsm/article/view/14550).
- **Findings:** High power scenarios generally evoke a mean positive sentiment, while low power scenarios tend to generate a mean negative sentiment. However, at least 25% of text responses do not align with the expected patterns of high and low power, indicating inconsistencies with the theoretical framework (nomological net) of these constructs

### Study 3: Topic Modeling
- **Objective:** Uncover the latent themes across power recall conditions by implementing a topic modeling technique on the text responses from participants. 
- **Methods:** We use BERTopic [(Grootendorst, 2022)](https://arxiv.org/abs/2203.05794), a topic modeling pipeline that leverages state-of-the-art transformer-based embeddings and clustering algorithms to generate coherent and contextually rich topics. 
- **Findings:** Participants in low power conditions tend to recall a wider range of events and topics (e.g., academics, accidence, financial issues, relationships with friends/family) compared to those in the high power and equal power condition (e.g., workplace dynamics). 

---
