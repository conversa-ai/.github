# Conversa project

Access to information is increasingly conversational. However, there is a lack of conversational AI training material for Spanish and the co-official languages, in general and for specific key tasks and domains. Additional barriers include steep computational costs for training conversational agents and challenging inference times, and a lack of guarantees for the safety and transparency of conversational systems. The CONVERSA project (TED2021-132470B-I00) constitutes a step forward to democratize access to conversational AI through computation and data efficient development and testing of innovative, open and safe resources in Spanish and co-official languages. The duration of the project is from December 2022 to November 2024.

Our objective is to increase the availability of resources and models for conversational AI in Spanish, as well as the co-official languages of Spain: Basque, Catalan, and Galician. To achieve this, we are developing a comprehensive collection of dialogue datasets and offering tools that allow for the reproducible creation of corpora for each segment of the dataset. 

Apart from corpora we also create both dialogue and QA interactive systems in diverse domains.

### Dialogue corpora

We are creating a collection of dialogue corpora in Spanish and co-official languages that is called "Spanish Dialogue Pile". So far, we have worked on the following corpora:

1. ChatSubs which is the dialogue corpora in Spanish and co-official languages created from the subtitles of movies and TV series. The corpora is available in [Zenodo](https://zenodo.org/record/8220853) and the code for the corpus creation is available in [our repository](https://github.com/conversa-ai/ChatSubs). The corpora is described in the following [paper](https://www.sciencedirect.com/science/article/pii/S2352340923006650):

```
@article{KHARITONOVA2023109565,
    title = {ChatSubs: A dataset of dialogues in Spanish, Catalan, Basque and Galician extracted from movie subtitles for developing advanced conversational models},
    journal = {Data in Brief},
    volume = {50},
    pages = {109565},
    year = {2023},
    issn = {2352-3409},
    doi = {https://doi.org/10.1016/j.dib.2023.109565},
    url = {https://www.sciencedirect.com/science/article/pii/S2352340923006650},
    author = {Ksenia Kharitonova and Zoraida Callejas and David Pérez-Fernández and Asier Gutiérrez-Fandiño and David Griol},
    keywords = {Dialogue, Conversation, Chatbots, Conversational AI, Speech, Natural language processing},
    abstract = {The ChatSubs dataset [5] contains dialogue data in Spanish and three of Spain's co-official languages (Catalan, Basque, and Galician). It has been obtained from OpenSubtitles, from which we have gathered the movie subtitles in our languages of interest and processed them to generate clearly segmented dialogues and their turns. The data processing code is publicly accessible. The result is 206.706 JSON files with more than 20 million dialogues and 96 million turns, which represents one of the biggest dialogue corpus available, as other similar datasets in better resourced languages do not reach 500k dialogues or present less defined conversations. Thus, the ChatSubs dataset is an ideal resource for research teams that are interested in training dialogue models in Spanish, Catalan, Basque, and Galician.}
}
```

2. Usenet-based corpus that represents dialogues extracted from Usenet forums.
3. A corpus derived from dialogues sourced from Reddit discussions.
4. A corpus based on dialogues taken from various online forums.
5. A corpus drawn from dialogues found in the proceedings of the European Parliament, based on Europarl data.

We are considering more corpora to come.

### Dialogue systems