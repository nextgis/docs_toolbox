Split into equal parts
======================

Tool splits all objects of polygon layer into parts with equal area. Note: tool doesn't process multipolygons.

Inputs:

* Shapefile - polygon layer to be splitted. Should be in ESRI Shapefile format and packed in ZIP-archive.
* Number of parts - specify, into how many parts source Shapefile should be splitted.

Outputs:

* ZIP-archive with modified Shapefile, where initial polygons are splitted into specified number of parts with equal area, and each part is an individual polygon itself. 

Launch tool: https://toolbox.nextgis.com/operation/split_to_equal

View the results of calculations on an interactive map: https://demo.nextgis.com/resource/4552/display?panel=layers 
