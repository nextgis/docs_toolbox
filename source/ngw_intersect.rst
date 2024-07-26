Intersector
===========

The tool intersects all layers of the nextgis.com web map using the specified geometry and generates a report listing the layers, with which the intersection took place. If different features intersect in a separate layer, these cases are displayed as separate events in the report.

Inputs:

*  url - address of the used Web GIS
*  webmap_id - web map ID from used Web GIS
*  wkt - geometry with which the intersection of layers of the web map is checked. Indicated in wkt format, coordinate system - EPSG: 3857

Outputs:

*  .xlsx table with a list of intersected layers

Launch tool: https://toolbox.nextgis.com/operation/ngw-intersect
	
 

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/ngw_intersect/ngw_intersect_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/ngw_intersect/ngw_intersect_outputs.zip>`_ to additionally check the results.
