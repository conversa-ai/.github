# Conversa project

Access to information is increasingly conversational. However, there is a lack of conversational AI training material for Spanish and the co-official languages, in general and for specific key tasks and domains. Additional barriers include steep computational costs for training conversational agents and challenging inference times, and a lack of guarantees for the safety and transparency of conversational systems. The CONVERSA project (TED2021-132470B-I00) constitutes a step forward to democratize access to conversational AI through computation and data efficient development and testing of innovative, open and safe resources in Spanish and co-official languages. The duration of the project is from December 2022 to November 2024.

Our objective is to increase the availability of resources and models for conversational AI in Spanish, as well as the co-official languages of Spain: Basque, Catalan, and Galician. To achieve this, we are developing a comprehensive collection of dialogue datasets and offering tools that allow for the reproducible creation of corpora for each segment of the dataset. 

Apart from corpora we also create both dialogue and QA interactive systems in diverse domains.

[Project description](https://drive.google.com/file/d/1nTvVLMz9zb7_VBXHkhmNSTrPmEPvPr3t/view?usp=sharing).

### Dialogue corpora

We are creating a collection of dialogue corpora in Spanish and co-official languages that is called "Spanish Dialogue Pile" soon to be released. 

So far, we released **ChatSubs** which is the dialogue corpora in Spanish and co-official languages created from the subtitles of movies and TV series (4 Gb). The corpora is available in [Zenodo](https://zenodo.org/record/8220853) and the code for the corpus creation is available in [our repository](https://github.com/conversa-ai/ChatSubs). The corpora is described in the following [paper](https://www.sciencedirect.com/science/article/pii/S2352340923006650):

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
}
```

We are also developing the corpora from Reddit discussions, Usenet forums and other online forums.  The final size of the corpus will exceed 30 Gb.

### Dialogue systems