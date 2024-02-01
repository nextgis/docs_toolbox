Normalized difference index
===========================

The tool calculates the normalized difference index for any two input images.

Inputs:

* First component of the difference index

Any GDAL-compatible raster

* Second component of the difference index

Any GDAL-compatible raster

Outputs:

* A raster with normalized difference index in GeoTiff format

The calculation is carried out according to the formula: (First image - Second image) / (First image + Second image). The pixel values of the resulting raster are in the range from -1 to 1
Before the calculation, both images are brought into a single spatial domain. The projection and spatial resolution of the first raster is used.

Examples of common normalized difference indices:

* NDVI - for vegetation assessment (the first raster - NIR, the second - RED) For Landsat 8 data: 5 and 4 bands.
* NDWI - for the detection of water bodies (the first raster - NIR, the second - SWIR). For Landsat 8 data: 5 and 6 bands.
* NDSI - for assessing the snow cover (the first raster - GREEN, the second - SWIR). For Landsat 8 data: 3 and 6 bands.

Launch tool: https://toolbox.nextgis.com/operation/ndi

Download an example of source data and calculation results: https://nextgis.ru/data/toolbox/ndi/ndi.zip
