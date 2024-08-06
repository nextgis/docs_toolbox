Convert lines to polygons
=========================

Each line turns into a polygon. Straight and self-intersected lines are omitted.  Multilines are exploded to multiple features.

* Input: linear vector layer in geojson or geopackage format or ESRI Shapefile in a zip archive.
* Output: polygon layer in geojson or geopackage format, linear layer with remaining self-intersecting lines

Launch tool: https://toolbox.nextgis.com/operation/lines2poly

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/lines2poly/lines2poly_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/lines2poly/lines2poly_outputs.zip>`_ to additionally check the results.
