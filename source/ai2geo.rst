Adobe Illustrator (*.ai) to geodata
===================================

The tool extracts vector data layers from an Adobe Illustrator (* .ai) file using an additional file in GeoTIFF format for georeference.

Inputs:

* An Adobe Illustrator file (with the .ai extension) that contains vector features 
* A GeoTIFF file (.geotiff or .tif extension) of PNG+PGW pair, on the basis of which the georeferencing of the extracted vector features will be performed. The same rasters should be used as a basemap in *.ai itself.

The tool works in the following way: geometries are extracted from the .ai file. For each geometry, its type (point, line or polygon) is determined, as well as the style with which it is drawn (line thickness, line color, fill color). Layers are created (according to the types of geometries) in which each feature will contain the resulting geometry and a style string in the “STYLE” field. In this case, the coordinates of the geometries are converted from local coordinates to spatial coordinates, based on the transmitted GeoTIFF file, which must contain the correct geospatial reference (it is implied, that the vector features in the .ai file were drawn “on top” of a similar image in Adobe Illustrator).

The result of the process is a ZIP archive containing a set of files in the ESRI Shapefile format according to the created layers.

Launch tool: https://toolbox.nextgis.com/operation/ai2geo

.. figure:: _static/ai2geo_before.png
   :align: center
   :width: 32cm
   
   Source vector data in .ai file

.. figure:: _static/ai2geo_after.png
   :align: center
   :width: 32cm
   
   The result of the tool’s usage: the resulting layers are loaded into QGIS and displayed on the background of the OSM basemap
