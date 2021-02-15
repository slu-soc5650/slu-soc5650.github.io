+++
  title = "Meeting 03 - Cartography 101"
  
  date = 2021-02-15T00:00:00
  lastmod = 2021-02-15T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 03 - Cartography 101"
  [menu.docs]
  parent = "Module 1"
  weight = 3
+++

<br> 

{{% callout warning %}}
Please submit Lab-02 on your own via GitHub Desktop!
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Apply gestalt principles to map reading and map design
  2. Design `ggplot2` maps with both figure and ground layers
  3. Revise `ggplot2` maps to use different color ramps
  4. Employ different break algorithms to "bin" data together on a map

<br>

## Before Class
### Tasks
Please complete the tasks listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-1-course-introduction.html), and see [Blackboard](https://blackboard.slu.edu) for the entry ticket link.

<br>

## During Class
### Agenda

  1. Exercise 1 - Discussing Map Layers and Cartographic Choices
  2. Exercise 2 - Complicating Our `ggplot2` Maps
  3. *Break*
  4. Lab-02 and one-on-one meetings

### Exercise 1 - Discussing Map Layers and Cartographic Choices
To illustrate some of the points about gestalt principles and color in the meeting prep video, please consider the following questions as a group after taking a look at this [map of Ozark National Senic Riverways](http://npmaps.com/wp-content/uploads/ozark-map.jpg), a National Park Service resource in southern Missouri. 

  1. What do you think are the ground layers?
  2. What do you think are the figure layers?
  3. How is the gestalt principle of nearness used?
  4. How is the gestalt principle of similarity used?
  5. What do you think is the hierarchical organization of layers?

### Exercise 2 - Complicating Our ggplot2 Maps
To apply some of our gestalt principles, and also introduce some tools for working with color, we're going to add some complexity to the way we're been using `ggplot2` for mapping. Our goal is to load some data saved in several shapefiles and then:

  1. Create a map using `ggplot()` and *several instances* `geom_sf()`
  2. Manually alter color of layers
  3. Illustrate using `viridis` and `RColorBrewer` to create palettes for thematic maps
  4. Use a custom function to create map breaks
  
All of the materials are available in our [meeting GitHub repo](http://github.com/slu-soc5650/module-1-cartography). 

## After Class
The Lab-03 instructions are available in `module-1-cartography` or can viewed online [here](https://github.com/slu-soc5650/module-1-cartography/blob/master/assignments/lab-03.pdf). You'll need to create a new `.Rproj` for it in your assignments repository and then create a static map of St. Louis showing the extent of owner occupied housing in the city. This map should include the Mississippi River and local highways as ground layers, and include map breaks as well as a `viridis` or `RColorBrewer` palette of your choice.
