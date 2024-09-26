Split into rectangles and calculate their number
================================================

Splits polygon layer into equal rectangular parts and calculates number of rectangles. Layer can consist of several polygons, number of rectangles will be calculated for each of them. 

Inputs:

*  Shapefile - polygonal layer in ESRI Shapefile format, for which the number of rectangles will be calculated. Should be packed in ZIP-archive. Attributes should contain empty integer field, where the results of calculation will be recorded. Layer CRS must be use meters, EPSG:4326 and EPSG:3857 are not suitable.
* Length of rectangle - longer side of rectangle, should be specified in meters.
* Width of rectangle - shorter side of rectangle, should be specified in meters.
* Field name - name of the string field in initial layer, where to write the number of calculated rectangles for each polygon.
* Percentage of not filled area – please, specify percentage. Percentage is calculated out of rectangle area and will be used to form a buffer around each rectangle.

Outputs:

* ZIP-archive with modified Shapefile, with a number of rectangles recorded in attribute table. 

Launch tool: https://toolbox.nextgis.com/operation/split_to_rect
