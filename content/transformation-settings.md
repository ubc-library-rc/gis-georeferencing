---
layout: default
title: Transformation Settings
nav_order: 4
parent: Hands On
---
# Transformation Settings 

**Transformation Settings** tell QGIS how to georeference the image. Open Transformation Settings by clicking the gear icon.
<br>

<img src="./images/transformation-settings_20231112.jpg" style="width:90%">

<br>
Select the following settings:    

<img src="./images/transformation-settings_20231109.png" style="width:90%">
<br>

The **Transformation type** determines how the pixels of your Source Layer are shifted so as to warp to match a projection. The **Target CRS** should be the project CRS (Coordinate Reference System) and the projection you wish to georeference your historical map in. QGIS should automatically **save the output** georeferenced image to the same folder as it currently is stored in and append "modified" to its file name. If this has not automatically occurred, save the output to the workshop folder as `vancouver-school-map-1975_modified.tif`. We'll use **nearest neighbor** as our resampling method since we don't want to assign new values to the image pixels. 

    
This workshop is focused on the workflow and technical skills to georeference a scanned historical map. If you are interested in the computational aspect of georeferencing, read this [short description by Esri](https://www.esri.com/about/newsroom/wp-content/uploads/2018/07/Understanding-Raster-Georeferencing.pdf) to understand the math behind locating image pixels in coordinate space.
{: .note}
