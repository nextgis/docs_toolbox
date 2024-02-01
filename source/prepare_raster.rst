Prepare raster
==============

A tool that performs a per-band connection of a set of single-band rasters and crops the result using a vector mask.

Input:

* Initial raster data

The initial raster data can be presented in two forms:

1. Multi-band raster in GDAL-compatible format

2. ZIP archive with a set of single-baned GDAL-compatible rasters

* Vector layer, which is used as mask

ZIP archive with ESRI Shapefile or a other file format supported by OGR.

* “No data” value

The value that is marked as “No data”. Use the - symbol to use the default value.

* The name of the resulting raster

No file extension (e.g. ndvi, water). The extension will be automatically installed in .tif

If the input is an archive with single-band rasters, the tool first combines them into a multi-band raster. The order of the bands is determined by alphabetically sorting the names of the initial rasters in the archive. 
Then the multi-band raster (assembled from the archive or submitted immediately) is cropped with a vector mask.

The initial rasters and the vector mask can be in different coordinate systems before processing, all data is brought into a single spatial domain.

Launch tool: https://toolbox.nextgis.com/operation/prepare_raster

Download an example of initial data and calculation results: https://nextgis.ru/data/toolbox/prepare_raster/prepare_raster.zip

View the source data and calculation results on the interactive map: https://demo.nextgis.com/resource/4595/display?panel=info

.. figure:: _static/prepare_raster.png
   :align: center
   :width: 16cm

   An example of the result of the tool’s usage
