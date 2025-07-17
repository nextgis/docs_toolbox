Prepare raster
==============

A tool that performs a per-band connection of a set of single-band rasters and crops the result using a vector mask.

Inputs:

* Input raster dataset. Input raster could be presented as 1) multiband GDAL-supported raster or 2) ZIP archive with singleband GDAL-supported rasters;
* Input vector dataset. Input vector could be presented as 1) OGR-supported single file 2) ZIP archive with ESRI Shapefile. It will be used for clipping input raster.
* Nodata value. Optional. Value that will be set as Nodata. Default is 0.
* Output dataset name. Optional. No extension (e.g. ndvi, water). Extension will be automatically set to .tif.

Outputs:

* Result raster in TIFF format.



If the input is an archive with single-band rasters, the tool first combines them into a multi-band raster. The order of the bands is determined by alphabetically sorting the names of the initial rasters in the archive. 
Then the multi-band raster (assembled from the archive or submitted immediately) is cropped with a vector mask.

The initial rasters and the vector mask can be in different coordinate systems before processing, all data is brought into a single spatial domain.

Launch tool: https://toolbox.nextgis.com/t/prepare_raster


**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/prepare_raster/prepare_raster_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/prepare_raster/prepare_raster_outputs.zip>`_ to additionally check the results.
