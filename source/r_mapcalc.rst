Raster calculator (GRASS)
==============================

The tool allows calculations with single band rasters. The tool is based on `r.mapcalc <https://grass.osgeo.org/grass83/manuals/r.mapcalc.html>`_.

Input:

* A – obligatory field. Single band GDAL supported raster, e.g. GeoTIFF.
* B – optional field. Single band GDAL supported raster.
* C – optional field. Single band GDAL supported raster.
* D – optional field. Single band GDAL supported raster.
* E – optional field. Single band GDAL supported raster.
* F – optional field. Single band GDAL supported raster.
* G – optional field. Single band GDAL supported raster.
* H – optional field. Single band GDAL supported raster.
* Expression – obligatory field. Use arithmetic (+, -, /, * etc.) or logical (>, == etc.) operators, as well as functions (log(x), if(x) etc.) to build an expression.  The whole list is available `here <https://grass.osgeo.org/grass83/manuals/r.mapcalc.html>`_.  Variables (rasters) should be specified as A, B, C etc. An example of expression: **(A+B)/C**

Output:

* GeoTIFF file with a result of calculation.

Launch the tool: https://toolbox.nextgis.com/operation/r_mapcalc

:download:`Example <files/r_mapcalc_example.zip>` of source data.

