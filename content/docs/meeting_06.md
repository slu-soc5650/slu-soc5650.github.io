+++
  title = "Meeting 06 - Working with Map Projections"
  
  date = 2021-03-08T00:00:00
  lastmod = 2021-03-08T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 06 - Projectings"
  [menu.docs]
  parent = "Module 3"
  weight = 1
+++

<br> 

{{% callout warning %}}
Please submit Lab-05 as well as Waypoint 2 for the final project. Your second waypoint should be submitted via your final project repository.
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Describe map projections and the practical impact they have on GIS work.
  2. Identify the appropriate projections for different map scales.
  3. Apply transformations to projections for geometric data.
  4. Construct geometric data from tabular data that contains `x,y` coordinate pairs.
  5. Create new spatial data files for storing your modified geometric data.
  
<br>

## Meeting Resources

  * An overview of the meeting can be on the [syllabus](https://slu-soc5650.github.io/syllabus/module-3-geoprocessing.html)
  * Prep videos and entry ticket are on [Blackboard](https://blackboard.slu.edu/)
  * Meeting materials are available on [GitHub](https://github.com/slu-soc5650/module-3-projections) in the `module-3-projections` repository
  * You can follow along with the complete code for Exercise 2 [here](https://slu-soc5650.github.io/module-3-projections/index.nb.html)
  * Lab-05 instructions are available [here](https://github.com/slu-soc5650/module-3-projections/blob/master/assignments/lab-06.pdf)
  * Some helpful links for today include:
      * [Interactve map of UTM zones](https://mangomap.com/robertyoung/maps/69585/what-utm-zone-am-i-in-#)
      * [Interactive map of State Plane zones](https://hub.arcgis.com/datasets/23178a639bdc4d658816b3ea8ee6c3ae_0)
      * Coordinate system database
          * [EPSG.io](https://epsg.io)
          * [Spatial Reference](https://spatialreference.org)
      * [Reference for `ggplot2` point shapes](http://www.sthda.com/english/wiki/ggplot2-point-shapes)

<br>

## Before Class
### Tasks
Please complete the tasks listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-3-geoprocessing.html), and see [Blackboard](https://blackboard.slu.edu) for the entry ticket link.

<br>

## During Class
### Agenda

  1. Exercise 1 - Getting Acquainted with ESRI Story Maps
  2. Exercise 2 - Exploring the Mercator Projection
  3. *Short Break*
  4. Exercise 3 - Working with Projections in R
  5. *Short Break*
  4. Lab-06 and one-on-one meetings
  
### Exercise 1 - Getting Acquainted with ESRI Story Maps
Your final projects will involve creating a story map. To get acquainted with these as a medium, we'll take a look at a [sample story map](https://storymaps.arcgis.com/stories/da0df1524c704b488d79bb3e656addb3?_lrsc=3a74f8ba-3735-4900-9084-134c8d7823c8) today. In your group, discuss:

  1. How does this differ from the map layouts we have been discussing the last few weeks?
  2. What are elements of this story map that are appealing?
  3. What are elements of this story map that you might change?

### Exercise 2 - Exploring the Mercator Projection
Both of the "bonus" prep videos for this week ([*The West Wing*](https://www.youtube.com/watch?v=vVX-PrBRtTY&t) and [Vox.com](https://www.youtube.com/watch?v=kIID5FDi2JQ)) mention issues with map projections. The [Mercator Projection's history](https://www.gislounge.com/look-mercator-projection/) underscores a need for easy navigation for ships navigating the world's oceans beginning in the 16th century. In order to maintain the right angles between latitude and longitude lines, the map must distort the shape of the earth as you get closer to both poles. This results, for example, in making Greenland appear as though it is equally sized to Africa. We'll use [The True Size Of...](https://thetruesize.com/) project to explore the distortions that projections can create.

We'll also talk about some projections that are good for mapping at different scales. This largely apply to static maps, and the handout associated with this can be found on [Blackboard](https://blackboard.slu.edu/).

### Exercise 3 - Working with Projections in R
For our work in `R` today, we'll dig into the projection tools in the `sf` package, specifically the `st_transform()` and `st_as_sf()` functions. Since we're working on both changing projections as well as projecting points, we'll also cover how to change points on `ggplot2` maps. Finally, we'll discuss options for saving geometric data using the `st_write()` function.

The data and example notebook are available in this course meeting's repository, named `module-3-projections`. You can find them in `examples/module-examples.Rmd`. You can also follow along with the completed code [here](https://slu-soc5650.github.io/module-3-projections/index.nb.html). *Note that there are some issues with how my code is rendering right now with RStudio, and these are incomplete.*

<br>

## After Class
The Lab-06 instructions are available in `module-3-projections` or can viewed online [here](https://github.com/slu-soc5650/module-3-projections/blob/master/assignments/lab-06.pdf). You'll need to create a new `.Rproj` for it in your assignments repository and make three maps - one of the lower 48 states, one of Alaska, and one of Hawaii - showing health insurance rates. Each map should use an appropriate coordinate system.
      