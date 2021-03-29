+++
  title = "Meeting 09 - ArcGIS Online"
  
  date = 2021-03-29T00:00:00
  lastmod = 2021-03-29T00:00:00
  
  draft = false  # Is this a draft? true/false
  toc = true  # Show table of contents? true/false
  type = "docs"  # Do not modify.
  
  # Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
  # weight = 3
  
  # Add menu entry to sidebar.
  linktitle = "Meeting 09 - ArcGIS Online"
  [menu.docs]
  parent = "Module 4"
  weight = 1
+++

<br> 

{{% callout warning %}}
Please submit Lab-08 before the beginning of this meeting.
{{% /callout %}}

<br>

## Meeting Goals
This course meeting has an emphasis on the following goals:

  1. Differentiate between different static map export formats.
  2. Discuss caching, and its implications for how we create web maps.
  3. Summarize considerations for licensing maps and map products.
  4. Create ArcGIS Online feature layers based on data exported from `R`.
  5. Design reference and thematic web maps using ArcGIS Online.
  
<br>

## Meeting Resources

  * An overview of the meeting can be on the [syllabus](https://slu-soc5650.github.io/syllabus/module-4-map-products-with-arcgis.html)
  * The entry ticket is available on [Blackboard](https://blackboard.slu.edu/)
  * This [guide to adding images to ArcGIS StoryMaps](https://www.esri.com/arcgis-blog/products/arcgis-storymaps/constituent-engagement/images-in-arcgis-storymaps/) will be useful as you consider content for future course meetings and your final project.
  * You can login to [ArcGIS Online here](https://www.arcgis.com/home/signin.html)

<br>

## Before Class
### Tasks
Please complete the tasks listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-3-geoprocessing.html), and see [Blackboard](https://blackboard.slu.edu) for the entry ticket link. Please make sure you have also created your password and successfully logged into to ArcGIS Online.

<br>

## During Class
### Agenda

  1. Exercise 1 - Sharing Maps
  2. Exercise 2 - Uploading Data to ArcGIS Online
  3. *Short Break*
  4. Exercise 3 - Mapping the Missouri Compromise using ArcGIS Online
  5. *Short Break*
  6. Lab-09 and one-on-one meetings
  
### Exercise 1 - Sharing Maps
Take a look at [this StoryMap](https://storymaps.arcgis.com/stories/8eba6b85803b4b56b6389abcc74708a8). As you scroll through it, give some thought to the following points:

  * Think about the characteristics you find appealing about the StoryMap itself.
  * When get to the web map in the section titled "A New Road," think about how long it takes to load and what data is present on the map. This is related to the caching discussion in the Brewer article for this week. 
  * Scroll down a bit further to the section "Mapping conservation priorities" and check out the two map images that have been exported from ArcGIS Pro. Does it seem crisp or pixilated? 
  * Finally, look further for any evidence of copyright or licensing.

### Exercise 2 - Uploading Data to ArcGIS Online
[ArcGIS Online](https://www.esri.com/en-us/arcgis/products/arcgis-online/resources) is the web platform associated with the broader ArcGIS ecosystem. You can [sign-in here](https://www.arcgis.com/home/signin.html). Our focus for this exercise is on the `Content` section, which we'll use to [add items](https://doc.arcgis.com/en/arcgis-online/manage-data/add-items.htm). While you can add quite a few different types of files, we are going to focus on adding spatial data that you have cleaned and prepared in `R`:

  * If you have exported a `.geojson` file, you can upload it directly to ArcGIS Online.
  * If you have exported a shapefile (`.shp`), you need to **zip** all of its component files into a single archive before uploading to ArcGIS Online. Here are some instructions for creating `.zip` files on [macOS](https://support.apple.com/guide/mac-help/zip-and-unzip-files-and-folders-on-mac-mchlp2528/mac) and [Windows](https://support.microsoft.com/en-us/windows/zip-and-unzip-files-8d28fa72-f2f9-712f-67df-f80cf89fd4e5). If you have older versions of either operating system, you may have to look for alternative instructions.
  
Regardless of which format you upload, you **must** add at least one tag, and can optionally add metadata to your files. For this class, I do want you to add metadata that includes a description, a note about the data source, and a [Creative Commons CC-BY 4.0 license](https://creativecommons.org/licenses/by/4.0/).

For this exercise, we are going to upload three files that are available in our meeting's [GitHub repository](https://github.com/slu-soc5650/module-4-arcgis-online):

  1. `MO_HISTORIC_Louisiana_Purchase.geojson` - the boundaries of U.S. states and territories as of 1803-04-30, when the Louisiana Purchase was completed
  2. `MO_HISTORIC_1820_Census.zip` - a zipped shapefile (`.shp`) showing the boundaries U.S. states and territories as of 1820-12-31 along with the the total populations of most (but not all) of these jurisdictions
  3. `MO_HISTORIC_State_1821.geojson` - the boundaries of U.S. states and territories as of 1821-08-10, when Missouri officially became the 24th state
  
We're focusing on Missouri statehood not just because it is our bicentennial this year, but also because Missouri and Maine's aspirations were linked together in what was known as the [Missouri Compromise](https://en.wikipedia.org/wiki/Missouri_Compromise). Maine was admitted a free state, where slavery was not legal. Missouri was admitted as a slave state. As part of Missouri's statehood, Congress agreed not to admit any additional slave states north of the [36 degree, 30 minute north parallel](https://en.wikipedia.org/wiki/Parallel_36°30′_north#/media/File:Missouri_Compromise_Line.svg). This corresponds to the majority of Missouri's southern border with Arkansas. 

The Missouri Compromise codified pre-existing geographic distinctions over slavery, and set the stage for a balancing act that that the United States engaged in until 1854. That year, Congress passed the [Kansas-Nebraska Act](https://en.wikipedia.org/wiki/Kansas–Nebraska_Act), which gave both territories the right to decide for themselves if they would allow slavery. This repealed the Missouri Compromise, and set the stage for the guerrilla war known as ["Bleeding Kansas"](https://en.wikipedia.org/wiki/Bleeding_Kansas). This violent conflict set the stage for the Civil War, and involved the participation of many pro-slavery Missouri residents known as ["Border Ruffian"](https://en.wikipedia.org/wiki/Border_Ruffian) who flooded the Kansas Territory to fight for the expansion of slavery there.

If you are interested in learning more about this period in Missouri's history, I highly recommend my colleague Walter Johnson's book [*The Broken Heart of America: St. Louis and the Violent History of the United States*](https://www.basicbooks.com/titles/walter-johnson/the-broken-heart-of-america/9780465064267/).

### Exercise 3 - Mapping the Missouri Compromise using ArcGIS Online
Now that we have our shapefile and `.geojson` files loaded, we're going to make a couple different ArcGIS Online web maps:

  1. A reference map of the Louisiana Purchase relative to other territories in the United States
  2. A thematic map of state and territorial populations as of the 1820 Decennial Census
  3. A reference map of the Missouri Compromise
  
Along the way, we'll discuss the following concepts:

  1. Adding content to an ArcGIS Online Map
  2. Saving an ArcGIS Online Map
  3. Re-ordering and re-naming layers
  4. Viewing attribute tables
  5. Changing an individual layer's style
  6. Filtering (i.e. subsetting) features in a layer
  7. Sharing ArcGIS Online web maps

<br>

## After Class
### Lab-09
The Lab-09 instructions are available in `module-4-arcgis-online` or can viewed online [here](https://github.com/slu-soc5650/module-4-arcgis-online/blob/master/assignments/lab-09.pdf). This exercise picks up where we have left-off with the in-class exercise, showing Missouri's population after its first decade of statehood during the 1830 Decennial Census.

### Lab-09 Replication Materials
#### Data
The replication data, stored as a Feature Layer, are [available here](https://arcg.is/0KbW8W).

#### Map 1
The replication for Map 1 can be [viewed here](https://arcg.is/1Di4Du) and is embedded below.

<style>.embed-container {position: relative; padding-bottom: 80%; height: 0; max-width: 100%;} .embed-container iframe, .embed-container object, .embed-container iframe{position: absolute; top: 0; left: 0; width: 100%; height: 100%;} small{position: absolute; z-index: 40; bottom: 0; margin-bottom: -15px;}</style><div class="embed-container"><iframe width="500" height="400" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" title="SOC 4650/5650 - Intro to GIS - Lab-09 Map 1" src="//slustl.maps.arcgis.com/apps/Embed/index.html?webmap=3c6f04625cec41f88555d2beacb6f466&extent=-164.9793,6.5927,-35.1648,64.1365&zoom=true&previewImage=false&scale=true&disable_scroll=true&theme=light"></iframe></div>

#### Map 2
The replication for Map 2 can be [viewed here](https://arcg.is/1jzqna2) and is embedded below.

<style>.embed-container {position: relative; padding-bottom: 80%; height: 0; max-width: 100%;} .embed-container iframe, .embed-container object, .embed-container iframe{position: absolute; top: 0; left: 0; width: 100%; height: 100%;} small{position: absolute; z-index: 40; bottom: 0; margin-bottom: -15px;}</style><div class="embed-container"><iframe width="500" height="400" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" title="SOC 4650/5650 - Intro to GIS - Lab-09 Map 2" src="//slustl.maps.arcgis.com/apps/Embed/index.html?webmap=a37637ae0d6a4e56b69f66f1511d9aa9&extent=-126.2549,24.7202,-61.3477,53.9776&zoom=true&previewImage=false&scale=true&disable_scroll=true&theme=light"></iframe></div>

<br>

## Meeting Reminders
Please don't forget about what is due for next week, which is listed on the [syllabus](https://slu-soc5650.github.io/syllabus/module-4-map-products-with-arcgis.html). In addition to Lab-09, there are also some upcoming deadlines in April I want to remind you of: 

  * the fifth [final project waypoint](https://slu-soc5650.github.io/final-project/index.html#waypoints) is due in next week for *all students*
  * students in SOC 5650 will have a draft paper due on April 12th
  * all students will have a draft ArcGIS story map due April 26th

<br>

## Course Trajectory
Now that we have covered getting data into ArcGIS Online and creating web maps, you can start to work on this facet of your final project! There are five maps that you will need to create, which are listed [here](https://slu-soc5650.github.io/final-project/index.html#overview). More details on these maps are forthcoming!
