Adobe Illustrator (*.ai) to geodata
===================================

The tool extracts vector layers from a PDF file or Adobe Illustrator (* .ai) file.  An additional raster file could be used for georeference.

Inputs:

* PDF file or Adobe Illustrator file (with the .ai extension) which contains vector features.
* Raster file for georeferencing - GeoTIFF file (with the .geotiff or .tif extension) or ZIP-archive with PNG + PGW (world-file). Same files should be used as a base layer in PDF or AI file. This is an optional field, if you leave it blank, vector layers will be in a relative coordinate system.

Output:

* ZIP-archive with a set of ESRI Shapefile files.

Launch tool: https://toolbox.nextgis.com/operation/ai2geo

.. figure:: _static/ai2geo_before.png
   :align: center
   :width: 32cm
   
   Source vector data in .ai file

.. figure:: _static/ai2geo_after.png
   :align: center
   :width: 32cm
   
   Resulting layers are loaded into QGIS and displayed in front of the OSM basemap
