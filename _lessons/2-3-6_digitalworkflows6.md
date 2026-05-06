---
layout: sublesson
structurehead: workflows
title: "Activity: Building Complex Workflows"
group: projectmanagement
abstract: "In this lesson, students will think through the step-by-step process of incorporating archival materials in a digital humanities project, looking at how different programs are used to transform data into useable forms." 
lessonnumber: 6
lessonprint: 6
permalink: /lessons/projectmanagement/digitalworkflows/6
nest: nonest
previouslesson: /lessons/projectmanagement/digitalworkflows/5
nextlesson: /lessons/projectmanagement/digitalworkflows/7
split: none
authors: spurcell
---

How would we transform archival materials, like the ones we used in the last lesson, into useful data? An important concept for digital workflows is an understanding that the materials we work with (like a physical book) require work to make them legible to our software. A computer does not have eyes to read a paragraph nor does it have hands to open a book or turn the pages. To make it readable by our computers we need to scan it, format the scanned image, and extract OCR. 

For this next activity, we will look at the steps a scholar would have to make in order to add archival objects into a digital humanities network graphing project. This process will incorporate the following steps: 1) The processing of digital archival files using an optical character reader (OCR) program, Abbyy Finereader, 2) The management of these files on a platform with .pdf reading capabilities, Obsidian, 3) the data entry process using a spreadsheet program, Microsoft Excel, and 4) the use of a computational textual analysis tool, AntConc, to check our work. As we are getting more specific, we will use specific programs instead of general program types, because we can be more concrete about a technology’s unique {% include term.html term="affordance" %}s.  

{% include definition.html term="Affordances" definition="The term ‘affordance’ refers to the material and technological limitations of a specific tool, platform, or method. For example, one of the affordances of a simple technology like a ballpoint pen is its ability to write." %} 

We’re adding multiple programs into our workflow at the same time, so we should define their uses concrete terms. More than describing their uses, we are also going to pay attention to the forms of labor required to make these tools work.  

This latter attention to labor is important: we may have a powerful, useful tool that requires extra person hours to get our data into a form that the tool can process, or we may be trying to kluge material into a shape to make it work. For example, Microsoft Word has a variety of uses and affordances, including ways to add images to a document; however, if you have ever tried to get an image into the right place in a document, you will know how finicky and difficult it is to get the program to work as you want it to.  

Being honest about the time it takes to get a program to work is an important step in this process. It is also an important one as we move, after this exercise, to thinking about {% include term.html term="prototyping" %} your own workflow. 

{% include definition.html term="Prototyping" definition="Prototyping refers to the development and testing of project methods and tools using a small sample size. The prototyping phase helps scholars work through technical snags early on, while also creating evidence for publications and grant proposals." %} 

To start, we should define our tools: 

**Abbyy Finereader:** This is an optical character recognition (OCR) tool that was commonly used prior to the development of machine learning and generative AI tools. It is a single program, and it does not use a cloud service, making the workflow simpler. For this example Abbyy Finereader is being used to generate OCR files for computational textual analysis later in the process. 

**Obsidian:** Obsidian is a file management program that has a lot of flexibility, with unique plugins and addons, and an interface that reads .pdfs and allows for detailed notes. This is going to be used by coders to access and read the files. 

**Microsoft Excel:** Microsoft Excel is a tabular data platform that can used to create auto-fill formulas to take data and automatically format it for Gephi. 

**AntConc:** AntConc is a computational textual analysis platform that can do simple, non-machine learning, analyses of textual corpora. 

What you may notice is that we have a divergent workflow: where we have data entry by hand working through Obsidian and Microsoft Excel, and then an OCR workflow for doing computational textual analysis. We are including both because we want to show how we can connect programs together, but we also want you to consider the moments when humans interact with the material. Human labor is often the most important and time-consuming part of a project, and we do not want to omit this in our workflow. 

Let’s start with our Obsidian workflow first. 

On a scratch piece of paper or on your computer, create a workflow diagram where .pdf files are added to Obsidian and coders translate that information into Microsoft Excel. Once you do, link that workflow to the Gephi and word processing workflow we sketched in the previous section. 

The Obsidian to Excel workflow might look like this: 

{% include spoiler.html title="Check Your Work" image="/assets/img/Workflow_Revised5.JPG" alt="A workflow. 'Original .pdf File' points to 'Obsidian' points to 'Individual Coders' points to 'Input into Microsoft Excel'." answer="This workflow shows the steps required to transfer the .pdf files into Obsidian and then code them into a Microsoft Excel file." %} 

Now try linking that into the Gephi workflow from [our previous lesson](digitalhealthumanities.github.io/toolkit/lessons/projectmanagement/digitalworkflows/4). Here is our example: 

We can add that to our Gephi workflow: 

{% include spoiler.html title="Check Your Work" image="/assets/img/Workflow_Revised6.JPG" alt="A larger workflow built on the workflow from the previous lessons. 'Citation Manager' and 'Image Editor' have arrows pointing to 'Word Processor'. Both 'Word Processor' and 'Image Editor' have arrows pointing to 'Final Submission'. The Gephi workflow connects to the Excel and Obsidian elements. 'Original .pdf File' connects to 'Obsidian' connects to 'Individual Coders' connects to 'Input into Microsoft Excel'. The 'Input to Microsoft Excel' category splits, pointing to the Gephi elements'—'Comma Separated Value File' connecting to 'Gephi' connecting to 'Image File' connecting to 'Image Editor.' 'Input to Microsoft Excel' also connects to 'Exported Figures' box. 'Exported Figures' connects to 'Word Processor'." answer="This workflow links directly to the 'Spreadsheet Software' element from the previous lessons’ workflow." %} 

What about the OCR documents? How might that fit in? Maybe we are using the OCR files to check our work? Maybe we are using them to analyze with a program like AntConc? 

Try sketching out an OCR workflow that requires some programmatic data cleaning in python.  

Once you have that, add into that workflow the use of a AntConc to do computational textual analysis. We have coders who are working on data entry for this hypothetical project, but computational textual analysis can be a helpful method to check our work at scale, looking to see if the trends we are observing occur throughout our sampled materials. 

What does this workflow look like? Here is our example: 

{% include spoiler.html title="Check Your Work" image="/assets/img/Workflow_Revised7.JPG" alt="A workflow 'Original .pdf File' points to 'Abbyy Finereader' points to 'Export .ocr File' points to  'Clean File in Python' points to 'Analyze Materials in AntConc'." answer="This workflow shows how the .pdf file is processed through multiple programs. We could add an additional human role for the AntConc element, which requires some examination and extrapolation. We will add that in the next lesson." %} 

Now add it to your main workflow. It should look something like this: 

{% include spoiler.html title="Check Your Work" image="/assets/img/Workflow_Revised8.JPG" alt="A larger workflow from above. 'Citation Manager' and 'Image Editor' have arrows pointing to 'Word Processor'. Both 'Word Processor' and 'Image Editor' have arrows pointing to 'Final Submission'. The Gephi workflow connects to the Excel and Obsidian elements. 'Original .pdf File' connects to 'Obsidian' connects to 'Individual Coders' connects to 'Input into Microsoft Excel'. The 'Input to Microsoft Excel' category splits, pointing to the Gephi elements'—'Comma Separated Value File' connecting to 'Gephi' connecting to 'Image File' connecting to 'Image Editor.' 'Input to Microsoft Excel' also connects to 'Exported Figures' box. 'Exported Figures' connects to 'Word Processor'. The 'Original .pdf File' box has a new, linear workflow, pointing to 'Abbyy Finereader' pointing to 'Export .ocr File' pointing to 'Analyze Materials in AntConc' pointing to 'Analyze and Interpret AntConc Data' which ends at the 'Word Processor' box." answer="The .pdf file is used by two very different workflows to create distinct data for the final printed project." %}  

Important in this hypothetical workflow is that sometimes you may need to apply different methods and digital tools to different kinds of material. The way you are processing and analyzing that material may be different, may require different moments where humans are doing labor, and may include different forms of processing and file transformation.  

The workflow we developed over the past four sections has taken a lot of liberties with how we might define a workflow. We chose the example above because it allowed us to consider unique tools, human intervention, as well as branching and converging moments. It is very likely a workflow for your project would look nothing like the one we sketched out. 

What we would like for you to take away are two understandings: 

You will most likely need to work through multiple tools and file formats in the process of your research. This is often more complicated than we recognize, because we are used to doing this work in some form already. 

The specific tools you use have some technical {% include term.html term="affordance" %}s that require specific transformations. You need humans to translate .pdf files into .csv data which can be ingested into Gephi. You need an image editor to take Gephi images and format them for publication. 

The next sections will take these lessons and apply them to your unique research. You will learn about the purpose of prototypes and protocols in digital humanities research, and you will be encouraged to sketch out these elements in the process. 