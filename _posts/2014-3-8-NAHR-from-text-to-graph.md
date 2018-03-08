---
layout: post
title: >-
  NAHR: building a visualization of personal and professional connections in the
  art community of the 17th century
published: true
---

You know those moments when you’re being told of a major incident between someone’s family members, elderly neighbors and visiting cousins? It’s hard to follow, but you still want the drama.

Well I wouldn’t have expected it, but it turns out studying records from art history sounds like  a similar pursuit. Digging through confusing timelines of who married whom, who moved where, and who tutored whose children is a task art historians have to get into in order to retrace the influence of specific actors, the dynamics of communities of artists, the impact of economic factors on the produced art and so on. In 2017, we at the VDA-Lab were approached by the people working on the Cornelia Project to design a visualization that could bring together data collected by researchers in art history, in a way that could help them understand the stories and trajectories of specific persons, and the dynamics of community. The goal of the project being enabling the understanding of influence and impact of artists on their community (and vice-versa).

This data is comprised of parish and guild records, essentially combining personal information (birth and death dates, spouses, children as well as godparents) with what can essentially be described as professional information: masters, pupils, collaborations and so on. 

For this project, we built a tool that took in this data, and represented it visually as an annotated interactive and adapted family tree. This visualization will allow the users to have a quick and synthetic view of the studied subgroup. They'll also be able to interact with it to learn more about specific actors, and access sources and references for the data.






## Tool
Here's a view of the main visualization designed -- It's live, play on! --


<iframe width="1080" height="660" style="margin-left:-140px" src="//homes.esat.kuleuven.be/~hlamqadd/NAHR/simpleTL.html"  ></iframe>


It's important to note that the data we were given was a mock dataset, mostly tailored to the size of the project, in order to build a proof of concept.


### How to read the graph?

Each person's life span is represented by a bar. It's shorter if they lived less, longer if they lived longer. It gets filled up with years passing by as they "consume" some of it.
Each bar is annotated with the person's name, gender, and profession if known.

The structures shown are families. Professional and godparenthood links can be toggled using the button in the bottom right corner

The initial view is "outside of time". But that changes if you select a specific year on the slider to the right, as the graph updates to show the valid information at that point in time. People who have passed away, or who have not been born yet fade, relationships that have not yet happened or are no longer true also fade out 

### What can you do with the graph?

* Toggle the relationship buttons on the bottom right to view other co-existing links

* Adjust the slider to select a year (The colored squares tell you which years have seen more action)

* Hover over a person's name to view more info about them

* Hover over a professional/godparenthood link to get more info about the relationship




## Data

The data we were handed was a ~~messy~~ complex story of love and drama between three families of artists, tapesty producers and merchants. This story was also declined as a spreadsheet summarizing the family and professional links. 

The spreadsheet we received looked a bit like this, listing every possible link between 2 persons.

![screencap of spreadsheet containing names and relationship types]({{site.baseurl}}/images/spreadsheet.png)

There are mainly 3 types of relationships:

• Family: Each actor has a link to their parents, potentially spouse and children.

• Godparenthood links: godparenthood is an important marker of social links in the described social context. We therefore also have each person's link to a godmother and godfather, if known.

• Professional links: We know that some of the people in the dataset have professions, and we also know some have collaborated. In this dataset, only one type of professional collaboration is present, so we're not dividing it up into further subgroups.


## Design choices 




**(a) Time sewn into a graph:**	Family trees are great for showing genealogy, but they don't really show time. The contemporaneity of persons and evolving nature of links do are usually visible in such visualizations. Through interaction, we went for a user-controlled vision of time that shows the family tree as it is at first, but also shows what is true at each moment in time. This approach recognizes the fact that family and community dynamics are just that, dynamic, and there is no ultimate true form of a family tree but a sequence of truths over time.

**(b) Personal cards:**	Each person is much more interesting that can fit a node, so we added tooltip "cards" containing the extra data we could not place in the graph so that users can learn more about every actor. This is also where the sources of the data will be linked to once that aspect of the database is complete, for more reliability.

**(c) Actors and actor ghosts:**	Family and community links matter, and they matter even more to our users because of what they can teach about specific community dynamics. Especially knowing that the goal of this research is to study influence and impact, as these elements do not tend to simply vanish after the death of a person. For this reason, we chose to keep all persons and links visible on the visualization even long after there were gone. The elements are grayed out or fade away, but are still visible to allow for a full understanding of what happened. 

**(d) The active years:**	Some years see more action than others, or simply have more records surviving and archived than others. To give users a direct way of knowing which periods are more interesting to look at, we built a vertical bar chart attached to the time slider, that shows the event frequency across time.



![screenshot of the tool, with labels where each task is answered]({{site.baseurl}}/images/spreadsheet2.png)

_________________

This project was overall a very fun one to work on. Having a description of a dataset and a problem and basically carte blanche on what type of solution should be delivered is always fun. 
At the time of writing, this work was written up as a short paper and is awaiting notification.

A full version of the tool is live [here](http://homes.esat.kuleuven.be/~hlamqadd/NAHR/timeLineView.html) 

Read more about the Cornelia project [here](http://www.projectcornelia.com/)
