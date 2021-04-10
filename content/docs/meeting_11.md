+++
  title = "Meeting 11 - ArcGIS StoryMaps - Design"
  
  date = 2021-04-10T00:00:00
  lastmod = 2021-04-10T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 11 - StoryMaps 2"
  [menu.docs]
  parent = "Module 4"
  weight = 3
+++

<br> 

{{% callout warning %}}
Please submit Lab-10 *as an issue in your assignments repository* before the beginning of this meeting.
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Create new attribute columns and edit existing columns using ArcGIS Online.
  2. Apply labels and pop-ups to ArcGIS Online web maps.
  3. Identify different design elements on ArcGIS StoryMaps.
  4. Modify a basic ArcGIS StoryMap by adding design elements to enhance its presentation.
  
<br>

## Meeting Resources

  * An overview of the meeting can be on the [syllabus](https://slu-soc5650.github.io/syllabus/module-4-map-products-with-arcgis.html)
  * The entry ticket is available on [Blackboard](https://blackboard.slu.edu/)
  * You can login to [ArcGIS StoryMaps here](https://storymaps.arcgis.com)
  * You can login to [ArcGIS Online here](https://www.arcgis.com/home/signin.html)

<br>

## Before Class
### Tasks
Please complete the tasks listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-4-map-products-with-arcgis.html), and see [Blackboard](https://blackboard.slu.edu) for the entry ticket link. Please make sure you have completed **all** work both from the in-class exercises last class and the lab, because you will need them for today's in-class exercises.

<br>

## During Class
### Agenda

  1. Exercise 1 - Labeling
  2. Exercise 2 - Adding Labels and Pop-ups to Web Maps
  3. *Short Break*
  4. Exercise 3 - Adding Design Elements to StoryMaps
  5. *Short Break*
  6. Lab-11 and one-on-one meetings
  
## Exercise 1 - Glacier National Park
Glacier National Park is located in northern Montana along the U.S.-Canadian border. We'll start by looking at this [static map of the National Park](http://npmaps.com/wp-content/uploads/glacier-national-park-map.jpg) before we look at an [ESRI StoryMap about avalanche activity](https://www.nps.gov/gis/storymaps/cascade/v1/index.html?appid=2d5a9d390a034a7cb4f2f3fc66af107c) along the iconic Going-to-the-Sun Road. On the static map, the Going-to-the-Sun Road is highlighted using dark red. It travels east/west across the spine of the Rocky Mountains.

For the static map, consider the following questions:

  1. How are labels differentiated from each other based on feature categories?
  2. What are some examples of labels that have splined text?
  3. What are some examples of leader lines?
  4. What are some examples of callouts (from Chapter 5)?
  
For the StoryMap, consider the following questions:

  1. Think about the characteristics you find appealing about the StoryMap itself.
  2. What types of media and design features are present on the map?
  3. On the interactive map located approximately half-way down, how are labels and pop-ups used?

## Exercise 2 - Adding Labels and Pop-ups to Web Maps
To illustrate how ArcGIS Online provides options for labeling and pop-ups, we'll create a new version of our Louisiana Purchase map. We'll start by creating a bit of additional data for mapping purposes. Using the `Show Table` option in the `Content` pane, we'll add a new character column to illustrate the type of territory each feature represents. We'll add the values `State`, `Territory`, or `Federal District` as appropriate.

Once our column has been created, we can configure pop-ups by turning them on and off. We can also modify pop-ups by changing their titles, and using different types of contents (lists of fields, descriptions of one field, and custom attributes to display). Alternatively, we can use just the title itself for the pop-up contents.

For labels, we'll discuss how to modify both their contents, use the halo effect, and change their visibility range.

## Exercise 3 - Adding Design Elements to StoryMaps
### Covers
We'll start by working on the cover of the StoryMap, adding a photo from the Library of Congress of [slave quarters at the Ste. Genevieve Hotel](https://www.loc.gov/item/mo0918/) in Ste. Genevieve, MO. After we add the photo, we'll discuss the various arrangements covers can take on.

### Adding Media
There are two main sources of media we'll be adding to our StoryMaps - images and videos. Below the map of the Louisiana Purchase, we'll add a [drawing of Thomas Jefferson](https://www.loc.gov/item/2004669440/), also from the Library of Congress, alongside the quote:

  > [T]his little event, of France possessing herself of Louisiana, ... is the embryo of a tornado which will burst on the countries on both shores of the Atlantic and involve in it’s effects their highest destinies.

We'll also work on adding videos by embedding [this Missouri Historical Society video about Lewis and Clark](https://www.youtube.com/watch?v=uBsEDCMBCds).

Finally, we'll add an image of [Henry Clay](https://en.wikipedia.org/wiki/Henry_Clay) to our sidecar. Like our other images today, this is also [from the Library of Congress](https://www.loc.gov/item/2009633654/). Clay, as a Senator from Kentucky helped broker the Missouri Compromise.

### Other Design Features
In addition to media, we'll discuss adding buttons to link to additional content, and separators to create sections.

### Selecting and Editing Themes
Finally, we'll discuss both changing the theme between the stock ArcGIS Online themes as well as editing a custom theme to change the colors, button, and separator appearance.

<br>

## After Class
### Lab-11
The Lab-11 instructions are available in `module-4-storymap-2` or can viewed online [here](https://github.com/slu-soc5650/module-4-storymap-2/blob/master/assignments/lab-11.pdf). This exercise picks up where we have left-off with the in-class exercise, changing the theme, modifying the cover, and adding an additional image and another video embed.

### Lab-11 Replication Materials
A replication StoryMap will be available after class.

<br>

## Meeting Reminders
Please don't forget about what is due for next week, which is listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-4-map-products-with-arcgis.html). In addition to Lab-11, there is one final upcoming deadline in April I want to remind you of: 

  * all students will have a draft ArcGIS story map due April 26th - instructions have been added to the [final project document](https://slu-soc5650.github.io/final-project/arcgis-storymap.html)

<br>

## Peer Reviews  
Additionally, students in SOC 5650 will be paired up this week and asked to review their partner's GitHub repository as well as their draft paper. Each student should open an issue on their partner's GitHub repository and provide three sets of feedback:

  1. The first section should, in approximately sentences, describe the topic of the project being reviewed and provide some **initial positive feedback** (ex - "The repository is well-organized and the paper draft presents a clear picture of their data.")
  2. The second section should provide **major points** for author to address. Areas to focus on for reviews are: 
      * the structure and organization of the GitHub repository - have good principles of analysis development been followed? is it easy to follow their code? is their narrative text descriptive and helpful?
      * the structure and organization of the paper - are the major sections present? clear and easy to read? are their conceptual or organizational gaps that need to be addressed?
  3. The third section should provide **minor points** for the author to address. These may be small changes or clarifications, grammar or spelling issues you notice, or small suggestions to improve the project.
  
Reviews should be **constructive** - your goal is not to tear down your partner's project but provide them with concrete guidance on how to **improve** their work. Even when you are being critical, be positive and supportive while also being honest. 

Provide at least one major point for your partner's repository and two major points with the paper. Likewise, aim to provide at least two minor points for the repository and two for the paper. 

Reviews are due by 4:15pm next Monday (April 18th).

<br>

## Course Trajectory
We have now covered all facets of the final project *except creating publication-ready maps using `R`, which students in SOC 5650 will need to include with their final papers*. From here, we'll spend two weeks going deeper on creating both static and interactive maps using `R`.

<br> 

{{% callout warning %}}
Next week will be a working session for the final project. Attendance to class is not required, but Chris will be available in our class Zoom meeting for one-on-one meetings from 4:15pm to 5:30pm. Feel free to drop-in if you would like to chat!
{{% /callout %}}
