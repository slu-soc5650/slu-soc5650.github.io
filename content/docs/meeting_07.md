+++
  title = "Meeting 07 - Geoprocessing - Intersect, Select, and Aggregate"
  
  date = 2021-03-15T00:00:00
  lastmod = 2021-03-15T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 07 - Geoprocessing 1"
  [menu.docs]
  parent = "Module 3"
  weight = 2
+++

<br> 

{{% callout warning %}}
Please submit Lab-06 as well as Waypoint 3 for the final project. Your third waypoint should be submitted via your final project repository.
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Describe features that make for effective basemaps.
  2. Perform spatial joins using point, line, and polygon data to identify where geometric features fall in a set of polygon features.
  3. Apply these skills to create counts of points that fall within a set of polygon features.
  
<br>

## Meeting Resources

  * An overview of the meeting can be on the [syllabus](https://slu-soc5650.github.io/syllabus/module-3-geoprocessing.html)
  * Prep videos and entry ticket are on [Blackboard](https://blackboard.slu.edu/)
  * Meeting materials are available on [GitHub](https://github.com/slu-soc5650/module-3-intersect) in the `module-3-intersect` repository
  * You can follow along with the complete code for Exercise 2 [here](https://slu-soc5650.github.io/module-3-intersect/index.nb.html)
  * Lab-07 instructions are available [here](https://github.com/slu-soc5650/module-3-intersect/blob/master/assignments/lab-07.pdf)
  
<br>

## Before Class
### Tasks
Please complete the tasks listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-3-geoprocessing.html), and see [Blackboard](https://blackboard.slu.edu) for the entry ticket link.

<br>

## During Class
### Agenda

  1. Exercise 1 - Basemaps with ESRI Story Maps
  2. Exercise 2 - Geoprocessing using Intersects in `R`
  3. *Short Break*
  4. Lab-07 and one-on-one meetings
  
### Exercise 1 - Basemaps with ESRI Story Maps
*We'll be skipping this tonight.*

### Exercise 2 - Geoprocessing using Intersects in `R`
For our work in `R` today, we'll dig into some initial geoprocessing operations using `st_intersection()` and `st_difference()`. We'll cover working with point, line, and polygon data, and also discuss a common issue with "geometry collections." We'll also review skills for working with projections, and cover using `dplyr`'s `group_by()` and `summarise()` to aggregate counts of points for a set of polygon features.

The data and example notebook are available in this course meeting's repository, named `module-3-intersect`. You can find them in `examples/meeting-examples.Rmd`. You can also follow along with the completed code [here](https://slu-soc5650.github.io/module-3-intersect/index.nb.html). *Note that there are some issues with how my code is rendering right now with RStudio, and these are incomplete.*

<br>

## After Class
The Lab-07 instructions are available in `module-3-intersect` or can viewed online [here](https://github.com/slu-soc5650/module-3-projections/blob/master/assignments/lab-07.pdf). 
