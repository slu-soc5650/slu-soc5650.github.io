+++
  title = "Meeting 12 - Static Maps in R"
  
  date = 2021-04-26T00:00:00
  lastmod = 2021-04-26T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 12 - Static Maps"
  [menu.docs]
  parent = "Module 5"
  weight = 1
+++

<br> 

{{% callout warning %}}
Please submit the sixth final project waypoint as an issue on your GitHub project repository before class today.
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Review processes for creating static maps using `ggplot2`.
  2. Apply themes to `ggplot2` maps.
  3. Create static maps using an alternative package, `tmap`.
  
<br>

## Meeting Resources

  * An overview of the meeting can be on the [syllabus](https://slu-soc5650.github.io/syllabus/module-5-map-products-with-r.html), but please keep in mind that we are switching up the content and ordering of these final two course meetings.
  * The entry ticket is available on [Blackboard](https://blackboard.slu.edu/)

<br>

## During Class
### Agenda

  1. Exercise 1 - Mapping Wildfires
  2. Exercise 2 - Adding Themes to ggplot2 Maps
  3. *Short Break*
  4. Exercise 3 - Creating Maps with `tmap`
  5. *Short Break*
  6. Lab-12 and one-on-one meetings

### Exercise 1 - Grizzly Creek Fire
The Grizzly Creek Fire was part of the 2020 fire season, and burned 32,631 acres in Glenwood Canyon, Colorado. The fire began on August 10th and was not declared fully contained until December 18th. The [StoryMap about the fire](https://storymaps.arcgis.com/collections/6c3a35fdf9d049298874d8c27a6ca0cb?item=4) is part of a collection ESRI maintains of [StoryMaps related to that fire season](https://storymaps.arcgis.com/collections/6c3a35fdf9d049298874d8c27a6ca0cb).

  1. As you look at the map, think about what design features you like and what you might want to tweak or add to your own final project StoryMap. 
  2. At the bottom, take a look at the 3D map rendering of the fire itself. We have not talked about these maps, but they are an option on StoryMaps as well.
  
### Exercise 2 - Adding Themes to ggplot2 Maps
For our work in `R` today, we'll dig into some theme options for `ggplot2` maps after we review the processes for changing point and line symbols (related to our final Brewer chapter). The data and example notebook are available in this course meeting's repository, named `module-5-static`. You can find them in `examples/meeting-examples.Rmd`. You can also follow along with the completed code [here](https://slu-soc5650.github.io/module-5-static/index.nb.html).

### Exercise 3 - Creating Maps with `tmap`
After our review of `ggplot2`, we'll talk about the pros and cons of an alternative mapping package called `tmap`. The data and example notebook are available in this course meeting's repository, named `module-5-static`. You can find them in `examples/meeting-examples.Rmd`. You can also follow along with the completed code [here](https://slu-soc5650.github.io/module-5-static/index.nb.html).

<br>

## After Class
The Lab-12 instructions are available in `module-5-static` or can viewed online [here](https://github.com/slu-soc5650/module-5-static/blob/master/assignments/lab-12.pdf). 

<br>

## Meeting Reminders
Please don't forget about what due in May, which is listed on the [syllabus](ttps://slu-soc5650.github.io/syllabus/module-5-map-products-with-r.html). In addition to Lab-12, there is one final upcoming deadline in May I want to remind you of: 

  * May 17th - all final project materials must be submitted via GitHub. Link to your final StoryMap in your final project's `README.md` file.
  
<br>

## Peer Reviews  
All graduate students should have now received their peer reviews for their repositories and draft papers. In addition to wrapping up your data, code, documentation, papers, and StoryMaps, you should author a "response to reviewer" letter. I will post a sample on Blackboard, but my basic strategy for this aspect of the peer review process is to break up the comments from all the reviewers into action items. Every facet of each review should convert to an action item, but sometimes if there are a lot of minor points, I'll simply say that I addressed the various misspellings instead of listing each one I fixed. At the top, I summarize the major changes I have made to my manuscript since my last submission.

Please create your "response to reviewer" either as a `.md` file or a Word document, and include it in your final project repository. Summarize the main changes you've made, and then break down how you responded to each of the action items in your partner's review (Reviewer 1) and in my review (Reviewer 2). For each action item, add a bullet below it that describes how you addressed the reviewer's concerns.

<br>

## Course Trajectory
We have now covered all facets of the final project. Graduate students will need to apply today's skills for creating publication-ready maps using `R` that will be included in their final papers. Next week's class will cover a final set of skills, picking up where we left off on the first day of class, with interactive maps in `R`.

<br> 

{{% callout warning %}}
Next week will be our last course meeting!
{{% /callout %}}


<br>