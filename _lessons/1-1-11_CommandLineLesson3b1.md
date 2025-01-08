---
layout: sublesson
structurehead: CommandLine
group: databasics
nest: mac
title: "The Find Command"
abstract: "In this section you will learn about the history of the command line in computers, and why it matters for doing digital research."
lessonnumber: 11
lessonprint: 3b.1
permalink: /lessons/databasics/commandline/3b1
previouslesson: /lessons/databasics/commandline/2b2
nextlesson: /lessons/databasics/commandline/3b2
split: none
---

**Required: You will need to download and unzip the [command prompt files](https://ucsf.box.com/s/xlyqx9t24e2su78ww2jh52f6xc2xp4va) for this lesson.**

The command line has the ability to process text files in important and unique ways. While some programs and approaches can do more granular analysis, the command line can introduce us to some simple ideas around computational text analysis. 

This also can teach us some of the basics of inputting commands into the command line, and understanding how it functions. 

To learn these tools, first navigate to the command prompt folder in your downloads. (If you are confused about how to navigate see section 2b.2.) 

Once you are there, let’s see what we’re working with. To look at what is in the directory type the following code

    dir 
	
![]({{ site.baseurl }}/assets/img/CLWin3.jpg)

The files in the directory are text files, demarcated with the .txt suffix for each file. Text files are just that: files that only contain textual information. There are other file types you may work with regularly like Adobe’s portable document format (.pdf), or Microsoft Word’s files (.docx), or compressed image files in the joint photographic experts group file type (.jepg or .jpg). All files have this suffix, and computer programs look at these suffixes to determine whether the file is readable. 

The [PLACEHOLDER] files in this folder are all text files for materials related to the history of tuberculosis around 1910 and 1920. They were originally taken from HathiTrust, but they have been formatted in such a manner as to have every page be its own unique line in the text. This is what the file BrownSampson_IntestinalTuberculosisIts_1926.txt looks like when opened using a text editor. 

![]({{ site.baseurl }}/assets/img/CLWin4.jpg)

We won’t have to change these files in any way, but it usually useful to get a sense of what is happening inside a document before you start using code on it. This document has been formatted in a particular way, but it is obviously not cleaned. There’s a lot of extra punctuation that the optical character recognition (OCR) tool did not read correctly. This is fine for this activity, but might run into problems later down the line. 

We can also learn about these tools using Voyant—a web-based text analysis tool. (See our text analysis introduction for more information about Voyant.) 

Based on this little information we have, we can use the command line to look for specific terms and count them. 

While you are in the command prompt directory type in: 

    find /c “tuberculosis” * 

You will get this output:  

![]({{ site.baseurl }}/assets/img/CLWin5.jpg)

What you have done is use the command “find” using a specific set of commands and characters that have defined what the computer will look for. 

The “find” command works in sequential order with a space between each command. The command works like this: 

    find [parameters marked with a ‘/’ slash] [the search string enclosed in quotation marks “”] [what files it will look at] 

<p style="margin-left: 40px"><b>Important Term - String:</b> A string is a line of characters which a computer can use for specific programmatic functions.</p>  

The parameter used in this command is ‘/c’ which counts each time the string appears in the text. And the asterisk ‘\*’ at the end of the command is a wild character—which means that the computer will look for all files in the directory. 

<p style="margin-left: 40px"><b>More information:</b><br> 
We could use the asterisk to search for a specific file type by typing “*.txt” at the end of this search. We could also use it to define specific files, so if I wanted to only read the transactionsofthefifteent15_1919.txt and transactionsofthesectiono_1923 I could write “trans*” at the end of my search command.<br></p>
We can think of a find command as having a kind of grammar and logic the command we used above, 

    find /c “tuberculosis” * 

Can be read as 

    In the current directory, find and count every instance of the term “tuberculosis” in every file. 

There are a few other parameters that are important to know, like the /i which searches for the string without considering capitalization. This can matter because sometimes terms may be capitalized or not capitalized across a document. 

![]({{ site.baseurl }}/assets/img/CLWin6.jpg)

Before we go to the next step, try searching for a few terms of these terms: 

- Google 
- E. L. Trudeau 
- tuberculin  

The first term ‘google’ shouldn’t show up, because these documents come from the early twentieth century. The other two terms E. L. Trudeau and tuberculin refer to specific historical actors and practices. What is important, at least for E. L. Trudeau is that he might show up in the files in a few different ways, because E. L. might be written out as his full name Edward Livingston Trudeau. 