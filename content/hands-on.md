---
layout: default
title: Hands On
nav_order: 7
has_children: true
---

# Hands On

In this section you will georeference a historical map of Vancouver schools (1975) with QGIS. The map is one from UBC's physical map collection, located on Level 2 of Koerner Library. A high quality scan has already been made for you. This will be your **Source Layer**. You will also need a **Target Layer**, a geospatial data layer which will serve as reference for assigning locative information to the Source Layer. The Target Layer for this workshop will be a web map of Vancouver displaying city streets. You will also be provided with a spatial file of Vancouver's shoreline and a dataset of Vancouver schools (2023) from the city's [Open Data Portal](https://opendata.vancouver.ca/explore/dataset/schools/map/?location=12,49.25526,-123.11228). 
<br>    
Download **and unzip** the workshop project folder now.
    
[Download Data](gis-georeferencing-workshop.zip){: .btn .btn-purple }


## Workflow Overview
When georeferencing within a Geographic Information System (GIS) like QGIS, the basic workflow is as follows

1. Load your Target Layer into GIS 
2. Set the Coordinate Reference System (CRS) of your project
3. Load your Source Layer as a high resolution image (filetype .tif) 
4. Match a handful of points on the Source Layer to those on the Target Layer, thus appending locative information to the Source Layer 
5. Assess error; Adjust; Save georeferenced image

The points matched between the two layers are called **Ground Control Points (GCPs)**. When choosing a map to georeference (Source Layer) and geospatial reference layer(s) (Target Layer), it is important to ensure there are clear GCPs. GCPs may be physical geographic features, such as river bends, coastlines, or lake boundaries. GCPs may be infrastructural features such as the intersection of two roads or political boundaries or meridian lines. In any case, it is important to consider whether the geographic location of a potential GCP may have changed in the time since the historical map was rendered. These changes will matter more or less depending on the scale of the Source Layer. Most likely, your GCPs will be mix of features.
<!-- For instance, if the goal is to georeference a map of lower British Columbia, the exact bends of the Fraser River are less important than it's general location. The Fraser River could therefore be used as a reference to match the Source to Target Layer.  -->





