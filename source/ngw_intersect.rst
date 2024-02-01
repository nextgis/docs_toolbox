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

Usage example:

How many types of anemones can you find on the Appalachian Trail?

*  url - https://demo.nextgis.com
*  webmap_id - 4714 (since the web map address is https://demo.nextgis.com/resource/4714/display)
*  wkt - LineString (-9378421.57282677479088306 4115819.42546373652294278, -7678593.31173497438430786 5764332.11640937067568302)	
 
.. figure:: _static/ngw_intersect_layers.png
   :align: center
   :width: 16cm
   
   Initial Data Example
   
.. figure:: _static/ngw_intersect_result.png
   :align: center
   :width: 16cm
   
   An example of the result of the tool’s usage 
