---
layout: default
title: Set Project CRS
nav_order: 9
parent: Hands On
---

# Coordinate Reference Systems (CRS)

Making Cartesian maps requires some method for flattening out the earth so we can represent portions of it on our 2-dimensional computer screens. A **Coordinate Reference System (CRS)** defines this transformation. A CRS contains two components: a **datum** and a **coordinate system**. 

## Datums
Earth is not a perfect sphere but rather a *spheroid* as it is flattened slightly at the poles. *Ellipsoid*, referencing a 3-dimensional ellipse, describes the same shape. [From Esri's description:](https://desktop.arcgis.com/en/arcmap/latest/map/projections/datums.htm) "While a spheroid approximates the shape of the earth, a datum defines the position of the spheroid relative to the center of the earth. A datum provides a frame of reference for measuring locations on the surface of the earth. It defines the origin and orientation of latitude and longitude lines." A **geocentric datum** positions the center of the spheroid, aka ellipsoid, at the earth's center of mass. A **local datum** "aligns its spheroid to closely fit the earth's surface in a particular area." Datums are developed using satellite data.

A geocentric datums is useful when a map is meant to show the whole earth, such as a World Map or Open Street Maps' web map. Local datums are useful when the area of interest is confined to a continent such as North America or a single country. Because local datums are accurate precisely for the area of their ellipsoid's best fit, it would be unwise to use a local datum for a global map, or a datum specific to North America for Africa. Datums are named by their extent and survey year. Today, the most common geocentric datum is WGS 84 (World Geodetic System 1984), and the most common local datum for the United States and Canada is NAD 83 (North American Datum 1983). Notice that Vancouver Open Data allows you to download data in either NAD 83 or WGS 84. The data for this project has been downloaded in WGS 84 so as to align with Open Street Maps' datum. 

## Coordinate Systems
A coordinate system is the math governing the projection of points on an ellipsoid to a 2-dimensional plane. A coordinate system is either a **Projected Coordinate system (PCS)** or **Geographic Coordinate system (GCS)**. Move your cursor around on your map canvas and look at the status bar. You should see coordinate pairs. You may also have noticed your map looks a bit squashed or slanted:

<img src="./images/GCS-example.png" style="height:50%;">


These two ques tell us that our project is in a GCS because geographic coordinate systems plot points in decimal degrees, whereas the unit for projected coordinate systems is meters. If you are interested in any sort of distance or area measurement, you'll want to ensure your project has a defined PCS. 


## Set Project CRS
Setting the project CRS doesn't change the stored projection of each layer, only how they are rendered 'on the fly' by QGIS. QGIS will reproject all the project layers 'on the fly' to match the project CRS. Read the [QGIS Documentation on coordinate reference systems](https://docs.qgis.org/3.28/en/docs/gentle_gis_introduction/coordinate_reference_systems.html) or check out the Library's [workshop on projections](https://ubc-library-rc.github.io/map-projections/content/CRS.html) if you're interested in learning more. Another great reasource is [pbcgis.com/projection_fundamentals/](https://www.pbcgis.com/projection_fundamentals/).

When choosing the CRS for your QGIS project, it's important to think about both the projection of your Source Layer and the projection of your Target Layer. Generally, you want to set project's CRS to the projection you want your map georeferenced in. The best projection will depend on many factors, including the scale and area the map covers, and what properties (size, angle, distance or direction). If your Source Layer appears to be already projected, it's useful to do some research to deduce the what projection it's in. From the **Project** Menu at the top of your screen, go to **Properties** and then **CRS**. Notice that as we suspected, the project is using the datum WGS 84, and has no projected coordinate system.   

To Do 
{: .label .label-green}
Set your project projection to `NAD 27 / UTM zone 10N`. Notice the map become less slanted and the status bar units change from decimal degrees to meters. 

<!-- <img src="./images/project-properties_20240104.png" style="width:100%"> -->


<img src="./images/Nad27UTMzone10N_20240104.png" style="width:100%">


**NAD 27** refers to the North American Datum created in 1927. We won't use NAD 83 because since it was created *after* our historical map, it couldn't have been used by the original cartographer as reference. **UTM** stands for Universal Transverse Mercator, a commonly used projection. Mercator projections distort size but preserve angles and shapes. To further reduce distortion we will choose zone 10N, which is the UTM zone specific to our area of interest.

Note that you can set the CRS for your georeferenced layer independently of the CRS you choose for your project. In cases where the georeferenced image covers but one small area of your entire map, you might choose to do so. However, because our focus is on Vancouver, we can set the project CRS to what we want our map georeferenced in, saving us a step down the line.

Remember to save your project before continuing.







