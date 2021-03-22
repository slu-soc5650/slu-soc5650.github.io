+++
  title = "Meeting 08 - Geoprocessing - Merge, Dissolve, Centroids, and Buffer"
  
  date = 2021-03-22T00:00:00
  lastmod = 2021-03-22T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 08 - Geoprocessing 2"
  [menu.docs]
  parent = "Module 3"
  weight = 3
+++

<br> 

{{% callout warning %}}
Please submit Lab-07 as well as Waypoint 4 for the final project. Your fourth waypoint should be submitted via your final project repository.
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Describe features that make for effective map layouts.
  2. Perform additional geoprocessing operations including merges and dissolves.
  3. Calculate centroids and buffers for features.
  
<br>

## Meeting Resources

  * An overview of the meeting can be on the [syllabus](https://slu-soc5650.github.io/syllabus/module-3-geoprocessing.html)
  * Prep videos and entry ticket are on [Blackboard](https://blackboard.slu.edu/)
  * Meeting materials are available on [GitHub](https://github.com/slu-soc5650/module-3-dissolve) in the `module-3-dissolve` repository
  * You can follow along with the complete code for Exercise 2 [here](https://slu-soc5650.github.io/module-3-dissolve/index.nb.html)
  
<br>

## Before Class
### Tasks
Please complete the tasks listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-3-geoprocessing.html), and see [Blackboard](https://blackboard.slu.edu) for the entry ticket link.

<br>

## During Class
### Agenda

  1. Exercise 1 - Explaining Maps
  2. Exercise 2 - Additional Geoprocessing in `R`
  3. *Short Break*
  4. Lab-08 and one-on-one meetings
  
### Exercise 1 - Explaining Maps
Take a look at the following three maps, thinking about the three core characteristics that Brewer lays out at the beginning of Chapter 3:

  1. "an informative legend that shows the meaning of map symbols"
  2. "hierarchies in text content, descriptions of mapped calculations, and logical line breaks and spacing"
  3. "well-designed marginal elements, including indicators of scale and direction"
  
The maps we'll discuss are all maps from the CDC's website:

  1. [Stroke Death Rates, Total Population 35+](https://www.cdc.gov/dhdsp/maps/national_maps/stroke_all.htm)
  2. [Stroke Mortality Rates and Population Distribution, Non-Hispanic Whites, by County, Texas](https://www.cdc.gov/dhdsp/maps/gisx/mapgallery/TX-stroke-mortality.html)
  3. [Map Details - Percent of Population Adherent to Blood Pressure Medication and Location of Practices with Collaborative Practice Agreements (CPAs), Rhode Island, 2018-2019](https://www.cdc.gov/dhdsp/maps/gisx/mapgallery/RI-bpmed-cpa.html)
  
As you look at each map and consider the three core characteristics, think about what elements are present on each map, how hirearchies in content are being used, and how informative the legend is.
  
### Exercise 2 - Additional Geoprocessing in `R`
For our work in `R` today, we'll dig into some additional geoprocessing operations using `dplyr`'s `group_by()` and `summarise()`. We'll also discuss using `rbind()` in greater detail, and will talk about `st_centroid()` and `st_buffer()` as well..

The data and example notebook are available in this course meeting's repository, named `module-3-dissolve`. You can find them in `examples/meeting-examples.Rmd`. You can also follow along with the completed code [here](https://slu-soc5650.github.io/module-3-dissolve/index.nb.html). *Note that there are some issues with how my code is rendering right now with RStudio, and these are incomplete.*

<br>

## After Class
The Lab-08 instructions are available in `module-3-dissolve` or can viewed online [here](https://github.com/slu-soc5650/module-3-dissolve/blob/master/assignments/lab-08.pdf). 

<br>

## Meeting Reminders
Please don't forget about what is due for next week, which is listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-4-map-products-with-arcgis.html). In addition to Lab-08, there are also some upcoming deadlines in April I want to remind you of: 

  * the fifth [final project waypoint](https://slu-soc5650.github.io/final-project/index.html#waypoints) is due in two weeks for *all students*
  * students in SOC 5650 will have a draft paper due on April 12th
  * all students will have a draft ArcGIS story map due April 26th

<br>

## Course Trajectory
We are heading into our fourth module next week, focused on creating map products with ArcGIS Online. Now that we've discussed basics of cartography (in Module 1), data cleaning (in Module 2), projections (in Module 3), and geoprocessing (also in Module 3), we're ready to talk about using ESRI's tools for creating interactive maps and Story Maps. You should browse ESRI's [gallery of story maps](https://www.esri.com/en-us/arcgis/products/arcgis-storymaps/stories) to start to get a sense of options, designs, and how interactive maps are used.