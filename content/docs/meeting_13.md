+++
  title = "Meeting 13 - Interactive Maps in R"
  
  date = 2021-05-03T00:00:00
  lastmod = 2021-05-03T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 13 - Interactive Maps"
  [menu.docs]
  parent = "Module 5"
  weight = 2
+++

<br> 

{{% callout warning %}}
Please submit Lab-12 to your GitHub assignments repository before class today.
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Review processes for creating interactive maps using `leaflet`.
  2. Create more complex interactive maps that include palettes, customized pop-ups, legends, and overlaid features.
  3. Identify options for sharing `html` documents with embedded maps.
  
<br>

## Meeting Resources

  * An overview of the meeting can be on the [syllabus](https://slu-soc5650.github.io/syllabus/module-5-map-products-with-r.html), but please keep in mind that we are switching up the content and ordering of these final two course meetings.
  * The entry ticket is available on [Blackboard](https://blackboard.slu.edu/)

<br>

## During Class
### Agenda

  1. Exercise 1 - Adding Complexity to `leaflet`
  2. Exercise 2 - Sharing `leaftlet` Maps
  3. *Short Break*
  4. Lab-13 and one-on-one meetings

### Exercise 1 - Adding Complexity to leaflet
For our work in `R` today, we'll dig into some additional options for `leaflet` maps after we review the processes for creating a basic map. The data and example notebook are available in this course meeting's repository, named `module-5-leaflet`. You can find them in `examples/meeting-examples.Rmd`. You can also follow along with the completed code [here](https://slu-soc5650.github.io/module-5-leaflet/index.nb.html).

### Exercise 2 - Sharing leaflet Maps
It is easy to share `leaflet` maps. Once we have a completed `.Rmd` notebook, we'll change the output type to `html_document` and also add two output options to the final chunk. The `echo = FALSE` option removes the code block, and the `out.width = '100%'` option makes the map take up the full-width of the document. When we knit it again, we get an `html` file that can be emailed or turned into a simple website.

## Meeting Reminders
Please don't forget about what due in May, which is listed on the [syllabus](ttps://slu-soc5650.github.io/syllabus/module-5-map-products-with-r.html). In addition to Lab-13, there is one final upcoming deadline in May I want to remind you of: 

  * May 17th - all final project materials must be submitted via GitHub. Link to your final StoryMap in your final project's `README.md` file.
  
<br>

## Course Trajectory
This week's content is strictly "bonus" material that is not a part of the final project. 

<br> 

{{% callout warning %}}
This week is our last course meeting! If you need a final one-on-one with me before the final project submission, please send me an email!
{{% /callout %}}

<br>
