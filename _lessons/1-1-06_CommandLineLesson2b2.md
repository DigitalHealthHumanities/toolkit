---
layout: sublesson
structurehead: CommandLine
group: databasics
nest: windows
title: "Navigating Your Computer's Folders"
abstract: "In this section you will learn about the history of the command line in computers, and why it matters for doing digital research."
lessonnumber: 6
lessonprint: 2b.2
permalink: /lessons/databasics/commandline/2b2
previouslesson: /lessons/databasics/commandline/2b1
nextlesson: /lessons/databasics/commandline/3b1
split: none
---

**To do the next step, please download and unzip the [working files folder](https://ucsf.box.com/s/xlyqx9t24e2su78ww2jh52f6xc2xp4va). (For the examples, I have unzipped this folder in my downloads folder.)**

**This introduction assumes that the files you have downloaded are in the downloads folder. If they aren’t be sure to put them there!**

When we open the Command Prompt, we’ll start in the same place: your user folder. This is what a user folder might look like. (You can access it by clicking on your OSDisk, which is the C drive for this computer, clicking on the folder titled ‘Users’ and clicking on the folder with your username. For this example the user is ‘spurcell’.) 

![](/assets/CLWin2.jpg)

If you are lost, you can always use the GUI folder hierarchy to help you search, because they are looking at the same thing. 

Let’s write our first command. Type the following into the Command Prompt:

    dir

This command—‘dir’—is short for ‘directory’. It will output all of the potential directories and files that you can access from your current place in the computer. 

<p style:"margin-left: 80px">**Important Term: Directory –** A directory is a collection of files and directories which the command line accesses. Often, we call them folders, largely because of their iconography in contemporary GUIs</p>

The ‘dir’ command can help us if we are lost, or if we do not know what directories of files we have access to at a given moment.

Let’s look at that output from that command. This is how it looks like on my computer: 

![](assets/CLWin3.jpg)

I can see the folder ‘downloads’ in the directory, which means that I can move to that folder in the Command Prompt. To do this, we will need to use a different command, ‘cd’ or change directory. 

So type in:

    cd downloads

The Command Prompt processes this function by first reading the command—‘cd’—and then reading the additional information designating specifics about how to execute that command. Typing in ‘cd downloads’ is telling the command prompt to change directories to a directory named ‘downloads’. 

Once we’re in downloads we will need to access the directory that holds the files we’re going to use. This directory, which needs to be unzipped, is titled ‘commandline_examples’. To access it type: 

    cd commandline examples

You just ran into a problem, right? It is important to know that when navigating folders, you may run into issues with files with spaces—’ ‘—in them. The reason for this error is that the Command Prompt reads each space as a new kind of information (we’ll see how this operates later in this lesson!). To fix this, we have to escape out—or create an argument in the Command Prompt—that it recognizes as a single unit, using quotation marks. 

Try this instead:

    cd "commandline examples"

There are a few more things to know before we move forward. First, we can move backwards in the directory hierarchy using the following command 

    cd ..

This command tells us to go to the directory that contains our current working directory. Let’s do the ‘cd ..’ a second time to return to the user directory. 

We can also navigate multiple steps through directories by compounding them using the backslash. 

From the user directory (the directory which we started this exercise) type: 

    cd "downloads\commandline examples"

The last thing we need to do, before actually using the Command Prompt to do some text analysis is that we’ll need a directory into which our analyses will be output. To do this type 

    mkdir outputs 

This command makes a directory—‘mkdir’ is short for make directory—and titles the directory whatever we write after the space. 

We can navigate to that directory by typing ‘cd outputs’ or navigate out of it by typing 'cd ..'.	