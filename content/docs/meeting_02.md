+++
  title = "Meeting 02 - Map Production Basics"
  
  date = 2021-02-08T00:00:00
  lastmod = 2021-02-15T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 02 - Mapping Basics"
  [menu.docs]
  parent = "Module 1"
  weight = 2
+++

<br> 

{{% callout warning %}}
Please come to class with your Lab-01 materials ready to submit!
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Introduce `ggplot2` for static mapping in `R`
  2. Introduce Git and GitHub for analysis development
  3. Distinguish between different scales of maps
  4. Evaluate the effect that normalizing data has on a map

<br>

## Before Class
### Tasks
  
  1. Double-check to make sure you have completed all course onboarding steps (see Blackboard)
  2. Complete Lab-01 from our first course meeting, and come prepared to submit it during class
  3. Complete the two meeting prep videos (see Blackboard)
  4. Submit Entry Ticket 02 (see Blackboard)
  5. Submit your final project memo (see the [final project instructions](https://slu-soc5650.github.io/final-project/topic-data-selection.html))

<br>

## During Class
### Agenda

  1. Exercise 1 - Discussing Map Scale and Features
  2. Exercise 2 - Working with Git and GitHub
  3. *Break*
  4. Exercise 3 - Introducing `ggplot2`
  5. *Break*
  6. Lab-02 and one-on-one meetings

### Exercise 1 - Discussing Map Scale and Features
To illustrate some of the points about scale and detail in the second meeting prep video, we'll take a look at some maps of California from a number of different sources. The goal is to get more comfortable talking and thinking about maps, their purpose, and you need to make them.

  1. Map 1 - [Yosemite Valley Detail Map](http://npmaps.com/wp-content/uploads/yosemite-valley-map.jpg) via the National Park Service / npmaps.com
  2. Map 2 - [Tenaya Lake 2015 7.5 Minute Topo Map](https://prd-tnm.s3.amazonaws.com/StagedProducts/Maps/USTopo/PDF/CA/CA_Tenaya_Lake_20150226_TM_geo.pdf) via pickatrail.com
  3. Map 3 - [Main Yosemite National Park Map](http://npmaps.com/wp-content/uploads/yosemite-map.jpg) via the National Park Service / npmaps.com
  4. Map 4 - [Map of California Counties by Population, Count](https://slu-soc5650.github.io/module-1-basics/results/california_total_population.png)
  5. Map 5 - [Map of California Counties by Population, Density](https://slu-soc5650.github.io/module-1-basics/results/california_population_density.png)
  
For these maps, discuss the following four questions in your breakout groups:

  1. The scale that they are mapped at - which is the largest scale map? Which is the smallest scale map? How do the ones in between differ?
  2. What is the relationship between scale and what you think the intended use of each map might be?
  3. What data and "layers" are needed for each of the maps? For different data, think about whether they are points, lines, or polygons.
  4. Which map, Map 4 or Map 5, is properly normalized? What is the effect of normalization?
  
### Exercise 2 - Working with Git and GitHub
Since we'll be submitting our work through GitHub this semester, the goal of this exercise is to get comfortable with the GitHub Desktop user interface as well as the Git workflow that we discussed in the first meeting prep video this week. We'll talk about GitHub Desktop, and then work through three examples of the workflow:

  1. Clone the `module-1-basics` repo with today's meeting materials
  2. Clone your assignment repo, add `Lab-01`, commit the changes, and submit it
  3. Clone your final project repo, add a `.Rproj` project file to it, and submit it

### Exercise 3 - Introducing ggplot2
We'll be using `ggplot2` this semester to produce static thematic maps in `R`. To get acquainted with `ggplot2`, we'll re-create Maps 4 and 5 above. All of the materials are available in our [meeting GitHub repo](http://github.com/slu-soc5650/module-1-basics). Our goal is to load some data saved in a shapefile (review from last week) and then:

  1. Create a map using `ggplot()` and `geom_sf()`
  2. Add a color `viridis` color palette to the map
  3. Add a title, subtitle, and caption to the map

<br>

## After Class
### Tasks

  1. Complete Lab-02 after and *try to submit it via GitHub on your own*
  2. Follow-up with Chris in your Final Project repo about any outstanding memo questions
  
### Lab-02
The Lab-02 instructions are available in `module-1-basics` or can viewed online [here](https://github.com/slu-soc5650/module-1-basics/blob/master/assignments/lab-02.pdf). You'll need to create a new `.Rproj` for it in your assignments repository (which you cloned during class), and then create a static map using `ggplot2` of Missouri counties' total populations that is appropriately normalized.
