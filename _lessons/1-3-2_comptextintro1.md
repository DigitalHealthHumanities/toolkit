---
layout: sublesson
structurehead: WhatisDH
lessontitle:
title: "The First Computational Text Analysis Project: The 'Index Thomisticus'"
group: "digital basics"
headabstract: "This lesson refreshes some of the discussions from the previous lesson concerning the identity of the digital humanities."
abstract: "This lesson will teach learners about different digital methods and how they fit into humanistic research."
lessonnumber: 2
lessonprint: 2
permalink: "/lessons/intro/comptextinto/2"
previouslesson: "/lessons/intro/comptextinto/1"
nextlesson: "/lessons/intro/comptextinto/3"
authors: cagostini
---

A pivotal project that marked the inclusion of digital scholarship began with Father Roberto Busa, S.J., and his Index Thomisticus (in Latin, “Index of St Thomas Aquinas”). Busa made a concordance of the corpus, or collected works, of St Thomas Aquinas (https://www.britannica.com/biography/Saint-Thomas-Aquinas), who is a Doctor of the Church. Aquinas, an Italian Dominican friar and priest, is regarded as the foremost Scholastic thinker due to the profound impact of his theological treatises, commentaries, and philosophical writings. The Corpus Thomisticum, the collected works of St Thomas Aquinas, encompasses approximately 11 million words. Father Busa’s work represents an initiative in **computational linguistics**—a field now recognized as part of **Digital Humanities (DH)**.

Previous concordances, such as the one compiled by James Strong, the [Concordance of the Bible](https://www.google.com/books/edition/The_Exhaustive_Concordance_of_the_Bible/3TBGAQAAMAAJ?hl=en&gbpv=0) (1894), were created manually and listed thousands of words, including the 8,674 Hebrew words of the Old Testament and the 5,624 Greek words of the New Testament. This project took thirty-five years to complete. Knowing about the work of philologists, Father Busa believed there had to be a more efficient way to generate textual information, particularly with the aid of technology. 
The [Index Thomisticus project is now accessible online](https://www.corpusthomisticum.org/it/index.age). 

## From Corpus Linguistics to IBM 

Father Busa recognized the scale of the task ahead, especially if he attempted to produce a concordance by hand—an extensive process that would involve systematically ordering all words in a text alongside relevant metadata. In 1946, he became interested in creating a concordance of the corpus he studied–the works of [St. Thomas Aquinas](https://www.britannica.com/biography/Saint-Thomas-Aquinas).
 
Building on his doctoral research (1949), Father Busa planned to track **word occurrences** and the decision to work computationally gained traction after he began collaborating with **IBM** in 1949 (Busa 1951). Father Busa’s project, thus, combined theological studies with computer-based technologies. The Index Thomisticus aimed to make a comprehensive concordance of all St. Thomas Aquinas’s works and related texts, culminating in a series of fifty-six printed volumes completed in 1980.

## From Punch Cards to Machine-Readable Texts

Father Busa made significant efforts to collaborate with a leading technology company of his time. Through his Jesuit connections at Fordham University, he arranged a meeting with Thomas J. Watson, the President of IBM. This meeting led to his collaboration with Paul Tasman, an IBM engineer who was knowledgeable about contemporary data processing equipment. Punch cards, previously used for data storage, served as a medium for storing, sorting, and reporting data processed by punched card equipment and computers. 

Rockwell and Sinclair argued that the technology utilized by Busa and Tasman represented key innovations facilitating the application of data processing to unstructured text data. Consequently, Busa and Tasman’s humanistic perspective on technology and their goals influenced the algorithm they developed for the final product.[^1]

Their process with the punch cards generally followed these steps:

- **Keypunch**: Encoding words and phrases as patterns of punched holes on a card. This was done in two stages: 
   - First, a scholar forms phrases
   - Second, a punch card operator encodes phrases using keypunch technology.
- **Reproducing Punch**: Copying the encoded information onto multiple cards, with each card representing a single contextual entry.
- **Sorter**: Alphabetizing the decks of cards and grouping them by related classifications.
- **Tabulator**: Reading the data from the cards and printing it onto continuous-feed paper.
- **Collator**: Checking the accuracy of the transcriptions using multiple sets of cards, akin to the collation of variant texts in traditional textual studies.

Father Busa sought to go beyond the contextual interpretation of the texts so that he could renew the study of philology. By rigorously examining the semantic and lexical properties of St. Thomas Aquinas's writings, he devised his own algorithmic process for recording textual information using handwritten cards, reflecting a deeply traditional approach to text. Steven Jones discussed Busa’s technological innovation as follows:

> For Busa, mechanization was to serve {% include term.html term="hermeneutics" %}. He aimed to interpret, to reveal meaningful patterns, different dimensions of the language. It’s just that some dimensions were too extensive (while their evidence was too minute) to be grasped by the unassisted eye and mind of the reader across an oeuvre of over ten million words. Philosophical and theological questions drove his linguistic research, and this led him to develop the complex process of literary data analysis. Looked at another way, in the Jesuit tradition, Father Busa sought the divine presence in all things; IBM’s punched-card machinery was at first only a means to this ultimate end.[^2]

{% include definition.html term="Hermeneutics" definition="Hermeneutics refers to the philosophical field that describes the process of reading and understanding texts." %} 

Father Busa recognized the significance of **deep reading** and connected it to the **Jesuit tradition of scholarship**. He dedicated many years to his Index Thomisticus project, ultimately producing over fifty volumes containing a concordance of Aquinas's works. During this process, he established a **linguistics center in Gallarate, Italy**, which trained many technical workers in the complex IBM technology of the time. This center effectively served as a quasi-institute for Jesuit education in the region and connected with other institutions worldwide, including Georgetown University in Washington, D.C.

The main technology used was based on punched cards, which were modified versions of the IBM 80-column punch card, adapted to accommodate the replication and semantic information required for the concordance.[^3] These developments would play an essential role in literary and textual analysis, highlighting the potential of computational power for purposes beyond numerical analysis.

Each step in the punch card process required knowledgeable and trained punch card operators, often women. Then, Busa and Tasman iterated through this procedure many times before finalizing the process that produced the Index Thomisticus.

## Footnotes

[^1]: Rockwell, Geoffrey, and Stéfan Sinclair. 2020. “Tremendous Mechanical Labor: Father Busa’s Algorithm.” Digital Humanities Quarterly 14 (3). [Link](https://dhq.digitalhumanities.org/vol/14/3/000456/000456.html).

[^2]: Jones, Steven E. 2016. Roberto Busa, S.J., and the Emergence of Humanities Computing: The Priest and the Punched Cards. Routledge.

[^3]: Rockwell, Geoffrey, and Stéfan Sinclair. "Tremendous Mechanical Labor: Father Busa's Algorithm."