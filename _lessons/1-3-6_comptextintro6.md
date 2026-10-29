---
layout: sublesson
structurehead: comptext
lessontitle:
title: "Working with a Corpus: Finding Files"
group: intro
headabstract: "This lesson refreshes some of the discussions from the previous lesson concerning the identity of the digital humanities."
abstract: "This lesson will teach learners about different digital methods and how they fit into humanistic research."
lessonnumber: 6
lessonprint: 6
permalink: "/lessons/intro/comptextinto/6"
previouslesson: "/lessons/intro/comptextinto/5"
nextlesson: "/lessons/intro/comptextinto/7"
authors: cagostini
---

**For this lesson, we will use a collection of .txt files to analyze a corpus. Please download these [sample .txt files](https://ucsf.app.box.com/s/xlyqx9t24e2su78ww2jh52f6xc2xp4va).**

## Analyzing a Corpus
To read all your files into R together. Point to where your files are. (You will need to unzip the files and locate them in your computer's file system.)

    input_loc <- "/Users/yourname/Desktop/corpus_text"

## Finding Your Dataset
Now let’s make sure you’re working in an appropriate directory on your computer. Enter `getwd()` in the Console to see current working directory or, in RStudio, this is displayed in the bar at the top of Console. ([We have an introduction to the command line in this toolkit]({{ site.baseurl }}/lessons/databasics/commandline/1)!)

In RStudio, go to Session > Set Working Directory > Choose Directory > [folder you saved to your Desktop].

The current working directory is displayed by the RStudio IDE within the title region of the Console pane. You can also check your current working directory by running the command getwd() in the console.

There are a few ways to change the current working directory:

Use the setwd R function

Use the Tools | Change Working Dir... menu (Session | Set Working Directory on a mac). This will also change directory location of the Files pane.

From within the Files pane, use the More | Set As Working Directory menu. (Navigation within the Files pane alone will not change the working directory.)

Be careful to consider the side effects of changing your working directory:

Relative file references in your code (for datasets, source files, etc) will become invalid when you change working directories.

The location where .RData is saved at exit will be changed to the new directory.

If you want to type the specific location for your files, you can follow these directions.
    file.copy(from="C:/Users/[Your Name]/Documents/[Folder Name]/[File Name].txt",
          to="C:/Users/[Your Name]/Documents/[Another Folder Name]/[Same File Name].txt")