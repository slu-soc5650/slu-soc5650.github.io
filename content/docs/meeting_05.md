+++
  title = "Meeting 05 - Combining Data Sources"
  
  date = 2021-03-01T00:00:00
  lastmod = 2021-03-01T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 05 - Combining Sources"
  [menu.docs]
  parent = "Module 2"
  weight = 2
+++

<br> 

{{% callout warning %}}
Please submit Lab-04 via GitHub Desktop!

Students in SOC 5650 should also upload their annotated bibliography to their assignments repository!
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Differentiate between different Census data sources.
  2. Select the correct packages and functions for downloading Census geometric and tabular data.
  3. Construct an `sf` object by combining two data sources.

<br>

## Meeting Resources

  * An overview of the meeting can be on the [syllabus](https://slu-soc5650.github.io/syllabus/module-2-data-cleaning.html)
  * Prep videos and entry ticket are on [Blackboard](https://blackboard.slu.edu/)
  * Meeting materials are available on [GitHub](https://github.com/slu-soc5650/module-2-combine-sources) in the `module-2-combine-sources` repository
  * You can follow along with the complete code for Exercise 2 [here](https://slu-soc5650.github.io/module-2-combine-sources/index.nb.html)
  * Lab-05 instructions are available [here](https://github.com/slu-soc5650/module-2-combine-sources/blob/master/assignments/lab-05.pdf)

<br>

## Before Class
### Tasks
Please complete the tasks listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-2-data-cleaning.html), and see [Blackboard](https://blackboard.slu.edu) for the entry ticket link.

<br>

## During Class
### Agenda

  1. Exercise 1 - More on Map Layouts
  2. Exercise 2 - Combining Data Sources
  3. *Break*
  4. Lab-05 and one-on-one meetings
  
### Exercise 1 - More on Map Layouts
To illustrate some of the elements from the [cartography reading](https://slu-soc5650.github.io/syllabus/module-2-data-cleaning.html) assigned for today, please look at [this map of Missouri Highways](https://www.modot.org/missouri-highway-map-archive-1979-2019) (choose 2019, front and break) created by the State of Missouri. Once you have reviewed the map, discuss the following prompts with your group:

  1. *Review from Meeting 3:* Which layers are in figure, and which layers are in ground?
  2. *Review from Meeting 3:* Which map layout elements are present here? (see Brewer, p. 4)
  3. Eevaluate the layout of the front map - how is empty space used? how is proximity between elements used?
  4. Evaluate the layout of the back map - how is empty space used? how is proximity between elements used?
  
### Exercise 2 - Combining Data Sources
We'll introduce two packages, `tigris` and `tidycensus`, to access Census data from within `R`. This provides a significant time savings and makes your work more reproducible. We'll also go over some review of the data wrangling workflow, touching on specific verbs that are useful for prepping data for joins.

The data and example notebook are available in this course meeting's repository, named `module-2-combine-sources`. You can find them in `examples/meeting-04.Rmd`. You can also follow along with the completed code [here](https://slu-soc5650.github.io/module-2-combine-sources/index.nb.html).

<br>

## After Class
The Lab-04 instructions are available in `module-1-cartography` or can viewed online [here](https://github.com/slu-soc5650/module-2-data-cleaning/blob/master/assignments/lab-04.pdf). You'll need to create a new `.Rproj` for it in your assignments repository and then works to clean-up some more Clean Water Act data on polluted rivers and streams in the St. Louis area. You won't need to create a map this week, just focus on wrangling the data.

<br>

## Meeting Reminders
Please don't forget about what is due for next week, which is listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-2-data-cleaning.html). In addition to Lab-05: 

  * the second [final project waypoint](https://slu-soc5650.github.io/final-project/index.html#waypoints) is due next week for *all students*
  * the third [final project waypoint](https://slu-soc5650.github.io/final-project/index.html#waypoints) is due in two weeks for *all students*
