# Conversa project

Access to information is increasingly conversational. However, there is a lack of conversational AI training material for Spanish and the co-official languages, in general and for specific key tasks and domains. Additional barriers include steep computational costs for training conversational agents and challenging inference times, and a lack of guarantees for the safety and transparency of conversational systems. The CONVERSA project (TED2021-132470B-I00) constitutes a step forward to democratize access to conversational AI through computation and data efficient development and testing of innovative, open and safe resources in Spanish and co-official languages. The duration of the project is from December 2022 to November 2024.

Our objective is to increase the availability of resources and models for conversational AI in Spanish, as well as the co-official languages of Spain: Basque, Catalan, and Galician. To achieve this, we have compiled and processed a large-scale conversational corpus containing tens of millions of dialogues in Spanish, Catalan, Basque, and Galician. This corpus represents a valuable resource for the scientific community, as no other comparable resource exists in terms of size, linguistic diversity, and quality.

Apart from corpora we also create both dialogue and QA interactive systems in diverse domains.

[Project description](https://drive.google.com/file/d/1nTvVLMz9zb7_VBXHkhmNSTrPmEPvPr3t/view?usp=sharing).

## Dialogue corpora

We are creating a collection of dialogue corpora in Spanish and co-official languages that is called **Spanish Dialogue Pile** soon to be released. 

### OpenSubtitles

So far, we released **ChatSubs** which is the dialogue corpora in Spanish and co-official languages created from the subtitles of movies and TV series (4 Gb). The corpora is available in [Zenodo](https://zenodo.org/record/8220853) and the code for the corpus creation is available in [our repository](https://github.com/conversa-ai/ChatSubs). The corpora is described in the following [paper](https://www.sciencedirect.com/science/article/pii/S2352340923006650):

### Usenet

We processed the information contained in newsgroups of Usenet, a decentralized network of user-generated content. Out of 279 Spanish-speaking groups we extracted 494,928 dialogues with 1,799,788 turns. The code for corpus creation is available at the [repository](https://github.com/conversa-ai/process_usenet).

### Forums

For this part of corpus we chose two popular public Spanish forums, [Meneame](https://www.meneame.net/) and [Mediavida](https://www.mediavida.com/). Additionally, we incorporated 51 of the largest Spanish subreddits from [Reddit](https://www.reddit.com/). 

We extracted the following data:
- 6,796,035 dialogues with 15,185,945 turns from 1,055,796 Reddit posts ([code](https://github.com/conversa-ai/processReddit)),
- 3,192,173 dialogues with 6,270,915 turns from 216,413 Meneame posts ([code](https://github.com/conversa-ai/processMeneame)),
- 307,818 dialogues with 683,978 turns from 43,281 Mediavida posts ([code](https://github.com/conversa-ai/processMediavida)).

### Books

Using [software](https://github.com/ricsinaruto/gutenberg-dialog) from [Czaky et Resky, The Gutenberg dialogue dataset](https://aclanthology.org/2021.eacl-main.11/), we processed the Spanish and Catalan books from the Project Gutenberg internet library. We extracted 64 dialogues with 463 turns for Catalan and 12,801 dialogues with 94,862 turns for Spanish.

### Total 

In total we obtained a corpus of 31,058,130 dialogues and 120,961,102 turns.

## Tools and open access
We have developed and implemented tools to:

* Collect, clean, and adapt the corpus for large-scale language model training.
* Track data sources efficiently at scale.
* Ensure proper processing to meet the technical requirements for LLM training.

The code for the tools is available on Conversa's [github](https://github.com/conversa-ai).

## Bias and Toxicity Mitigation
To address potential biases and toxic content, we have developed four comprehensive annotation guidelines focused on:

* Sexism
* Racism
* Homophobia
* Aporophobia

These guidelines guide the ongoing work of two annotators who are currently generating datasets with both positive and negative examples of sexism and racism. Although this work is still in progress, the foundational steps have been completed.

### Ethical AI and bias removal

Based on these annotations, we are developing and training models specifically designed to automatically reduce biases in language generation. These models will help ensure the creation of more ethical and accurate content in conversational AI systems.

## Fine-Tuning and Model Optimization

We are in the final stages of fine-tuning large-scale language models (LLMs) using the corpus. Initial results show that this corpus significantly enhances dialogue generation performance. Our fine-tuning process has focused on high-performance open-source models, such as LLaMA 3.1, recognized for its advanced capabilities in natural language understanding and generation.

The ultimate goal is to optimize these models to handle contextually appropriate and linguistically diverse dialogues across the target languages. This fine-tuning process is also designed to reduce biases in response generation, improving both the ethical quality and contextual accuracy of the outputs.

## Dialogue systems

We created a conversational question answering system based on Clinical Practice Guidelines (CPGs) created by the Aragonese Institute of Health Sciences (IACS) for the benefit of the Spanish National Health System. These guidelines are developed by a team of healthcare experts, and their purpose is to provide medical professionals with recommendations for patient care that are founded on solid scientific research.

We created a system based on Retrieval-Augmented Generation (RAG) with a Large Language Model (LLM) as a reasoning engine. Our approach serves as a step towards addressing the issues of hallucinated and false responses, as it allows developing explainable question answering systems based on trusted content. ([code]())

The system is described in the following [paper](https://www.tandfonline.com/doi/full/10.1080/0144929X.2024.2321959).

## References

1. [Kharitonova, K., Callejas, Z., Pérez-Fernández, D., Gutiérrez-Fandiño, A., & Griol, D. (2023). ChatSubs: A dataset of dialogues in Spanish, Catalan, Basque and Galician extracted from movie subtitles for developing advanced conversational models. Data in Brief, 50, 109565](https://doi.org/https://doi.org/10.1016/j.dib.2023.109565).
2. [Ksenia Kharitonova, & Griol, D. (2024). Incorporating evidence into mental health Q&A: a novel method to use generative language models for validated clinical content extraction. Behaviour & Information Technology, 1–18](https://doi.org/10.1080/0144929X.2024.2321959).
