---
layout: default
title: Project Setup 
nav_order: 1
parent: Hands On
---

# Project Setup
    

If you haven't already, [download QGIS](https://qgis.org/en/site/forusers/download.html). Revisit the Introduction of this workshop for instructions. You should also have downloaded **and unzipped** the workshop project folder. Inside you will see the historical map (school-map.tif), schools.geojson, shoreline.geojson, and a QGIS project file called gis-georeferencing.qgz. Double click the QGIS project to open it. 

Click <a href="https://ubc-library-rc.github.io/gis-intro-qgis/content/qgis-gui.html" target="_blank">here</a> for a review of the QGIS Graphical User Interface (GUI). 


## Connect Directory 
There are many ways to connect directories (folders) and add data to a QGIS project. Adding our working folder as a “favorite” connection now will make things easier later on. In the Browser Panel, right click Favorites and select Add new directory. Navigate to your newly extracted folder called gis-georeferencing-workshop. Select it (but don’t click into it) and hit Open at the bottom right of the dialogue box. The directory gis-georeferencing-workshop is now pinned in your Browser Panel. Expand the directory by clicking the triangle and open the data folder.

## Add Target Layers from Local Directory

From directory gis-georeferencing-workshop, drag the following layers onto your map canvas to add them, or simply double click each file. 

- schools.geojson
- shoreline.geojson 

These spatial files were downloaded from vancouver open data portal. Discuss Format? 
Change symbology.... 



## Add Target Layer from Web
Street intersections. Data layer quite big and specific. need major roads. 
2 ways:
- web plugin
- xyz tiles like from  [leaflet](https://leaflet-extras.github.io/leaflet-providers/preview/) or [stadia fka stamen](https://stadiamaps.com/products/map-tiles/)

- osm  (but will it work with projection) --> from web plugin 

### Install Plugin
[QGIS plugins](https://plugins.qgis.org/) are user developed tools that extend QGIS functionality beyond the basics. To access basemaps, we'll first install the QuickMapServices plugin. Click on the **Plugin** menu at the top of your screen and select **Manage and Install Plugins...**
![Install plugin](install-plugin_20221024.png)   
   
In the dialogue box that opens, select **All** as a search category on the left and type "QuickMapServices" as one word. Install the plugin and close the dialogue box.
![quick map services](quickmapservices_20221026.png)

### Add Basemap
Now go to the **Web** menu at the top of your screen. You should see the QuickMapServices plugin. Hover over it and click "Settings" at the bottom of the menu that pops up. In the settings dialogue box go to the "More services" tab and click "Get contributed pack." Click **save** to close settings and return to the **Web** menu. This time when you hover over the QuickMapServices plugin you will see an array of basemap options. Select OpenStreetMap as your basemap. Like QGIS, [Open Street Map (OSM)](https://www.openstreetmap.org/about) is open source and user developed.   

Make sure to drag your basemap to the bottom in your Layers Panel. Remove the basemap at anytime by right clicking the layer and selecting "remove." 




