---
layout: default
title: Set Project CRS
nav_order: 2
parent: Hands On
---
# Choose Coordinate Reference System 

Setting the project CRS doesn't change the stored projection of each layer, only how they are rendered 'on the fly' by QGIS. QGIS will reproject all the project layers 'on the fly' to match the project CRS. Read the [QGIS Documentation on coordinate reference systems](https://docs.qgis.org/3.28/en/docs/gentle_gis_introduction/coordinate_reference_systems.html) or check out the Library's [workshop on projections](https://ubc-library-rc.github.io/map-projections/content/CRS.html) if you're interested in learning more. 

When choosing the CRS for your QGIS project, it's important to think about both the projection of your Source Layer and the projection of your Target Layer. Generally, you want to set project's CRS to the projection you want your map georeferenced in. The best projection will depend on many factors, including the scale and area the map covers, and what properties (size, angle, distance or direction). If your Source Layer appears to be already projected, it's useful to do some research to deduce the what projection it's in. 



<!-- other data projections - will reproject on fly to match project 
> wgs for open street map
> vancouver open data allwos you to download in wgs or nad 

This workshop focuses on the practical  -->

<!-- how important to know whether your map has projection ///what it is -- and that of your target layers (vancouver open data allwos you to download in wgs or nad --- explain these -  -- downlaod in wgs or else wont be coordinate --) - why does nad not work?   -->


<!-- Datums and Projections  -->





