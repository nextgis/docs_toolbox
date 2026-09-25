Convert raster with ESRI AUX XML to GeoTIFF
===========================================

Fixes problem with georeferencing in the JPEG-rasters with ESRI AUX XML. Such rasters might be incorrectly referenced in QGIS and other GDAL-based tools.

Inputs:

* Input raster - GDAL-compatible raster with AUX XML in a ZIP file.
* CRS - Optional. proj string for coordinate system. If not set, CRS is defined from AUX XML.

Outputs:

* GeoTIFF file.

Launch the tool: https://toolbox.nextgis.com/t/esriauxxml2geotiff

.. admonition:: Related tools

   * `MapInfo to QGIS <https://toolbox.nextgis.com/t/mapinfo2qgis?from-related-tools=1>`_
   * `Convert vector layer <https://toolbox.nextgis.com/t/convert?from-related-tools=1>`_

