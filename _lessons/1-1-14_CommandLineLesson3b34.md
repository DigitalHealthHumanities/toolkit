---
layout: sublesson
structurehead: CommandLine
group: databasics
nest: windows
title: "Making Files"
abstract: "In this section you will learn about the history of the command line in computers, and why it matters for doing digital research."
lessonnumber: 14
lessonprint: 3b.4
permalink: /lessons/databasics/commandline/3b4
previouslesson: /lessons/databasics/commandline/3b3
nextlesson: /lessons/databasics/commandline/4
---

In order to address this problem of having a long output in the terminal, we will have to take that output and export it into a new file. We do this because it allows us to have it in a form that we can read using a text reader, and also because it can save the outputs we find. 

But first, so it does not effect any other outputs that we’re exporting, we should create a new directory. We do this by using the ‘mkdir’—make directory—command: 

    mkdir outputs 

This command will make a directory with the same name as the next word or string. 

Type: 

    dir 

And you can see the directory you just made. 

To create a file with an command output you will need to use the ‘>’ at the end of the command you enter. 

Let’s make a new folder counting the number times ‘tuberculin’ is used: 

    find /c /i “tuberculin” *.txt > outputs\tuberculinfind.txt 

This command looks a bit different than the others, so let’s break it down. 

    find /c /i “tuberculin”  

This part of the code is the same as before. We’re counting “tuberculin” as it appears, without considering different capitalization. 

    *.txt 

This is different because we have a different object in our directory: the outputs folder. We don’t want the code to look at that, so the *.txt is basically saying: look at every file with a ‘.txt’ suffix and ignore any other files. 

    > outputs\tuberculinfind.txt 

This is the command that is telling the command prompt to export the command output into a new file. (Or if that file exists to overwrite the file.) The ‘>’ tells the command prompt to do this and then the entry that follows is a folder hierarchy and a file name. So ‘outputs\tuberculinfind.txt’ is telling the command prompt to look into a directory inside the current directory named ‘outputs’ and then make a file with the name ‘tuberculinfind.txt’. 

Now run that command: 

    find /c /i “tuberculin” *.txt > outputs\tuberculinfind.txt 

You should have in that outputs directory a new file named tuberculinfind.txt and it should look like this: 

![]({{ site.baseurl }}/assets/img/CLWin8.jpg)

Now try to do the same with the findstr command. 

    findstr /i “tuberculin” *.txt > outputs\tuberculinstring.txt 

Remember that we want to make a new file, so it’ll have to have a new name. What you have now is a collection of pages that describe tuberculin. 