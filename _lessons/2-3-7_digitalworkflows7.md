---
layout: sublesson
structurehead: workflows
title: "Prototyping"
group: projectmanagement
abstract: "This lesson outlines the concepts behind prototyping in the digital humanities." 
lessonnumber: 7
lessonprint: 7
permalink: /lessons/projectmanagement/digitalworkflows/7
nest: nonest
previouslesson: /lessons/projectmanagement/digitalworkflows/6
nextlesson: /lessons/projectmanagement/digitalworkflows/8
split: none
authors: spurcell
---

{% include term.html term="Prototyping" %} in the digital humanities refers to the testing of workflows, tools, and approaches at a small scale, before using them with a larger collection of data. You might prototype a GIS project by selecting a few key addresses to test whether QGIS or ArcGIS are the best platform for your project; or you might run a few books through a topic modelling software to learn how it works. Prototyping is a process of intentionally testing every moving part within a digital humanities project to learn how each program, data source, and process works in conjunction with each other, to determine if different technologies may be better fits for the research project, and to develop protocols for the work. 

{% include definition.html term="Prototyping" definition="Prototyping refers to the development and testing of project methods and tools using a small sample size. The prototyping phase helps scholars work through technical snags early on, while also creating evidence for publications and grant proposals." %} 

A prototype helps answer questions like, "How can I apply my primary data to a specific method?" or "How do I create a table or figure for a finished journal article with this digital tool?" Prototyping is about filling in the gaps between what you expect to do in a research project, and the actual messy implementation of that method. 

{% include imgwithcaption.html filepath="/assets/img/Workflow_Revised9.JPG" alt="A graph showing a trajectory of thought. 'Your Data Source' is connected to the question, 'How do you need to process the data for your main method or tool?'. This question links to a box titled 'Your Main Method' which points to a new question, 'What do you need to do to translate that into your final product?' This question points to the final box, 'Your Main Deliverable." caption="An important thing to remember about designing a workflow is that your data, method, and final deliverable may not be the same medium. You have to think through the transformations that may happen." %} 

In the previous lesson, we looked at three archival items and considered them as potential resources for a network analysis project on the history of HIV/AIDS (figs. 2-4, also available on  GitHub). In that previous exercise, we asked you to think about a workflow with optical character recognition (OCR). The final workflow looked like this:  

{% include imgwithcaption.html filepath="/assets/img/Workflow_Revised8.JPG" alt="A larger workflow from above. 'Citation Manager' and 'Image Editor' have arrows pointing to 'Word Processor'. Both 'Word Processor' and 'Image Editor' have arrows pointing to 'Final Submission'. The Gephi workflow connects to the Excel and Obsidian elements. 'Original .pdf File' connects to 'Obsidian' connects to 'Individual Coders' connects to 'Input into Microsoft Excel'. The 'Input to Microsoft Excel' category splits, pointing to the Gephi elements'—'Comma Separated Value File' connecting to 'Gephi' connecting to 'Image File' connecting to 'Image Editor.' 'Input to Microsoft Excel' also connects to 'Exported Figures' box. 'Exported Figures' connects to 'Word Processor'. The 'Original .pdf File' box has a new, linear workflow, pointing to 'Abbyy Finereader' pointing to 'Export .ocr File' pointing to 'Analyze Materials in AntConc' pointing to 'Analyze and Interpret AntConc Data' which ends at the 'Word Processor' box." caption="The .pdf file is used by two very different workflows to create distinct data for the final printed project." %} 

When developing a prototype, we need to test every tool we plan to use on a small sample of representative materials that stand in for our larger collection. Where, in the previous section, we made assumptions about what the workflow might look like, a prototype tests to see if those assumptions are true for the project.  

We need to ask: 

- What if Abbyy Finereader does not work for these materals? 
- What if we wanted to test other tools and programs?  
- What if we don’t know how to use Python to data clean?  
- What if we were considering the use of another data cleaning software like OpenRefine? 
- What if all of these programmatic approaches are too much work to extract information from our materials? 
- We should test these methods with a small batch of information: Maybe 5 sources? Maybe 10 sources? 

For each step, we may need to test a few different tools or methods. 

{% include imgwithcaption.html filepath="/assets/img/Workflow_Revised10.JPG" alt="A flow chart where a box ‘.pdf Files’ has four arrows pointing to the following boxes ‘Abbyy Finereader’, ‘AI OCR Tool’, ‘Hand Read and Code’, and ‘Adobe Acrobat Text Recognition’" caption="It is good to test multiple tools to see what their affordances are. You may already have experience with one tool or another, or have a preference for a final product, which helps narrow this phase of prototyping." %} 

In this testing phase, you are trying to learn a tool’s {% include term.html term="affordances" %} and trying to get a sense of how effectively it can be applied based on your team’s skills and the needs of the project. At this phase, you are trying to make sure the tool can operate in the way you need it to do, but you are also testing to see if it fits for other personal or professional needs. Does it cost too much? Does the company that developed this program go against your personal ethics? Is it too hard to train others to use? 

During the prototyping phase, you may come to a best approach. You might also just come across a method you prefer, or one that works best out of a range of imperfect choices. 

{% include imgwithcaption.html filepath="/assets/img/Workflow_Revised10.JPG" alt="A flow chart where a box '.pdf Files' has four arrows pointing to the following boxes 'Abbyy Finereader', 'AI OCR Tool', 'Hand Read and Code', and 'Adobe Acrobat Text Recognition'. Different boxes have been crossed out with notes as to why. 'Abby Finereader' is crossed out because it is 'Too Imprecise'. 'AI OCR Tool' is crossed out because the researchers are 'Concerned about Data Privacy'. 'Adobe Acrobat Text Recognition' is crossed out because it is 'Too Time Intensive'." caption="As you test, you will start to build a preference for a tool, based on what it can do and how you want to use it." %} 

The goal of the prototyping phase is to run into issues, figure out solutions, and create a template for working at a larger scale. 