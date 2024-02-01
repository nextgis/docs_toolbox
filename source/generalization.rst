Generalization of vector data
=============================

Simplification of vector layer features to reduce data volume.

Inputs:

* A vector layer in ESRI Shape format, compressed(zip)
* import_snap - 
* iterations - 
* method - метод упрощения, один из: 'douglas', 'douglas_reduction', 'lang', 'reduction', 'reumann', 'boyle', 'sliding_averaging', 'distance_weighting', 'chaiken', 'hermite', 'snakes', 'displacement'.
* threshold - порог упрощения (вводится в метрах)
* look_ahead - 
* reduction - 
* slide - 
* angle_thresh - 
* alpha - 
* beta - 

The result of the process is a layer with simplified features (geometries).

Launch tool: https://toolbox.nextgis.com/operation/generalization

Download an example of source data and result: https://demo.nextgis.com/api/resource/4548/export?zipped=true&format=shp

View the result on an interactive map: https://demo.nextgis.com/resource/4108/display?panel=info

More on startup options: https://grasswiki.osgeo.org/wiki/V.generalize_tutorial
