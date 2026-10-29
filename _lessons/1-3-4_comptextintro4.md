---
layout: sublesson
structurehead: comptext
lessontitle:
title: "Installing R & Basic Functions"
group: intro
headabstract: "This lesson refreshes some of the discussions from the previous lesson concerning the identity of the digital humanities."
abstract: "This lesson will teach learners about different digital methods and how they fit into humanistic research."
lessonnumber: 4
lessonprint: 4
permalink: "/lessons/intro/comptextinto/4"
previouslesson: "/lessons/intro/comptextinto/3"
nextlesson: "/lessons/intro/comptextinto/5"
authors: cagostini
---

Text analysis examines large amounts of textual information. R is a programming language designed primarily for statistical computing and data analysis.

Text analysis, also known as text mining, refers to the computational examination of large volumes of documents, focusing on language, context, and patterns. It is a methodological approach that is applicable to various fields, including the humanities, sociology, communications, and computer science. Common text analysis case studies involve books, articles, news, and tweets. Text mining consists of these steps:

- Creating a dataset
- Exploring text analysis strategies
- Interpreting findings.

## Download
R is a programming language designed primarily for statistical computing and data analysis. It offers a wide array of statistical techniques, including linear and nonlinear modeling, time-series analysis, classification, and clustering. Additionally, R supports graphical representations of data, making it a popular choice for making plots and charts.

Highly extensible, R allows users to create packages that add new functionalities. While it is widely utilized by statisticians and data analysts, it has been adapted to answer research questions in the humanities and digital humanities. 

[https://posit.co/products/open-source/rstudio](https://posit.co/products/open-source/rstudio/#Desktop)

RStudio is an integrated development environment (IDE) for R, designed to make it easier to write and run R code. It provides a user-friendly interface that includes features such as syntax highlighting, code completion, and a built-in console. RStudio also offers tools for data visualization, package management, and project organization, making it easier to manage R scripts and files. Additionally, it supports RMarkdown for creating dynamic reports that combine code, output, and text. Overall, RStudio enhances the R programming experience by providing a comprehensive environment for coding, analysis, and reporting.

Another option is to access R and RStudio through university-licensed software from any device.

If you want a fast, easy way to try R, you can use the [RStudio Cloud](https://rstudio.cloud/). It is a cloud-based version of RStudio that allows users to write and run R code in a web browser without needing to install software on their local machines. 

This web browser version of RStudio looks and functions just like the desktop version, and it will save data between sessions as well. 

All it takes is a Google or GitHub account to log on.

## Setup

First, [download R](https://cran.rstudio.com/) for your operating system. R is the programming language. 

Second, it is recommended to [download RStudio](https://www.rstudio.com/products/RStudio/). RStudio is an integrated development environment (IDE) that makes scripting in R much easier. 

Both R and RStudio are free and open-source software.
[Caption: This is what the RStudio interface looks like when you open it.]: #

When you launch RStudio, you’ll notice the default panes:

- Console (left, with the > prompt)
- Environment/History/Connections/Tutorials (tabbed, upper right)
- Files/Plots/Packages/Help/Viewer/Presentation (tabbed, lower right).

> Programming is helpful in the humanities because you understand more deeply what computers do to your data. By understanding the workings of an algorithm, you can better justify your claims as well as understand the ways algorithms may distort the data.

The work of data analysis becomes transparent. Since we’re writing code, we can trace the steps we made to make something.

We start to correct for the problem of tools shaping research questions. In other words, we build the tool to fit our questions.

## Install R packages

To install R packages, open RStudio, then type and run these lines in the console:
    install.packages("tidyverse")
    install.packages("tidytext")
    install.packages("tokenizers")
    install.packages("quanteda")
    install.packages("quanteda.textmodels")
    install.packages("quanteda.textstats")
    install.packages("quanteda.textplots")
    install.packages("readtext")
    install.packages("devtools")
    install.packages("quanteda.corpora")
    install.packages("newsmap")
    install.packages("seededlda")

> tidyverse provides convenient tools for reading in and working with data sets.

> tokenizers contains the functions that allow us to split text data into words and sentences. 

Depending on your system setup, these may open a dialog box asking you to choose a “mirror” to download from. Select one near your current location. Then, follow and confirm download and installation as you get the automatic prompt to do so.

Now, ask R to load these packages through the `library` command. The `library` commands must be run every time you restart R.

    library(tidyverse)
    library(tokenizers)

### Running R
    library(tidyverse)
    library(tokenizers)

[5]: #
[Caption: Entering a numerical value in R.]: #

Let's enter some numerical values in R:

    a <- 10
    b <- 20
    a <- b
    print(a)

[Caption: Mathematical values in R.]: #

[More examples with mathematical operations.]: #
Let's try doing math in R:

    sum(c(10,20,30))

[Caption: Summing numbers.]: #

[One Text]: #
[One Text]: # 

To display ( or print) a text, use the R-command cat() or print(). The text is considered by R as a script, so we need to have the text in quotes.

    cat("Hello world")
    print("Hello world")
    
Let's try defining a message and then using the print command to display it:
    msg <- "Have a good day!"
    print(msg)
    print("msg")
    
[Caption: After writing a message, you can render it by printing it.]: #

What differences do you notice between these two examples?