---
layout: sublesson
structurehead: CommandLine
group: databasics
nest: windows
title: "The findstr Function"
abstract: "In this section you will learn about the history of the command line in computers, and why it matters for doing digital research."
lessonnumber: 13
lessonprint: 3b.3
permalink: /lessons/databasics/commandline/3b3
previouslesson: /lessons/databasics/commandline/3b2
nextlesson: /lessons/databasics/commandline/3b4
split: none
---

Where Mac computers have a single term that includes all the functionality we’re trying to achieve in this activity (called ‘grep’), for Windows, the ‘find’ function is accompanied by another function—‘findstr’. 

The ‘findstr’ function has a wider utility than the ‘find’ function, because it has a lot more and different parameters which it can use. What we are going to use it for is to find the unique pages for each instance of a given string. This will give us information as to the proximity of each term, so that we can produce different results from it. 

What we are going to do is search for each line for each page a specific term is used. The reason for this is that we can then use these extracted lines for a kind of simplified text analysis. It also lets us learn a few additional functions. 

The same grammar of using ‘findstr’ applies. So 

    findstr /i “tuberculin” * 

would read something like 

    Find every line in every document that includes the word “tuberculin” without considering capitalization. 

Try running that code. 

What you’ll realize when you run the command is that it outputs A LOT of text. In the next step we’ll learn how to create a new directory and how to output files in the command line. 