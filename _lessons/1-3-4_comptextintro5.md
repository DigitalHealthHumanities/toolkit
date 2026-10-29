---
layout: sublesson
structurehead: comptext
lessontitle:
title: "Word Tokenization"
group: intro
headabstract: "This lesson refreshes some of the discussions from the previous lesson concerning the identity of the digital humanities."
abstract: "This lesson will teach learners about different digital methods and how they fit into humanistic research."
lessonnumber: 5
lessonprint: 5
permalink: "/lessons/intro/comptextinto/5"
previouslesson: "/lessons/intro/comptextinto/4"
nextlesson: "/lessons/intro/comptextinto/6"
authors: cagostini
---

Let’s start text analysis with a single paragraph of text. The example here is the opening paragraph from [Henry James, *The Wings of the Dove*](https://www.gutenberg.org/files/29452/29452-h/29452-h.htm) (1902).

To read this into R, copy and paste the following into the R console.
    text <- paste("She waited, Kate Croy, for her father to come in, but he kept her unconscionably, and there were moments at which she showed herself, in the glass over the mantel, a face positively pale with the irritation that had brought her to the point of going away without sight of him. It was at this point, however, that she remained; changing her place, moving from the shabby sofa to the armchair upholstered in a glazed cloth that gave at once—she had tried it—the sense of the slippery and of the sticky. She had looked at the sallow prints on the walls and at the lonely magazine, a year old, that combined, with a small lamp in coloured glass and a knitted white centre-piece wanting in freshness, to enhance the effect of the purplish cloth on the principal table; she had above all, from time to time, taken a brief stand on the small balcony to which the pair of long windows gave access. The vulgar little street, in this view, offered scant relief from the vulgar little room; its main office was to suggest to her that the narrow black house-fronts, adjusted to a standard that would have been low even for backs, constituted quite the publicity implied by such privacies. One felt them in the room exactly as one felt the room—the hundred like it or worse—in the street. Each time she turned in again, each time, in her impatience, she gave him up, it was to sound to a deeper depth, while she tasted the faint, flat emanation of things, the failure of fortune and of honour. If she continued to wait it was really, in a manner, that she might not add the shame of fear, of individual, personal collapse, to all the other shames. To feel the street, to feel the room, to feel the table-cloth and the centre-piece and the lamp, gave her a small, salutary sense, at least, of neither shirking nor lying."
    words

[Caption: Entering a paragraph of text into R.]: #

Hit enter. You will see the paragraph of text “printed.” 

Next, we get the `tokenize_words` function from the tokenizers package.

    words <- tokenize_words(text)
    words

[Caption: Tokenizing words.]: #

The first line assigns the tokenize_words function to the term 'words'. The words command in the second line then outputs a word list, removing all punctuation, finding individual words, and making everything lowercase. 

To count words, we need to use the length function and associate it with the number `[[1]]` because a list object is one entry per document. Try this command with the other two:

    length(words[[1]])

[Caption: Requesting to count words.]: #

We can ask how many times is each word used in the text, and display them as a table:

    tab <- table(words[[1]])
    tab <- data_frame(word = names(tab), count = as.numeric(tab))
    tab

[Caption: Counting word occurrences.]: #

We can arrange the words by which ones are most frequent using the desc(count) command:

    arrange(tab, desc(count))

[Caption: Ordering frequent words.]: #

The most common words tend to be pronouns, articles, and conjunctions. 

A popular technique is to maintain a list of highly used words and removing these prior to any formal analysis. The words on such a list are called “stopwords”, and usually include words such as pronouns, conjugations of the most common verbs, and conjunctions. 

Stopwords (https://github.com/koheiw/stopwords) in several languages are available on GitHub.

## Visualizing Sentences

We have seen individual instances of words. We can also see individual sentences.
    sentences <- tokenize_sentences(text)
    sentences

[Caption: Viewing each sentence.]: #

We can also view each sentence and count its words.
    sentence_words <- tokenize_words(sentences[[1]])
    sentence_words
    
[Caption: Counting words in sentences.]: #

Checking the size of the output directly, we can see that there are “documents” in the object sentence_words:

    length(sentence_words)

## Analyzing a Corpus

Finally we can point to all of the files in

input_loc <- "/Users/yourname/Desktop/corpus_text"
Caption: Retrieving a corpus in R.