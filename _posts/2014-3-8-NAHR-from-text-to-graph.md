---
layout: post
title: >-
  NAHR: building a visualization of personal and professional connections in the
  art community of the 17th century
published: true
---

You know the times when you’re being described a incident happening between someone’s family members, elderly neighbors and visiting cousins? It’s hard to follow, but you stick around because you still want the drama.
Well I wouldn’t have expected it but it turns out studying records from art history can be a similar experience, where to retrace the influence of specific actors, researchers have to dig into confusing timelines of who married who, who moved where, and who tutored who. In 2017, we at the VDA-Lab were approached by the people working on the Cornelia Project to design a visualization that could bring together data collected by researchers in art history, in a way that could help them understand the stories and trajectories of historical persons, and their impact on their community. 


This data is comprised of parish and guild records, essentially combining personal information (birth and death dates, spouses, children as well as godparents) with what can essentially be described as “professional” information: masters, pupils, collaborations and so on. 

The goal of the project being enabling the understanding of influence and impact of artists on their community (and vice-versa).



## Tool
Here's a view on the main visualization designed -- It's live, play on! --


<iframe width="1080" height="660" style="margin-left:-140px" src="//homes.esat.kuleuven.be/~hlamqadd/NAHR/simpleTL.html"  ></iframe>

### How to read the graph?

Each person's life span is represented by a bar. It's shorter if they lived less, longer if they lived longer. It gets filled up with years passing by as they "consume" some of it.
Each bar is annotated with the person's name, gender, and profession if known.

The structures shown are families. Professional and godparenthood links can be toggled using the button in the bottom right corner

### What can you do with the graph?

* Toggle the relationship buttons on the bottom right to view other co-existing links

* Adjust the slider to select a year (The colored squares tell you which years have seen more action)

* Hover over a person's name to view more info about them

* Hover over a professional/godparenthood link to get more info about the relationship




## Data

The data we were handed was a ~~messy~~ complex story of love and drama between three families of artists, tapesty producers and merchants. This story was also declined as a spreadsheet summarizing the family and professional links. 

The spreadsheet we received looked a bit like this, listing every possible link between 2 persons.

![screencap of spreadsheet containing names and relationship types]({{site.baseurl}}/images/spreadsheet.png)


• Family: Each actor has a link to their parents, potentially spouse and children.

• Godparenthood links: godparenthood is an important marker of social links in the described social context. We therefore also have each person's link to a godmother and godfather, if known.

• Professional links: We know that some of the people in the dataset have professions, and we also know some have collaborated. In this dataset, only one type of professional collaboration is present, so we're not dividing it up into further subgroups.


## Tasks

We were able to identify a number of tasks, and from then on could extract a list of needs our tool needed to answer:

Actor-related tasks
a.  Viewing an actor in the context of their community relationships: Users are interested in seeing one or more actors as they interact with their community in terms of marriage and de- scendance, as well as godparenthood, and professional collaborations.


b. Understanding passed actors legacy: Family matters, and continues to matter. The family bonds should be visible even after the members’ deaths as their place in the community remains existing and their impact may stay valid.

c. Estimating the relationship density of an actor: An actor’s influence on the community may be deduced from the number of links they have to other members. As this changes through time, a user can have an idea of the change in dynamics around a user by looking at how much that density varies. 


Chronology-related

d. Freezing the story in time: Users are sometimes interested in looking at the ties and dynamics between members of a community frozen in a specific year. 

e. Focusing on the time periods with most activity: Some periods in time witness more events than others. we should assist the users in knowing the years with most changes in dynamics.



If you look at the visualization again with these in mind, you can see how each aspect and possible interaction is built to adress one of these tasks.

![screenshot of the tool, with labels where each task is answered]({{site.baseurl}}/images/labeledscreenshot.png)


_________________

This project was overall a very fun one to work on. Having a description of a dataset and a problem and basically carte blanche on what type of solution should be delivered is always fun. 
At the time of writing, this work was written up as a short paper and is awaiting notification.

A full version of the tool is live [here](http://homes.esat.kuleuven.be/~hlamqadd/NAHR/timeLineView.html) 

Read more about the Cornelia project [here](http://www.projectcornelia.com/)
