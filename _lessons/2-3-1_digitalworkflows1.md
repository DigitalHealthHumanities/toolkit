---
layout: sublesson
structurehead: workflows
title: "How Research Questions Relate to (Digital) Methods"
group: projectmanagement
abstract: "This lesson shows a few examples showing how research questions can be tied to digital methodologies."
lessonnumber: 1
lessonprint: 1
permalink: /lessons/projectmanagement/digitalworkflows/1
nest: nonest
---

For this first activity, we will think about how different programs work together to produce a final research output—a journal article, a book, a digital humanities project. For this activity, we will think about the production of a network graph for a journal article.
The first question to ask is, what is your deliverable?

**Important Term – Deliverable:** Deliverables are concrete materials which are prepared to be shared with others, based on yours and your receiver’s expectations. These can be very polished—like a published book manuscript—or something that is a work in progress—like a draft you submit to a writing group. Deliverables are most important because they give us clear goals to work toward, and help benchmark progress.

For this exercise, we are going to think about publishing this essay in a peer-reviewed, print-based journal in the history of medicine. The idea here is that we will work backwards from a very traditional research output, rather than think about something that might be more digitally specific—like a born-digital journal like the Journal of Digital History. We are using a history journal to think about primary, archival data. 

What might the journal need from its authors for a finished publication? A manuscript, probably written on or exported to a Microsoft Word (.docx) file. If this is the case, then all of our workflow will have to, in some way, feed back into that .docx file.

Before we even get to the network analysis elements, what other programs might we use for the written materials? We need a text editor--Microsoft Word or Google Docs or Open Office or Scrivener. We probably have images, which might need small edits so we should consider an image editor—Adobe Photoshop or GIMP. We also should use a citation manager—Zotero or OneNote. And we may need to generate tables and other figures which may need its own program—Tableau, Airtable, or Microsoft Excel. For just the written components we may have a workflow that looks like this.

<img src="{{ site.baseurl }}/assets/img/workflow1.jpg">

You may notice that some of these programs need to be used outside of Microsoft Word for the submission. Often journals require unique files as part of their submissions if you have images or tables. This workflow is relatively, at least when broken down into the most simple elements, assuming you are not processing data, generating findings with programs or digital platforms.

Let’s think about Gephi. There is an introduction to Gephi in this toolkit.

Usually it is better to use Gephi as the network generator, but the data entry software. We will assume that the workflow uses a pair of comma separated value (.csv) files and is exporting an image of the graph. There will also be some data that we’ll input into the Microsoft Word manuscript, but that that information will be made from analyzing the final graph.

The workflow would look something like this

<img src="{{ site.baseurl }}/assets/img/workflow2.jpg">

Let’s think about two things. The first question is, how does this workflow fit into the manuscript workflow?

For the rest of this activity, we will follow a sketch and reflection style of learning. I will prompt you to sketch out, on a scrap piece of paper, in a digital program (the images for this workshop were made by taking screenshots from Microsoft Whiteboard).

First draw out the manuscript workflow (the first chart) and then try to connect, using arrows how this simple Gephi workflow might fit into it.

Once you have done that, check it against this workflow.

<h3><details>
	<summary>Solution</summary>
	<img src="{{ site.baseurl }}/assets/img/workflow3.jpg">
</details></h3>

Most of the information from Gephi is going into images, which might also need to be cleaned up (resized or made into a different file format). We could also draw a line Gephi directly to Microsoft word because it is informing our writing, but this flow chart is going to get messy quick, so for sake of simplicity I have left that out.

Let’s work backwards again. How are we going to make that comma separated value (.csv) file?

As we learned in the introduction to Microsoft Excel, it is not feasible to handwrite .csv files. Instead we’ll need a spreadsheet software, like Microsoft Excel, from which we’ll export. We also will need to be working with some sort of data, which we will get to next.

Add Microsoft Excel to your sketched workflow. It should connect to Gephi in some way, but it might also connect elsewhere in the workflow.

<h3><details>
	<summary>Example with Gephi</summary>
	<img src="{{ site.baseurl }}/assets/img/workflow4.jpg">
</details></h3>

I added Microsoft Excel because it probably is going to be used in both the creation of .csv files for Gephi and for use in making figures.

The next question is the really sticky one: where are we getting our primary data? How are we processing our data? How are we getting it into the right form for Gephi to read it?
