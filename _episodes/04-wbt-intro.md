---
title: Workshop Builder Tool Introduction # title of the episode
teaching: 15 # time required to teach (minutes)
exercises: 30 # time required for participants to do the activities (minutes)
duration: # duration for a break, not needed if teaching/exercises are present (minutes)
# summary of the episode content for displaying on the schedule page
summary: An introduction to the Workshop Builder Tool and the Open Research Resource Browser, including a short exercise where you'll set up your own workshop website.
questions: # list of questions we are trying to answer
objectives: # list of learning outcomes
 - Understand the basics of the Workshop Builder Tool
 - Be able to search the Open Research Resource Browser for resources
keypoints:  # list of take-home points
 - The Workshop Builder Tool creates a website like this one with your content
 - The Open Research Resource Browser resources can be added to via our Google Sheets document

is-break:  # whether this episode is a break (has different presentation)
ukrn_wb_rules: # list of rules for the UKRN Workshop Builder tool

day: 1
order: 400000

---

## Workshop Builder Tool

Building a workshop can be a lot of work, and a lot of that work is the same for all of you, despite the specific content being different.
We've tried to streamline the workshop creating process for you with the use of this Workshop Builder Tool.
You can access the tool at <a href="{{ site.ukrn_or_builder }}" target="_blank">{{ site.ukrn_or_builder }}</a>.

### How it works

The tool works by providing an interface to GitHub.
GitHub has a mechanism for hosting GitHub repositories as websites called [GitHub Pages](https://pages.github.com/).
We use GitHub Pages for this website, for example.

The GitHub Pages template we use is fairly complex (based on [The Carpentries' template](https://carpentries.org/)), so to make it easier to manage we built to tool to:
* Allow you to use an existing workshop as a template
* Handle all the git commits and pushes for you
* Keep as much of the code out of the way as possible

### Getting started

You'll need a GitHub account - you can create one via the Builder Tool if you don't already have one.

> ## Create a workshop `5 min`
> 1. Go to the <a href="{{ site.ukrn_or_builder }}" target="_blank">Workshop Builder Tool</a>
> 2. Press the button to log in to your GitHub account (it will let you create one if you need to!)
> 3. **Create a new repository**
> 4. Select a **topic** and a **title** for your workshop, then scroll to the bottom of the Customize Workshop page and click the button
> 5. The 'workshop id' should be a two- or three-letter code for your university/institution followed by `DS` followed by today's date in YYYYMMDD format, followed by `_01`
>   * This id allows us to keep track of where attendees are and to ensure you get a copy of the feedback attendees give
{: .challenge}

You now have a workshop website being generated.
We'll wait a few seconds and then we'll look to see what our website looks like.
While we wait, we'll briefly cover the staging process your edits will go through.

#### Understanding changes
When you make changes using the Workshop Builder Tool the changes are kept in memory.
In order to save the changes to the website you're building, you need to tell the Builder Tool to send the changes to GitHub.
You can do this for individual files, as you'll see in a moment, or you can do it for all of the files you've changed by using the menu on the right (click the 'Save changes to GitHub' button).

Let's now hover over that menu - we should see at the bottom that there's a tick and a message that tells us that our website was built successfully.
If that's the case, click on the 'View workshop website' button to open the website in a new tab.
If you don't see the tick, or there's a cross there, please **ask for help**.

### Adding lessons
Workshops are made up of lessons - individual bits of content which contain explanations, activities, etc.
Each of the pages in this website is a 'lesson'.

You can add and customise lessons created by other users of the Workshop Builder Tool.
There are also template lessons if you want to build yours from scratch.
Let's start by customising an introductory lesson.

> ## Add jspsych-born-open-data Introduction `15 min`
> 1. Click 'Add Items to Stash'
> 2. Enter 'mjaquiery' in the search box to narrow the results down
> 3. Select the dropdown for 'jspsych-born-open-data' and wait while the results are fetched
> 4. Click 'Add items to stash' - you should now see a lot of lessons in the 'Stash'
> 5. Find 'Introduction' and drag it into the 'Day 1' slot
> 6. You'll see a green '+' icon appear in the lesson's icon bar - click it and you'll install the remote lesson into your workshop
{: .challenge}

Now it's installed, you can edit its metadata ('Edit properties' icon) and content ('Edit content' icon).

The content is written in a combination of [liquid, jekyll](https://devhints.io/jekyll), html, and markdown.
The markdown editor will allow you to use the buttons to insert markdown features like **bold**, and _italic_ text, and [hyperlinks](https://example.com/).
You do not need to know any of these to produce content, although being able to copy the examples in the [text lesson template](https://ukrn-open-research.github.io/ukrn-wb-lesson-templates/text-lesson/index.html) will help!
You can always **ask for assistance** with anything you're finding tricky.

You can try editing the data and metadata - once you've done that you'll see a 'Save changes to GitHub' icon appears in the icon bar, and the 'Save changes to GitHub' button becomes available in the right-hand-side GitHub Integration menu.

The 'Discard local changes' button also becomes available, useful for if you make mistakes!
Refreshing the page will have the same effect, and also clear your stash.

Click either of the 'save' buttons and you'll see the website updates in a few seconds - usually under a minute.

> ## Play around
> If you're waiting for us to finish helping others, have a go at **adding** and **customising** some more lessons, or go back to the **'Customize workshop' step** and add some more workshop details there.
{: .challenge}

## Open Research Resource Browser

The <a href="{{ site.ukrn_or_browser }}" target="_blank">Open Research Resource Browser</a> is a tool that reads and filters a Google Sheets document we have created (and to which you can contribute) which lists open research resources.

You should find the Browser intuitive to use, but ask if you're not sure.

> ## Can you... `10 min`
> 1. Find NASA's GeneLab
> 2. Work out how many Humanities resources there are
> 3. Find the data repositories which mention 'sequence' in their description
{: .challenge}

The spreadsheet the resources are taken from is <a href="{{ site.ukrn_or_resources }}" target="_blank">available to view</a> and we welcome suggestions for additional contributions.
Contributions can be added and available instantly, so just ask us to add something if you need it.

## Using the Tools

You don't have to use the tools we provide.
Our aim is that you have a workshop created ready to deliver by the time we finish here today.
Whether you do that using our tools or your own (e.g. making your own slides) we don't mind - we'll help as best we can whatever you choose.

We do hope you'll find the tools useful, of course - and we'd love to know how we can make them better.
You can send any feedback about the tools to <a href="mailto:{{ site.ukrn_email }}?Subject=UKRN Open Research Tools">{{ site.ukrn_email }}</a>.
