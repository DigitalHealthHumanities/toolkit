---
layout: sublesson
structurehead: comptext
lessontitle:
title: "Keyword-in-Context with AntConc"
group: intro
headabstract: "This lesson refreshes some of the discussions from the previous lesson concerning the identity of the digital humanities."
abstract: "This lesson will teach learners about different digital methods and how they fit into humanistic research."
lessonnumber: 3
lessonprint: 3
permalink: "/lessons/intro/comptextinto/3"
previouslesson: "/lessons/intro/comptextinto/2"
nextlesson: "/lessons/intro/comptextinto/4"
authors: cagostini
---

AntConc is a corpus analysis toolkit to examine words, texts, and corpora. It is a free corpus analysis tool used for studying text collections. For linguistic research and text analysis, it helps users gain insights into language use and structure. AntConc analyzes and visualizes text data through various functions, including word frequency counts, keyword extraction, concordance, and collocation analysis.

## Download

[Antconc](https://www.laurenceanthony.net/software/antconc/) from the [AntLab Website](https://www.laurenceanthony.net/).

**Unzip the download, if necessary. Next, launch the application.**
> [Updated releases](https://www.laurenceanthony.net/software/antconc/releases/AntConc324/) are published on a regular basis by AntConc’s creator, [Laurence Anthony](http://www.laurenceanthony.net/). 
> [Laurence Anthony’s guide to help users understand how to use AntConc.](https://prod-files-secure.s3.us-west-2.amazonaws.com/7b6b9cc5-d502-45c7-bc5d-561183134672/931a28b4-9fa4-4fda-9236-cd21771a0289/Anthony_Tutorial.pdf)

## Datasets
We can add files in the format of plain text (.txt), Word (.docx), and PDF (.pdf) files. 
- No More Silence, https://ucsf.app.box.com/s/ifdndlmnje0xme8jdg3i697s51zznect
- Industry Documents Library, https://ucsf.app.box.com/v/IDL-DataSets/folder/78644252849

## Corpus Analysis
{% include term.html term="Corpus" %} analysis is a form of text analysis which allows you to make comparisons between textual objects at a large scale. {% include term.html term="Distant reading" %} enables us to notice things that we might overlook when reading. If you have a collection of documents, you might want to find frequently recurring phrases in your corpus; statistically likely/unlikely phrases for a particular author or genre of text; grammatical structures; also, examples of a particular term or idea across many documents, and much more. Corpus analysis is valuable for testing hypotheses about texts and for cross-checking results from other digital methods.

{% include definition.html term="Distant Reading" definition="Distant reading is a mode of reading that is antithetical to 'close reading'. Rather than looking at one text with extreme scrutiny, distant reading looks for patterns and trends across a large collection of texts, making arguments based on these 'distant' observations." %}

This tutorial provides an overview of methods rather than a rigid step-by-step formula, and following the exact order is not always necessary. Corpus linguistic methods are customizable, so remember we need to think about how each step helps answer specific research questions.

This lesson will focus on the desktop tool AntConc. A similar webtool, [Voyant Tools](http://voyant-tools.org/), offers similar options for exploring text analysis methods. 

## The AntConc User Interface

{% include imgwithcaption.html filepath="/assets/img/Comptextintro1" alt="The top bar interface in AntConc. The tabs read, in order, 'KWIC', 'Plot', 'File View', 'Cluster', 'N-Gram', 'Collocate', 'Word', 'Keyword', 'Wordcloud', and 'ChatAI'." caption="Each of these tabs has its own function that can be used to do different forms of computational textual analysis." %} 

When AntConc opens, it shows an interface with the following tabs: 

- KWIC: {% include term.html term="Keyword in Context" %}, which is a concordance view.
- Plot: A visualization of your KWIC search along a bar, showing the position and frequency of words within the text.
- File View: Showing the broader context of a finding.
- Cluster: Words frequently found in the same context(s).
- {% include term.html term="N-gram" %}: Given that n is a number you decide, this feature shows commons terms.
- Collocate: Given a certain distance (number of words away from a specific word), words statistically likely to be found in the same context(s).
- Word: A list of all the words in the corpus.
- Keyword: Comparing most frequent, significant words across two corpora.
- Wordcloud: A visual representation of textual data in which the size of each word reflects its frequency or significance.
- ChatAI: This feature seems to be still in progress. There is a disclaimer, “Remember that OpenAI API calls will be charged to your account. Use the ChatAI tool with caution.”

{% include definition.html term="Distant Reading" definition="Keyword in context analysis provides a list of a specific word or phrase in context (up to five words in each direction is common). This approach is best for pattern identification and close reading." %}

{% include definition.html term="N-Gram" definition="N-grams observe clusters of terms which appear together in each dataset. This is very good for identifying common phrases in a particular genre, but also stylistic features which are unique to a specific author." %}

Start with File, then Open File as Quick Corpus or Open Corpus Manager. 

Add more than one file or a folder. Click Create so you can have a corpus loaded. Click Create. You will have a confirmation message, “Your corpus has been created.” 

This is your target corpus. You can always check what has been uploaded (and is being analysed) on the left,  in the window to see all corpus files–that would be your target corpus. 

Important: For all search tabs, except the Word tab (marked with an asterisk in this list), you need to type a word or more, then click Start.

## Search operators for **Keyword-in-Context (KWIC)**

{% include definition.html term="Keyword-in-Context" definition="Keyword-in-Context (KWIC) Analysis provides a list of a specific word or phrase in context (up to five words in each direction is common). This approach is best for pattern identification and close reading." %}

The * operator (for zero or more characters) can help find variations of the same word. For example, the singular and plural forms of nouns, or words with similar spellings but different meanings, but also irregular verbs in various tenses.

polic* would track police, policy, policies, etc.

s*t retrieves sit, sat

sit* finds sit, sits, sitting, etc.

The ? operator for d??r finds dear, deer, door, etc.

The | Operator (“or”)

The | Operator (“or”) can search alternative words, for example yes|no.

##Saving Outputs

While running AntConc, you can generate output files for reference. It is good practice to use descriptive filenames (for example, “med_hum_20241106.text”).
