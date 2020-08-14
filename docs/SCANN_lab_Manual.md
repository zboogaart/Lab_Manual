---
title: "SCANN Lab Manual"
author: "Steven M. Weisberg, PhD"
date: "14 August, 2020"
output:
  bookdown::gitbook:
    split_by: section
    output_dir: "docs"
    book_filename: "SCANN_Lab_Manual.Rmd"
    delete_merged_file: false
  pdf_document:
    includes:
      after_body: after_body.tex
      before_body: before_body.tex
      in_header: preamble.tex
    latex_engine: pdflatex
    number_sections: yes
    toc: yes
mainfont: Helvetica
linkcolor: blue
fontsize: 12pt
---



\pagenumbering{gobble}
\newpage
\pagenumbering{arabic} 


# Welcome

Welcome to the [**Spatial Cognition and Navigational Neuroscience**](https://scannlab.psych.ufl.edu) Laboratory at the University of Florida, directed by Steven Weisberg. If you'd like to view this lab manual as a website, check it out [here](https://htmlpreview.github.io/?https://raw.githubusercontent.com/Scann-Lab/Lab_Manual/master/SCANN_Lab_Manual.html?token=ABQDV4GZIYQLZUIZH3EPDO27H7JBC).

If you are new to the lab, your first job is to read through this manual, then go through the [Onboarding checklist]. 

Maybe you are just joining the lab or need a refresher on lab policy. Or maybe you're just curious about how we do things. Either way, we're glad you're here! This lab manual is an introduction to how we do work and science in the SCANN lab. The material you find here describes some overarching lab policies, the lab structure, and how to get started. It is also a living document and the manual itself is an introduction to some of the tools you will use when working in the lab (like RStudio, Git, and Slack). 

![Lab logo](./SCANN_Lab_Logo_NoOutline_With_Text.png)

Our lab manual is open to the public and can be shared under a GNU-3.0 license (the Github repo is [here](https://github.com/scann-lab/lab_manual), but we have also borrowed heavily from others, including [here](https://github.com/ContextLab/lab-manual), [here](https://handbook-public.themusiclab.org/welcome),  [here](https://github.com/alylab/labmanual), and [here](https://github.com/jpeelle/peellelab_manual/). 

You can also find SCANN lab: 

- [On the web](https://scannlab.psych.ufl.edu)
- [On Twitter](https://twitter.com/scannlab)
- [On Github](https://github.com/scann-lab)
- [On Open Science Framework](https://osf.io/4hbgz)[^OSF]

[^OSF]: You will also find our lab wiki here.


# Working in the lab

In the SCANN lab, we practice careful, deliberate, open science. This means that every person in the lab has a responsibility to make sure their projects are well-documented, reproducible, and undertaken with an eye toward the future. The following are a few more specific guidelines.

## Rights
* **You have the right to a work environment free from prejudice, bias, harrassment, and discrimination**
We have a strong focus on inclusion, diversity, and a harassment-free workplace. At all times, we treat each other, our participants, and our science with respect. (This does not mean we cannot argue - passionately, if need be. Dissenting opinions and knowing when to stand up for your opinion and when to back down, are in fact critical aspects of the scientific process.) You have the right a workplace culture that supports you, your career, and your expressions (as long as these rights don’t violate the rights of others.) 

* **You have the right to make mistakes.** No one is perfect. Dr. Weisberg has (probably) made bigger mistakes than you will during your time in the lab. (Ask him sometime.) Science is hard, and the work we do is at the edge of knowledge. This is very cool. But also means we are much more likely to make mistakes that we don’t catch right away. Below, you’ll see what your responsibilities are if (when) you make a mistake.

* **You have the right to have ideas.** No matter how strange.

* **You have the right to criticize ideas.** You are expected to criticize your own ideas! But you should also think critically about the ideas of others (including and perhaps especially Dr. Weisberg.) And, when you criticize an idea: focus your criticism on the idea not on the person who came up with (including yourself!)

* **You have the right to maintain a healthy work-life balance.** I hope that you love working in the lab, but this does not mean slavish devotion ;). 

## Responsibilities
* **All lab members will prioritize a healthy and supportive lab culture.** 
  The SCANN lab is deeply committed to maintaining a harrassment-free and inclusive culture. All lab members are expected to treat each other with respect, professionalism, and general courtesy. This also means you have a responsibility to ensuring you maintain a healthy work-life balance (whatever this means for you). We strive for diversity, anti-racism, and inclusivity. Some guiding principles are [here](https://coco-net.org/wp-content/uploads/2019/11/Coco-WhiteSupCulture-ENG4.pdf). We also follow [UF harrassment policy](https://hr.ufl.edu/forms-policies/policies-managers/sexual-harassment/). 

* **This is a professional work environment.** 
We keep things professional both for ourselves and especially when we interact with people outside of the lab and *most especially* participants. We owe our participants a huge debt of gratitude, regardless of their compensation, because they are taking the time to provide us with their data. Treat each one with the utmost respect and care. Professionalism means appropriate dress and respectful demeanor (cursing, loud music, messiness discouraged). Professionalism also means upholding your commitments - being on time for your shifts; cleaning up after yourself; sticking to deadlines. It also means communicating effectively. (To reiterate - you can make mistakes! Professionalism means communicating about them when you do!) Lastly, professionalism means appropriateness in all things (including humor; off-color jokes or jokes at the expense of others will not be tolerated). This applies for all times you're at work, but again *especially* when running participants. Finally - professionalism does NOT MEAN no fun! Work should absolutely be fun in a way that is fun for everyone!  

* **You are a team member first.**
  As a lab, we can only thrive by relying and counting on each other. Treat everyone in the lab (and anyone related to the lab, including participants, collaborators, mentors) with respect and care. Respect their time, their preferred hours, and their needs. Help them when they ask (within reason), and help build a culture of respect and honesty.
Work with care. Measure twice, cut once. Document your workflows. Save and backup all raw data and code (on a minimum of two of these locations: Hipergator, Dropbox, OneDrive). In preparation phase, make sure everything is clearly labeled, and the experimental paradigm captures data as expected. It is best practice to write analysis code on simulated or pilot data as proof of principle and good sanity checking. In the experiment phase, make sure raw data are being regularly backed up. In the analysis phase, make sure difficult-to-reproduce products are also backed up, and that all analyses are reproducible and documented. In the submission phase, all materials should be able to uploaded to OSF, OpenNeuro, or another online repository in preparation for submission.

* **Our goal is research products**
  Posters, presentations, and publications are the traditional academic products, and you will be expected to produce or contribute to these as a member of the lab. But we also value contributions of: data sets (documented and described), software packages (and analysis pipelines), and ‘reproducible sandboxes’ (Jupyter Notebooks). These research products are rarely peer-reviewed, but provide invaluable tools for the broader research world and their creation is not taken lightly.

# Personnel Expectations {.tabset}

## PI
* I am responsible for the overall lab vision and direction. This mainly includes developing project ideas and obtaining lab funding. But on a daily basis, it also means I am responsible for ensuring the lab produces research products. 
* I am responsible for contributing to the professional development of all lab members. I will try to prioritize this depending on the goals of each individual, but the better we can communicate about your goals, the more successful I will be in this regard. 
* I will support your general education in psychology, broader education in related fields, and specific education in the cognitive neuroscience of spatial navigation. 
* I will contribute to all ongoing projects in the form of: commenting on written drafts, presentations, and posters; helping develop and troubleshoot analyses; ensuring all resources needed for a project are available; providing opportunities for networking, collaboration, and professional development; designing and implementing experiments and protocols; helping manage the lab infrastructure (including analysis pipelines, data backup, and data storage). 
* I will support the physical and mental health and safety of everyone in the lab. 

## PhD Students
In general PhD students have a fairly loose leash as long as they are making progress on projects. In practice, this likely means there will crunch times where you're working hard to get things done and lighter times, when you can take it easy. Please let the PI know, though, if you plan to take extended time off (more than a few days).

PhD students are expected to: 

* Develop and manage an independent project. 

* Know the literature and learn the skills related to their project. 

* Have a strong grasp of (nearly all aspects of) cognitive neuroscience; a breadth of knowledge from areas closely related (psychology, mostly); and a familiarity with related disciplines (biology, anthropology, philosophy, etc.)

* Grow skills in writing, data analysis, experiment administration and protocols, and presentation. 

* Generate (ideally and roughly) one research product per year in the lab. 

* Seek out opportunities for awards (fellowships, travel awards)

* Advocate for what they think and what they need to do their jobs

* Develop (or maintain) healthy work habits and a good balance.

## Lab Manager
The lab manager should have a more regular schedule to ensure a stability in the lab. Due to the nature of OPS positions at UF, 8 hours per day is expected, and these hours should occur roughly between 8am and 6pm. There will be exceptions to this - weekend or late night fMRI scanning sessions come to mind - and these hours can be 'made up for' during the week. Time off requests can be somewhat informal, but should be submitted to the PI in writing so we have a record of such things. 

The Lab Manager is expected to: 

* Facilitate lab business, including: 

  * Recruiting participants

  * Organizing and documenting data storage and backups

  * Updating the lab website and Twitter

* Facilitate projects, including: 

  * Managing human subject payments

  * IRB protocol updates

  * Putting projects online (via Prolific, M-Turk, Pavlovia, etc.)

  * Running experiments

* Contribute to their own project (this will depend on the particular person, but all lab managers will have the opportunity to work on their own research project(s)).

* Develop and maintain code, including: 

  * Lab github

  * Lab Hipergator account(s)

  * Virtual Silcton

* Develop and maintain documentation, including: 

  * Lab experimental and consent protocols

  * fMRI administration checklists

  * Virtual Silcton website administration protocols

  * fMRI pipelines and data analysis

## Undergraduate RAs (PSY4911)
Undergraduate research assistants help with research duties. But, especially if this is your first time working in a research lab, you should not just blindly go about your work and do what your told. Look for ways you can actively contribute to the lab. This includes generating your own ideas, but also developing your own skills. You should not have empty time in the lab, but rather pick a skill you're interested in learning (consult with your grad mentor or Dr. Weisberg if necessary), and spend your free lab time teaching yourself. 

Undergraduate research assistants are expected to:

* Work in the lab 3-hours per credit per week; the general minimum is 9-hours per week (though the number of credits can be less than 3)

* Contribute to a project, including: 
  
  * Recruiting participants
  
  * Running participants 
  
  * Developing a project (collecting stimuli, coding the study)
  
  * Coding data
  
  * Analyzing data (to some extent)
  
* Develop their own skills, including: 

  * Knowledge of fMRI
  
  * Ability to code in Python, R, Matlab, and C# (Unity3D). 
  
  * Knowledge of the literature of cognitive neuroscience as pertains to their projects.
  
## Undergraduate Honors Students (TBD)
Section under construction

# Doing Science in the SCANN Lab

The SCANN lab is committed to open science, careful work practices, and multi-disciplinary shenanigans! What does this mean? There are three inter-related areas that are important to our approach. 

## Open science

1. Data, material, and code from all projects will be hosted publicly and shared[^Within a reasonable timeframe; obviously, nothing will be shared before we are ready to publish or while we are working through the data]. In practice, this means projects will be hosted on one or all of the following sources: [OSF](osf.io), [Figshare](figshare.com), [OpenNeuro.org](OpenNeuro.org), [Github](github.com). 

2. Projects will, whenever possible, be **pre-registered**. In practice, this means nearly all projects will be pre-registered in some form. Pilot projects may be the exception. See guides on [OSF](https://osf.io/prereg/) and [Aspredicted.org](aspredicted.org). 

3. Papers will be made available in pre-print form (e.g., [biorxiv](biorxiv.org), [psyarxiv](https://psyarxiv.com/)). 

## Data management

1. Data you collect in the lab will be backed up in two of these three locations (in addition to your local computer): 
  * UF Onedrive (folder shared with lab manager and/or Dr. Weisberg)
  * UF Hipergator (/orange)
  * Lab hard drives
  
2. Raw data MUST be backed up and not touched following lab protocols (with Readme.md documentation). Always work on a copy of the raw data when conducting analyses. 

3. De-identified or anonymized raw data may also be hosted online for sharing. For fMRI data, structural scans must be de-faced (https://pypi.org/project/pydeface/). 

## Careful work 

You will hear me use the term Sanity Check. We should all strive to be a little bit obsessive about our data and analyses. Mistakes absolutely happen, but we should do as much as we can to prevent them and detect them. The following practices have helped me immensely. 

* Develop a habit of documenting everything you do the *second time you do it*. (Why the second time? If you do it the first time, you may never do it again. If you do it a second time, you will almost certainly need to do it a third - it is now likely worth the time to document it). 

* Use the [Lab Wiki](https://osf.io/d8ke4/). 

# Communication 

Science, especially as practiced in the SCANN Lab, is a collaborative endeavor, which means good communication is key. Here are the main ways the lab communicates.

One thing we often forget about is communicating with ourselves. This means *good documentation* so people don't have to reinvent the wheel. We will follow 

## Lab meeting
Lab meetings are held weekly during the semester (time TBD) and intermittently through the summer. Lab meetings are approximately two hours long. The first ~20-30 minutes consist of lab updates in which each lab member briefly (5 minutes or so) explains what constituted the bulk of their work that week; what progress was made, what hurdles were hit; and any general info they encountered relevant to the lab. The remaining 1-1.5 hours is provided for one lab member to give a presentation. The presentation can range widely (almost all formats are acceptable). Here are a few examples: 

* A journal club / discussion of an article

* A project proposal / plan

* A discussion about a general issue in science (e.g., preregistration, p-hacking, etc.)

* Technique or tutorial (relevant to almost anything in the lab - e.g., Git or how head direction cells work; an MVPA crash course or how to organize folders for a project)

* A data talk (e.g., where you have data but need help thinking through what it means, what to do next, or what you might not have thought of)

* A polished (practice) presentation or job talk

## In-person meetings

In-person meetings (in person or via Zoom) are a great way to work directly and solve a particular problem or make a plan of action. But they are also usually very time-intensive. Lab members may have regularly scheduled meetings with me during the semester, but anyone should always feel free to schedule a meeting. Before asking about a meeting, however, ask yourself three things: 

1. Could this be solved via email? 
  If yes, send email. If no...

2. What is the purpose of the meeting? (In other words, what is the agenda?) Make sure the purpose is in the email to schedule it. 

3. What are the necessary inputs to the meeting? (Do we have all information we need to facilitate the meeting; if not, what are we waiting for? Are all necessary people involved?) 

4. What are the expected outputs? Always ask yourself at the end of the meeting whether you know what the action items are (who will do what). 

## Slack

Our lab [Slack](scannlab.slack.com) is the source for daily lab communication. Our communication via Slack takes three forms. 

* Easy instant messaging (@everyone; @steve weisberg)

* Communication about a particular topic. This is the purpose for channels. (#neurofeedback, #lab-purchasing). Feel free to start your own channel about a specific topic. Don't forget to invite the relevant people! 

* Updates and integration with other services. Check out integrations with Google Calendar, Github, Trello, and more!

## Trello

Our lab to-do lists. The [Onboarding checklist] is on Trello. I recommend that everyone use Trello as their own to-do list manager, but I would strongly encourage using the shared to-do list feature for projects we're working on. Note that cards can be assigned due dates and assigned to specific people, who can indicate when they are finished particular tasks. 

## Email 

Official communication, notifications, etc. I sometimes use interchangeably via Slack. The one difference is any communication regarding participants absolutely needs to happen through UF email. 

# Resources

## General Lab

### RMarkdown

* This lab manual is written in RMarkdown. If you'd like to contribute, you should! 

### Zotero

## Literature

Below are a few seminal lists of readings that any lab member can start with. Pick a topic and dive in. 

Active members of the lab would do well to track the literature on their own. Here a few tips for doing so: 

* Set up Google Scholar alerts 

* Set up Feedly and integrate that with journals you read regularly

* Become active on Cog. Neuro Twitter (seriously, I find way more articles that I actually read in this way than the other two methods!)

### Cognitive Neuroscience

### fMRI

### Spatial Navigation 

## Coding

### General 

* Git

* Bash

* Tools
  
  * Anaconda for Python
  
  * Atom editor

### fMRI

* 

### Unity3D

### R

### Python

### Matlab




# Onboarding checklist



<!--chapter:end:SCANN_lab_Manual.Rmd-->
