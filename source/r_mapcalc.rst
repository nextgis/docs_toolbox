Raster calculator (GRASS)
==============================

This tool performs calculations on single band rasters. The tool is based on `r.mapcalc <https://grass.osgeo.org/grass83/manuals/r.mapcalc.html>`_.

Input:

* Single band GDAL supported raster, e.g. GeoTIFF. Add at least one raster file (to the "A" field). You can upload up to 8 raster files.

    * A – required field;
    * B – optional field;
    * C – optional field;
    * D – optional field;
    * E – optional field;
    * F – optional field;
    * G – optional field;
    * H – optional field;

* Expression – required field. Use arithmetic (``+, -, /, *`` etc.) or logical (``>, ==`` etc.) operators, or functions (``log(x), if(x) `` etc.) to build an expression.  The whole list is available `here <https://grass.osgeo.org/grass83/manuals/r.mapcalc.html>`_.  Variables (rasters) should be specified as A, B, C etc. Example: ``(A+B)/C``.

Output:

* GeoTIFF file with the result of the calculation.

Launch the tool: https://toolbox.nextgis.com/t/r_mapcalc

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/r_mapcalc/r_mapcalc_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/r_mapcalc/r_mapcalc_outputs.zip>`_ to additionally check the results.

.. admonition:: Related tools

   * `Raster calculator (GDAL) <https://toolbox.nextgis.com/t/raster_calculator>`_
   * `Prepare raster <https://toolbox.nextgis.com/t/prepare_raster>`_
   * `Image clustering <https://toolbox.nextgis.com/t/image_clustering>`_
   * `Prepare and download Sentinel-2 data <https://toolbox.nextgis.com/t/download_and_prepare_l8_s2>`_