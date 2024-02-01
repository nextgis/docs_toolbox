Generate tileset from raster
============================

Service generates raster tiles (NGM format) from input gdal-supported raster.

Inputs:

*  Palette file - TXT file  with color scheme of each raster values  located in a separate line. Order: Value Red Green Blue Opacity. For example, for a value of 23, assigning a completely opaque lilac color looks like this: 23 200 162 200 255. Opacity ranges from 0 to 255, 0 - completely transparent, 255 - completely opaque.  Use an empty text file to keep the original palette (for single-band with palette) and for RGB / RGBA rasters.
*  Raster dataset - RGB, RGBA, single-band gray or single-band with palette GDAL-compatible raster
*  Tiles name - the name that will be used for the file name and for the layer in NGM
*  Zoom levels - the levels at which the tiles will be displayed. This refers to `standard zoom levels <https://wiki.openstreetmap.org/wiki/Zoom_levels>`_, for example, as for OSM maps. Possible input values: a number indicating one level, for example, 10; a range of levels, for example, 8-14; hyphen - for auto-selection of levels

Outputs:

*  NGRC file with tileset

.. figure:: _static/raster2tiles_input.png
   :align: center
   :width: 16cm
   
   Inputs example
   
.. figure:: _static/raster2tiles_output.png
   :align: center
   :width: 8cm
   
   Result example - NGRC file added to NextGIS Mobile

Launch tool: https://toolbox.nextgis.com/operation/raster2tiles

Download an example of source data and result :download:`here <files/raster2tiles_examples.zip>`.  
