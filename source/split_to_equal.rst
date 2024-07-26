Split into equal parts
======================

Tool splits all objects of polygon layer into parts with equal area. Note: tool doesn't process multipolygons.

Inputs:

* Shapefile - polygon layer to be splitted. Should be in ESRI Shapefile format and packed in ZIP-archive.
* Number of parts - specify, into how many parts source Shapefile should be splitted.

Outputs:

* ZIP-archive with modified Shapefile, where initial polygons are splitted into specified number of parts with equal area, and each part is an individual polygon itself. 

Launch tool: https://toolbox.nextgis.com/operation/split_to_equal


**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/split_to_equal/split_to_equal_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/split_to_equal/split_to_equal_outputs.zip>`_ to additionally check the results.
