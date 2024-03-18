layout:true

<div class="header">
  
  <p class="header-text">QGIS for Working Professionals</p>
</div>
<div class="footer">
  <p class="footer-text">
    <img src="images/datapolitan-logo-01.svg" class="logo_new">
    <span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">
      <img alt="Creative-Commons-License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" />
      </p>
</div>

--

class: center,middle

![img-center-50](images/datapolitan-logo-01.svg)

# QGIS for Working Professionals

- - -

## Facilitator: Richard Dunks

### Follow along at: 

#### See the code at: 

<p class="license-text"><strong><strong>QGIS for Working Professionals</strong></strong> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://www.datapolitan.com" property="cc:attributionName" rel="cc:attributionURL">Richard Dunks</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a></p>

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img style="border-width:0;width:8%" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a>

---

class:center,middle
# Welcome!

---

# A Few Ground Rules
???
+ Facilitators establish the intention we have for the culture of the classroom

--

+ Be present (phone, email, social media, etc.)
--

+ Be curious and ask questions
--

+ Step up, step back
--

+ One mic
--

+ Respect multiple perspectives 
--

+ Assume noble regard and positive intent


---

# Introductions
In pairs, please share with your partner:
+ Your name
+ What you do
+ Your level of comfort with QGIS (1 - 10)
+ What you hope to get from class this week

You'll be introducing your partner to the class (so take notes)

---

# Assumptions
--

+ You're all busy
--

+ You're all mostly self-taught
--

+ You're all motivated to learn how to better use QGIS
--

+ You all know your data better than I could (and might want to take a break from it)

---
class:center,middle

# How We're Going to Do This

---

# How I Teach
--

+ Minimal lecture
--

+ Demonstrate a concept/technique with open data
--

+ Learn by doing -> You'll be sharing your screen more than me
--

+ I ask a lot of you but I will help out along the way
--

+ I leave no one behind
--

[![img-center-50](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExMzJ0c2dnbHZtdjFhOG4wZ3RwN3RmaDM1bjAwZ2dob2kydnV6bWViZyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/XZOLVxfNcPuVAKOQ6l/giphy.gif)](https://giphy.com/gifs/tlc-network-tlc-90-day-fiance-the-other-way-XZOLVxfNcPuVAKOQ6l)

---
# How our Days Are Going to Go
--

+ 2 85-minute sessions
--

+ 10-minute break in between
--

+ "Your Turn" -> Practice exercise towards end of each block
--

+ "Peer Mapping" -> Work in pairs with one person driving
--

+ "Homework" -> A 10-15 minute task to demo the next day
--

+ 1-hour open lab after our session is over for questions and additional help

---

# How the Week is going to look
--

+ .orange[Monday] - Introduction to QGIS, loading data, filtering, and selecting
--

+ .orange[Tuesday] - Projections, buffering features, spatial joins
--

+ .orange[Wednesday] - Creating and editing features, validating geometries
--

+ .orange[Thursday] - Georeferencing and a "Bonus" section

---

# Outcomes
--

At the end of this week, you will:
--

+ Understand foundational GIS concepts
--

+ Understand the purpose and functionality of a GIS
--

+ Be practiced using QGIS for a variety of spatial operations
--

+ Demonstrate proficiency in applying GIS concepts to real-world problems
--

+ Be familiar with key resources for further information on using QGIS

---

# Keep in Mind
--

+ We're going to start simple but will move quickly forward
--

+ I'll make sure it's interesting no matter your skill level
--

+ This is also an opportunity to help your colleagues

---

# Topics for Today
--

+ Basic operations in QGIS (loading, styling, filtering, and exporting data)
--

+ Essential GIS definitions and concepts
--

+ Pro-tips for working with QGIS

---

# Let's Get Started

![img-center-65](images/dallas_cd_map.png)

## [Download this data](data/dallas_council_districts.zip) and [unzip the file](https://www.filecenter.com/blog/how-to-unzip-files-mac-iphone-android-windows/)

???
Image of map we're going to create

---

# Let's Get Started
![img-center-100](images/qgis-blank.png)

---

# Adding Data
![img-center-90](images/qgis_add_vector_layer.png)
???
1. Add Dallas Council districts

---

# Adding Data
--

+ Navigate to where you unzipped the file
--

+ Select the `.shp` file

![img-center-50](images/add_vector_dallas_cd.png)
--

+ Select .orange[**Open**]

---

# Adding Data
![img-center-75](images/add_vector_dallas_cd2.png)
--

+ Select .orange[**Add**] to add the data
--

+ Select .orange[**Close**]

---

# Adding Data
![img-center-90](images/qgis-cd-1.png)

---

# Attribute Table
![img-center-90](images/qgis-cd-2.png)

---

# Attribute Table
![img-center-95](images/qgis-cd-3.png)

---

# Attribute Table
+ Each feature has a corresponding row in the attribute table
--

+ When a feature is selected on the map, that row is selected in the attribute table
--

+ Features can be used to style the data

---

# Styling Features
--

+ Right click the layer and select .orange[**Properties**]

![img-center-75](images/qgis-cd-4.png)

---

# Styling Features
+ In the Layer Properties window, click the .orange[**Symbology**] tab
--

+ Click the .orange[**Single Symbol**] and select .orange[**Categorized**] from the drop-down menu
--


![img-center-85](images/qgis-cd-5.png)

---

# Styling Features
+ In the .orange[**Value**] field, select the column that has the data you want to style
--

+ In our case, this is the .orange[**district**] column
--


![img-center-75](images/qgis-cd-6_rev3.png)

---

# Styling Features
+ Then click .orange[**Classify**] (bottom left)
--


![img-center-65](images/qgis-cd-7_rev_box.png)
--

+ This should give each unique value in the column its own color

---

# Styling Features
+ Click .orange[**OK**] (or .orange[**Apply**] to preview)

![img-center-85](images/qgis-cd-8_rev.png)

---
exclude:true
class:center,middle
# Let's See What You Have

---

# Add labels to data
--

+ In the Layer Properties window click the .orange[**Labels**] tab
--

+ Select .orange[**Single labels**]

![img-center-95](images/qgis-cd-9.png)

---

# Add labels to data
--

+ Select the column that has the data you want to use for labels ("council")
--

+ Style the text however you want
--


![img-center-80](images/qgis-cd-10.png)

---

# Add labels to data
![img-center-90](images/qgis-cd-11.png)

---

class: center, middle
# What is our Map missing?

![img-center-85](images/dallas_cd_map.png)

---

exclude:true
# Base Maps
![img-center-60](images/gis-layers.jpg)
####Image Source: [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Visual_Representation_of_Themes_in_a_GIS.jpg)

---
exclude:true
# Base Maps
![img-center-70](images/disd_elementary.png)

---

# Base Maps

+ Give maps context (roads, topographical features, landmarks, etc.)
--

+ In QGIS, you need a plugin to use base maps
--

+ There are <a href="https://plugins.qgis.org/plugins/tags/basemap/?sort=-downloads" target=_blank>several</a>, but we're only going to use the most popular

---

# Loading Base Maps in QGIS
+ From the Plugins menu, select .orange[**Manage and Install Plugins**]

![img-center-90](images/qgis-plugins-0.png)

---

# Loading Base Maps in QGIS

+ Search for the .orange[QuickMapServices plugin] and install it

![img-center-90](images/qgis-plugins-1.png)

---

# Setting Up QuickMapServices
+ Go to the .orange[Settings] menu
![img-center-80](images/qgis-qms-0.png)

---

# Setting Up QuickMapServices

+ Get the contributed packs

![img-center-70](images/qgis-qms-1.png)

---

# Setting Up QuickMapServices

+ Revel in all the beautiful base maps

![img-left-45](https://media.giphy.com/media/3og0IuE1EjI5ZQzr3i/giphy.gif)
![img-center-45](images/qgis-qms-2.png)

---
exclude:true
class:center,middle
# Raise Your Hand When You Have All the Basemaps

---

# Loading Base Maps in QGIS
+ Take a moment and select the base map you want to use

![img-center-100](images/qgis-qms-3.png)

---

# Loading Base Maps in QGIS
![img-center-90](images/qgis-cd-basemap.PNG)

---

# QGIS Pro-tip
--

![img-right-40](images/qgis-project-save.png)
+ Save your project
--

+ .red[QGIS doesn't autosave]
--

+ .red[You will lose work when it crashes]
--


![img-left-50](https://media.giphy.com/media/obbIystETz0Xu/giphy.gif)


---

# Your Turn
Working with a peer, come up with a basic map with one data layer.
--

+ Think about styling and labeling
--

+ Be ready to show the group
--

+ Feel free to get creative with what you show

---

name: a-block-end
class:center,middle

# Wrap-up

---
class:center
# 10-Minute Break
![img-center-50](images/sadtopographies/unfortunate_cove.png)

#### Source: https://www.instagram.com/p/BmSmGcxhGGT/

---
name: b-block-start
class:center, middle

# Welcome Back

---

class:center,middle
# What did we just do?

---

class:center,middle
# Some Basic Concepts

---

# Geographic Info System (GIS)
--

> Any system for capturing, storing, checking, and displaying data related to positions on the Earth's surface

### [National Geographic Education Encyclopedia](https://www.nationalgeographic.org/encyclopedia/geographic-information-system-gis/)

---

# Or more simply

> In a GIS, you connect _**data**_ with _**geography**_.

### [GISgeography.com](http://gisgeography.com/what-gis-geographic-information-systems/)

---

# Geographic Info Systems (GIS)
--

+ Create interactive queries (user-created searches)
--

+ Analyze spatial information
--

+ Edit data in maps
--

+ Present the results of all these operations

---

class:center,middle
# Some More Key Concepts

---

# Basic Map Using QGIS
![img-center-75](images/disd_elementary.png)

---

# Points  
[![img-left-30](images/point_feature.png)](http://docs.qgis.org/2.8/en/docs/gentle_gis_introduction/vector_data.html#overview)

--

![img-right-70](images/disd_elementary.png)

---

# Lines
[![img-left-30](images/polyline_feature.png)](http://docs.qgis.org/2.8/en/docs/gentle_gis_introduction/vector_data.html#overview)

--

![img-right-70](images/disd_elementary.png)

---

# Polygons
[![img-left-30](images/polygon_feature.png)](http://docs.qgis.org/2.8/en/docs/gentle_gis_introduction/vector_data.html#overview)

--

![img-right-70](images/disd_elementary.png)

---

# Shapefiles
--
        
+ Basic file for storing map elements
--

+ Stores spatial data, like points, lines, and polygons
--

+ Multiple files comprise a "shapefile"

--

![img-center-75](images/dallas_cd_file_structure.png)

---

# Shapefiles

![img-center-75](images/dallas_cd_file_structure.png)
--

+ .orange[.shp]—The main file that stores the feature geometry
--

+ .orange[.dbf]—The dBASE table that stores the attribute information of features

---

# Shapefiles

![img-center-75](images/dallas_cd_file_structure.png)

+ .orange[.prj]—The file that stores the coordinate system information
--

+ .orange[.shx]—The index file that stores the index of the feature geometry

---

# You might also see
--

+ .orange[.cpg]—Identifies the character set to be used
--

+ .orange[.sbn] and .orange[.sbx]—The files that store the spatial index of the features

---

# Shapefiles

+ Have a few limitations
--

+ One geometry type (Point, Line, Polygon) per shapefile
--

+ So sometimes you end up with this:
![img-center-65](images/file_struct2.png)

---

# Shapefiles
--

+ Column names can only be letters, numbers, and underscores "_"
--

+ Column names can only be ten characters long

--

![img-center-100](images/shapefile-column-names.png)

---

# Other File Formats
--

+ CSV files
--

+ GeoJSON
--

+ GeoTIFF/GeoPDF
--

+ Spatial database

---

class:center,middle
# Let's add another layer

---

# What is a CSV file?
--

![img](images/csv1.png)

---

# What is a CSV file?
![img-center-90](images/csv2.png)

---

# Dallas 311 Service Requests
+ [Download the data](data/20240101_20240229_dallas_311.csv) to your desktop

![img-center-70](images/dallas_cd_311_basemap.png)

---

# Adding CSV Data
![img-center-60](images/add_csv1.png)

---

![img-center-60](images/add_csv2_box.png)

--


![img-center-60](images/dallas_311_add_csv.png)

---

# Adding CSV Data
+ Make sure it found the .orange[latitude] and .orange[longitude] fields

![img-center-75](images/dallas_311_add_csv4_box.png)

---

# Adding CSV Data
![img-center-85](images/dallas_cd_311_basemap.png)

---

# Layers
![img-center-60](images/gis-layers.jpg)
#### Image Source: [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Visual_Representation_of_Themes_in_a_GIS.jpg)

---

# Layer Ordering
--

+ Layers on top are drawn on top
--

+ Just drag and drop within the Layers Panel to change order
--

+ Try it now

---

# Filter and Query
+ We can filter the points based on the values in the attribute table

![img-center-90](images/dallas_311_attribute_table.png)


---

# Filter and Query
+ Right-click on the layer and select .orange[Filter] to open the Query Builder

![img-left-40](images/dallas_311_filter1.png)
--
![img-right-50](images/dallas_311_filter2.png)


---

# Filter and Query
+ Filter using the .orange[Service Request Type] field
+ Select .orange[All] under .orange[Values]

![img-left-48](images/dallas_311_filter3a_box.png)
![img-right-48](images/dallas_311_filter3b.png)


---

# Filter and Query
![img-left-60](images/dallas_311_filter4.png)
--
![img-right-35](images/dallas_311_filter5.png)

---

# Filter and Query
![img-center-60](images/dallas_311_filter6.png)

---

# Filter and Query
![img-center-80](images/dallas_311_filter7.png)

---

class:center,middle
# We can also filter by multiple conditions

---

# Multiple Conditions
![img-left-60](images/dallas_311_filter8_box.png)
--
![img-right-35](images/dallas_311_filter9.png)

---

# Multiple Conditions
![img-center-80](images/dallas_311_filter10.png)

---

# Select by Feature
--

+ Sometimes we don't want to filter, but just select based on attributes
--

+ We do this in the .orange[Attribute Table] (right click the layer and open)
--

+ Click on the icon in the top left with the backward 3
--


![img-center-100](images/dallas_311_sbf1_box.png)

???
(select noise complaints)

---

# Select by Feature
--

+ This will allow you to select by expression
--

+ Select the .orange[Fields and Values]
--

+ Select .orange[Service Request Type]
--

![img-left-48](images/dallas_311_sbf2_box.png)
![img-right-48](images/dallas_311_sbf3_box.png)

---

# Select by Feature
--

+ Add an .orange[=] sign to the expression
--

+ Filter the values for .orange[Noise]
--

+ Select .orange[Chronic Noise Complaint - DPD]
--

![img-left-48](images/dallas_311_sbf4.png)
![img-right-48](images/dallas_311_sbf5b.png)

--


![img-center-50](images/dallas_311_sbf6.png)

---

# Select by Feature
--

+ Click .orange[Select Features]
--

+ Check the top Attribute Table for the filtered row count
![img-center-100](images/dallas_311_sbf7_box.png)
--

+ Filter to .orange[Show Selected Features]
![img-center-60](images/dallas_311_sbf8.png)

---

# Select by Feature
+ The yellow dots are the selected features

![img-center-75](images/dallas_311_sbf10.png)


---
# Select by Location
--

+ Sometimes we want to select based on where the feature is on the map
--

+ This helps when the spatial location isn't an attribute
--

+ It also helps verify the attribute is accurate
--

+ Let's practice this

---

# Select by Location
--

+ Select a council district from the .orange[Councils] layer
--

+ Go to .orange[Vector] -> .orange[Research Tools] -> .orange[Select by Location]

![img-center-50](images/dallas_311_sbl1.png)
???
(select complaints in district)

---
# Select by Location
+ Add the parameters for the select
![img-center-100](images/dallas_311_sbl2_box.png)

---
# Select by Location
+ Turns out the feature isn't accurate

![img-center-100](images/dallas_311_sbl3_box.png)

---

# Exporting Data
--

+ Once we have a selection that we like, we can export it as it's own layer
--

+ Right-click on the layer
--

+ Select .orange[Export] -> .orange[Save Selected Features As...]
![img-center-50](images/dallas_311_export1.png)

---

# Exporting Data
--

+ Name the file and click .orange[OK]
--


![img-center-50](images/dallas_311_export2.png)


---
class:center,middle

# Some other useful functions

---

# Zoom to Layer
![img-center-60](images/dallas_311_ztl1.png)

---

# Zoom Selection
--

+ Select the zoom on the toolbar
--

![img-right-30](images/zoom_box.png)
--

+ Draw a box around the area you want to zoom into
--

+ Click the icon to return to the previous map extent
--

![img-right-30](images/extent_box.png)

---

# Pan Map
+ Select the hand tool to pan around the map

![img-center-30](images/hand.png)


---

# Toolbars
![img-right-30](images/qgis_toolbars.png)
--

+ Set of quick icons you can place on your window
--

+ You can adjust which ones are visible and where they are
--

+ They are great if you like to work using icons

---

# Panels
![img-right-30](images/qgis_panels.png)
--

+ Panels are panes to your desktop window
--

+ Good for quickly accessing information
--

+ Depends on how cluttered you want your window to be
--

+ [See the documentation](https://docs.qgis.org/2.18/en/docs/user_manual/introduction/qgis_gui.html#panels) for more information


---

# Your Turn
--

+ Working in your pairs, select a dataset (maybe `active rigs`)
--

+ Select points by both feature and location
--

+ See if they agree or if there's a discrepancy

---

# Homework
--

+ Create and style a basic map with data from the database
--

+ Play around with the styles and labels
--

+ Have fun and explore features
--

+ You can show the live map or export it to a PNG to demo

---
class:center,middle
# Wrap-up

---

# Looking Ahead
--

+ Projections and why they're important
--

+ Buffering and selecting features
--

+ Spatial joins


---
name: b-block-end
class: center, middle

# Thank you!

---
class:center,middle

# Lab Time 


