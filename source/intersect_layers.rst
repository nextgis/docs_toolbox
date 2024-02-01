Intersect layers
================

The tool intersects a polygonal layer with another vector layer (any type of geometry) and outputs the result as a set of CSV files.

Inputs:

*  Field name for CSV file. The name of the attribute column in the polygonal layer for resulting CSV files. If this field is blank, CSV file names will be generated automatically.
*  Polygonal shapefile. Polygonal layer in the ESRI Shapefile format (ZIP-archive), for the objects of which the fact of intersection (or non-intersection) with objects from another layer is defined.
*  Shapefile with intersecting layer. The vector layer with any geometries in the ESRI Shapefile format (ZIP-archive), containing objects intersecting with objects from the polygonal layer. The layer must be in the same coordinate system as the polygon layer.

Outputs:

*  Zipped CSV files, each of which describes one of the objects of the polygonal layer. If an object from a polygon layer has an intersection with an object from another layer, the CSV file will contain the coordinates of the center and the WKT description of the polygon.

Launch tool: https://toolbox.nextgis.com/operation/intersect_layers

Download an example of source data and result :download:`here <files/intersect_layer_example.zip>`.
