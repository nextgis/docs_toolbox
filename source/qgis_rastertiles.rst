Generate raster tiles from QGIS project
==========================================

Generate zipped raster tiles from an archive with QGIS project and data. 

Inputs:

* ZIP file containing QGIS project and data files;
* Extent. If empty, a combined extent of all layers will be used. It may unexpectedly calculate an extent of the entire planet, then the tool will take a lot of time to process. Options to set the extent are: 1) upload a file with polygons - it's handy if you need tiles for a complex area, along a coastline, for example, 2) mark it on a map, 3) draw it on the map and then correct the numbers or 4) enter the extent manually following the format 'xmin, xmax, ymin, ymax'. Enter coordinates in WGS 84 (EPSG:4326), for example ``-7.3,42.1,10.5,50.5``;
* Min zoom level - between 0 and 25, the default value is 0;
* Max zoom level - between 0 and 25, the default value is 9;
* Tile image format - if not specified generates PNG tiles. You can also enter ``JPG``;
* Background color in RGBA, if not specified, 0,0,0,0 (transparent) will apply;
* DPI - image resolution in dots per inch, between 48 and 600, the default value is 96;
* Metatile size - between 1 and 20, the default value is 4;
* JPEG quality - the level of image compression between 1 (more compression, low quality) and 100 (max quality), the default is moderately compressed, 75;
* Tile height in pixels, if not specified, 255 will apply;
* Tile width in pixels, if not specified, 255 will apply.

Output:

* ZIP archive with tile images organized into folders.

Launch the tool: https://toolbox.nextgis.com/t/qgis_rastertiles

.. figure:: _static/qgis_rastertiles_input.png
   :name: qgis_rastertiles_input_pic
   :align: center
   :width: 16cm

   Example polygons with complicated geometry used to calculate the extent

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/qgis_rastertiles/qgis_rastertiles_inputs.zip>`_ to test the tool. Step-by-step instructions included.

`Result example <https://nextgis.ru/data/toolbox/qgis_rastertiles/qgis_rastertiles_outputs.zip>`_ of the tool run.

