---
layout: default
title: Add GCPs 
nav_order: 5
parent: Hands On
---

# Begin Georeferencing! 


<br>
You are now ready to begin georeferencing by adding Ground Control Points (GCPs). <br>
Click the **Add Point** icon in the Georeferencer Window to get started.
    
<img src="./images/add-point_20231112.jpg" style="width:90%">

<br>     
Choose your first GCP on the historical map. Once you select a GCP on Source Layer from the Georeferencer window, a dialogue box will open prompting you to Enter Map Coordinates on the Target Layer. Choose to do this from **From Map Canvas**. The QGIS Map Canvas will come to the forefront of your screen and your cursor will turn into a crosshair. Click the corresponding GCP on the Map Canvas.
    
<br>
<img src="./images/from-map-canvas_20231112.jpg" style="width:90%">

   

If you need to zoom or pan on the Map Canvas, you will have to re-click "From Map Canvas" from the Enter Map Coordinates dialogue box. If the dialogue box is no longer visible, it's likely hiding behind your current window. 
{: .note}


<br>
Once you have have matched a GCP on the Target Layer, the Georeferencer Window will jump back to the forefront. If you are content with your selection, click OK. 

<img src="./images/coordinates-entered_20231112.jpg" style="width:100%">

<br>
You should now see your first point added to the GCP table in the Georeferencer Window. 

<img src="./images/first-GCP-pair_20231112.jpg" style="width:100%">


----

Continue adding GCPs. For this historical map, I recommend primarily using street intersections as GCPS. Begin around the periphery and then add some along major crossroads towards the center of Vancouver. Below is a sample set of 33 GCPs. If well placed, this should be plenty to georeference this map. 


<img src="./images/sample-GCP-points-source_20231112.jpg" style="width:100%">
<img src="./images/sample-GCP-points-target_20231112.jpg" style="width:100%">

You can find this set of sample GCPs in the workshop folder  or download [here](). From the Georeferencer Window, you can choose to upload a set of GCPs from the menu. 
{: .note}

You can always remove a GCP and re-place it, or move an existing GCP around.
<img src="./images/delete-point_20231112.jpg" style="width:100%">

<br>
I also recommend anchoring the shoreline by adding GCPs on either side of the three bridges. 

<img src="./images/bridge-points_20231112.jpg" style="width:100%">


## Assessing Error 

What are those red lines? 

Residual (pixels) 
warp

dont worry about them too much







