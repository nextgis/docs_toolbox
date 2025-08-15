Convert lines to polygons
=========================

Each line turns into a polygon. Straight and self-intersected lines are omitted.  Multilines are exploded to multiple features.

Input: 

* Linear vector layer in GeoJSON or GeoPackage format or ESRI Shapefile in a zip archive.

Output: 

* Polygon layer;
* Linear layer with remaining self-intersecting lines.

Both files are in the same format as the input.

Launch the tool: https://toolbox.nextgis.com/t/lines2poly

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/lines2poly/lines2poly_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/lines2poly/lines2poly_outputs.zip>`_ to additionally check the results.
