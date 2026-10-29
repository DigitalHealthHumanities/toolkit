---
layout: sublesson
structurehead: comptext
lessontitle:
title: "Stylometry in R"
group: intro
headabstract: "This lesson refreshes some of the discussions from the previous lesson concerning the identity of the digital humanities."
abstract: "This lesson will teach learners about different digital methods and how they fit into humanistic research."
lessonnumber: 6
lessonprint: 6
permalink: "/lessons/intro/comptextinto/6"
previouslesson: "/lessons/intro/comptextinto/5"
nextlesson: n/a
authors: cagostini
---

Stylometry, the study of linguistic style, makes extensive use of computational methods to describe the style of an author’s text. The corpus can be split into sentences using the tokenize_sentences function.

Let's start by looking for sentence length:

    sentences <- tokenize_sentences(text)
    sentences

And then we can tokenize the words in sentences:

    sentence_words <- sapply(sentences, tokenize_words)

And list the the words, and sentence length:

    sentence_length <- list()
    for (i in 1:nrow(metadata)) {
      sentence_length[[i]] <- sapply(sentence_words[[i]], length)
    }

And find the median length:

    sentence_length_median <- sapply(sentence_length, median)

[Caption: Sentences and style by year.]: #
[qplot(metadata$year, sentence_length_median)]: #

## More Resources

Posit (formerly RStudio) has a comprehensive guide, https://support.posit.co/hc/en-us