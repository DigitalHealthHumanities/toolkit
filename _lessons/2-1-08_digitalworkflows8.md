---
layout: sublesson
structurehead: workflows
lessontitle: "Digital Workflows"
title: "Activity: Prototyping"
group: projectmanagement
abstract: "This activity walks through the various questions and problems that arise when planning a project, showing how prototyping can solve some of these concerns at an early phase in the research." 
lessonnumber: 8
lessonprint: 8
permalink: /lessons/projectmanagement/digitalworkflows/8
nest: nonest
previouslesson: /lessons/projectmanagement/digitalworkflows/7
nextlesson: /lessons/projectmanagement/digitalworkflows/9
split: none
authors: spurcell
---

How about we do an activity, brainstorming how you might {% include term.html term="prototype" %} a research project?  

Take out a scratch piece of paper and list ONE media type you intend to plan to work with on your digital project. (We also have a worksheet with the questions in our GitHub Repo.) We are using "media type" to think of the material and technological limitations of working with a humanistic {% include term.html term="text" %}. Rather than thinking about a text as a single thing, a book like *Wuthering Heights*, we instead can think of it as its broader media type, a "printed novel". The reason for this is that the media type has its own set of {% include term.html term="affordances" %} —a printed novel has pages with text and it is bound in a very specific manner, and it is different than, say, a .txt file with all of the text from the novel. 

- With this medium type written out, respond to the following questions: 
- What is my research question? 
- How am I trying to answer this research question? (What is my method?) 
- What kind of data do I need to answer my research question? 
- How is the data I need found in the medium type? 
- How do I plan to extract this data? 
- How do I plan to process this data? And/or what tool do I plan to use to analyze the data? 

These questions broadly fit into a schema:  

1. What am I working with?  
2. What am I trying to do?  
3. What tools do I need to do this?  

The goal of these questions is to start thinking about how your sources link into a workflow. 

- Once you have these questions answered, reflect on the last three. Ask yourself:  
- What tools might you need to make your materials digitally accessible? What tools might you need to extract data?  
- What tools might you need to analyze that data? 

This process might be simple. If you are working with cleaned, digital scans of Shakespeare’s plays, you might answer that the materials are already accessible and organized. The only step is to figure out the best platform to do textual analysis. This process might also be more complicated, involving scanning, marking up visual files, and then using a tool to process metadata. 

{% include spoiler.html title="Example Responses" answer="<strong>What is my research question?</strong> How do each of the Bronte sister’s word choice differ in their novels?<br><strong>How am I trying to answer this research question? (What is my method?)</strong> I will use textual analysis in AntConc and sentiment analysis to answer these questions.<br><strong>What kind of data do I need to answer my research question?</strong> I need clean .txt files.<br><strong>How is the data I need found in the medium type? </strong>The material books have text that can be read with OCR.<br><strong>How do I plan to extract this data?</strong> I will scan the books with a book scanner, and use an OCR tool to turn those scans into .txt files.<br><strong>How do I plan to process this data? And/or what tool do I plan to use to analyze the data?</strong> I will clean the .txt files with a Python script. I will then analyze them with AntConc and a sentiment analysis program." %} 

From these questions draft out a prototyping workflow, linking your medium type to potential extraction technologies and methods as well as data processing tools and methods.  

On a scratch piece of paper, try to list out the **different {% include term.html term="transformative processes" %}  required to make your original object usable for analysis**. Using the example above, how might you take a bound book and make its text readable by a computational textual analysis tool? You would need to 1) scan the pages, 2) translate those pages to a text-only format, 3) clean the text-only file, and 4) input it into computational textual analysis platform. 

{% include definition.html term="Transformative Processes" definition="This concept refers to the moments when scholars need to change the medium, platform, or file type of their analytical materials. This can be a transformation from analog to digital (scanning a physical book) to make it legible for digital tools or a transformation of one file type to another (changing an image from .png to .jpg) to make it easier to display online." %} 

Each of these transformations requires some amount of labor and care, and there are multiple approaches and tools you might want to do. 

From this list of transformations, brainstorm 2-4 potential tools or methods you might use for each transformation. You want to make sure your approach is applicable for all the tools you plan to use. You may have a preferred method of extracting data, but if it does not extract information that is unusable with other tools, you may have to adjust to a different approach.  

<div class="backsplash"><strong>A note here:</strong> if you are a novice digital humanist, you may not know what tools you need! That is okay. You can leave them blank and do some research and/or consult with colleagues, and then fill in this information later.</div> 
 

{% include spoiler.html title="Here is our example, using the transformations listed above." image="/assets/img/Workflow_Revised12.JPG" alt="A brainstormed list, in the shape of a grid, which will be used to draw a workflow in the next step. At the top is a box labeled ‘Original Books’. The next row has a definitional box ‘Scan Physical Pages’ with three options: ‘Scan with Book Scanner’, ‘ Scan with .tiff Quality Scanner’, ‘Access Digital OCR Version’. The second row, ‘Translate Scanned Images to Text Form’, also has three options: ‘Type Text by Hand’, ‘OCR with Abbyy Finereader’, ‘OCR with AI Tool’. The third row, ‘Clean Text Files’, has two options: ‘Clean Files with Python Script’, and ‘Clean Files Manually’. The final row, ‘Analyze Text Files’ has three options: ‘Analyze with AntConc’, ‘Anayze with Voyant’ and ‘Analyze with Sentiment Analysis Tool’." answer="These are not our only options for each of the processes and transformations we want to test. You may find yourself not liking any of the options available to you, making you have to brainstorm new options." %} 

Once you have a sense of the different tools and methods you want to test, you can start testing the different methods. There is no *right* way to test these tools, as your own research questions, scholarly positionality, taste, and comfort may guide you to one tool or the other. 

An important phase in this process is to test how tools work together. You may need to additional steps to translate raw textual data into something more structured, or you may need to include a program that changes one file type to another. The only way you can know this ahead of time is to try it out.  

Here is an example of how you might cross out tools in the process: 

{% include spoiler.html title="Here is our example, using the transformations listed above." image="/assets/img/Workflow_Revised13.JPG" alt="A brainstormed list, in the shape of a grid, which will be used to draw a workflow in the next step. At the top is a box labeled ‘Original Books’. Three arrows point to three boxes in the‘Scan Physical Pages’ row: The option ‘Scan with Book Scanner’ is not crossed out. ‘ Scan with .tiff Quality Scanner’ is crossed out with a note: ‘No need for high quality scan’; and ‘Access Digital OCR Version’ is also crossed out with a note: ‘No OCR Version Available’. Three arrows point from the ‘Scan with Book Scanner’ block to the three entries in the ‘Translate Scanned Images to Text Form’ row. ‘Type Text by Hand’ is crossed out with a note: ‘too time consuming’; and ‘OCR with AI Tool’ is also crossed out with a note: ‘Personal Issues with Technology’. The final box, ‘OCR with Abbyy Finereader’ is not crossed out, and it has two arrows pointing to the boxes in the ‘Clean Text Files’ row. ‘Clean Files Manually’ is crossed out with a note: ‘Too Time Consuming’; and the other box, ‘Clean Files with Python Script’ is not marked. This latter box has three arrows pointing to the boxes in the ‘Analyze Text Files Row’. ‘Analyze with Voyan’ is crossed out with a note: ‘Poor Interface for Analysis’; and ‘Analyze with Sentiment Analysis Script’ is also crossed out with a note: ‘Not a Sentiment Analysis Project’. The final box in the row, ‘Analyze with AntConc’ is unmarked." answer="You may notice that some decisions can be made early on without directly testing. For example, if you do not want to use AI tools, you can cross out those tools altogether without using them." %} 

The goal of the prototype phase is to test out many different approaches together with a small, representative sample of material from your larger research project. You are taking time now to diligently test each object and tool, because it can save you hours, or weeks, or months of research time when you realize, halfway through a project, that the tool you intended to use would not answer your research question. 
