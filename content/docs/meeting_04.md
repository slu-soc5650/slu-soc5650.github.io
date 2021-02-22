+++
  title = "Meeting 04 - Data Cleaning Basics"
  
  date = 2021-02-22T00:00:00
  lastmod = 2021-02-22T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 04 - Data Cleaning"
  [menu.docs]
  parent = "Module 2"
  weight = 1
+++

<br> 

{{% callout warning %}}
Please submit Lab-03 on your own via GitHub Desktop!
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Identify common map layout elements.
  2. Select the correct verbs to perform specific data cleaning tasks.
  3. Construct a data cleaning workflow to prepare a data set for mapping.

<br>

## Before Class
### Tasks
Please complete the tasks listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-2-data-cleaning.html), and see [Blackboard](https://blackboard.slu.edu) for the entry ticket link.

<br>

## During Class
### Agenda

  1. Exercise 1 - Discussing Map Layout Elements
  2. Exercise 2 - Data Cleaning
  3. *Break*
  4. Lab-04 and one-on-one meetings

### Exercise 1 - Discussing Map Layout Elements
To illustrate some of the elements from the [cartography reading](https://slu-soc5650.github.io/syllabus/module-2-data-cleaning.html) assigned for today, please look at [this map of the Artic Research and Policy Region](https://prd-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/atoms/files/ArcticPoster.pdf) created by the U.S. Geological Survey. Once you have reviewed the map, discuss the following prompts with your group:

  1. *Review from last week:* Which layers are in figure, and which layers are in ground?
  2. What data does this map layout emphasize? (see Brewer, p. 5)
  3. Which map layout elements are present here? (see Brewer, p. 4)
  4. What are some weaknesses of this map design?
  
### Exercise 2 - Data Cleaning
To apply some of the verbs from our preparatory videos for this meeting, we are going to work on cleaning some data about Clean Water Act violations in Missouri. As we do this, we are going to follow [the data wrangling workflow found here](https://github.com/slu-soc5650/module-2-data-cleaning/blob/master/handouts/wranglingWorkflow.pdf). We'll focus on renaming variables, evaluating our data for missing values and duplicate observations, subsetting both columns and rows, and creating new variables. The data and example notebook are available in this course meeting's repository, named `module-2-data-cleaning`.

<br>

## After Class
The Lab-04 instructions are available in `module-1-cartography` or can viewed online [here](https://github.com/slu-soc5650/module-2-data-cleaning/blob/master/assignments/lab-04.pdf). You'll need to create a new `.Rproj` for it in your assignments repository and then works to clean-up some more Clean Water Act data on polluted rivers and streams in the St. Louis area. You won't need to create a map this week, just focus on wrangling the data.
