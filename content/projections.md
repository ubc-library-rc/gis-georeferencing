---
layout: default
title: Set Project CRS
nav_order: 2
parent: Hands On
---
# Choose Coordinate Reference System 

Setting the project CRS doesn't change the stored projection of each layer, only how they are rendered 'on the fly' by QGIS. QGIS will reproject all the project layers 'on the fly' to match the project CRS. Read the [QGIS Documentation on coordinate reference systems](https://docs.qgis.org/3.28/en/docs/gentle_gis_introduction/coordinate_reference_systems.html) or check out the Library's [workshop on projections](https://ubc-library-rc.github.io/map-projections/content/CRS.html) if you're interested in learning more. 

When choosing the CRS for your QGIS project, it's important to think about both the projection of your Source Layer and the projection of your Target Layer. Generally, you want to set project's CRS to the projection you want your map georeferenced in. The best projection will depend on many factors, including the scale and area the map covers, and what properties (size, angle, distance or direction). If your Source Layer appears to be already projected, it's useful to do some research to deduce the what projection it's in. 

## Datums and Projections 
move cursor around, look at status bar. decimal degrees and meters - distance. Geographic coordinate system and projected coordinate system/ Datum and Projection. Projection - 3d to 2d. after Datum - Ellipsoid approximation. 
    
INCLUDE DIAGRAM
    
CRS includes information on both the GCS and PCS - though PCS is not nec to visualize in GIS. 

Common datums are NAD 83 or WGS 84 - numbers represent years surveys completed. However, the historical map we're georeferencing today was made in 1975, before either of those datums. It looks already projected so I'm guessing it was NAD 27, the north american datum in 27. UTM - projection - universal transverse mercator, zone 10N - most accurate shape (?) wise for the sliver right over vancouver. As you will see, choosing the most likely CRS now will make georeferencing a lot more seamless later on. 

<!--vancouver open data allows you to download in wgs or nad; download in wgs or else wont be coordinate-->


## Set Project CRS

We'll set the project CRS to --- or ESPG

To do this...


Notice what happens on map canvas. 


