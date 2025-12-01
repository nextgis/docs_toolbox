Convert format of vector layer
==============================

Convert vector layer to other file format.

Coordinate refrence system (CRS) is not changing.
If output format is ESRI Shapefile, encoding of attributes cast to UTF-8.

Input:

*  Vector layer file - GeoJSON, GPKG, GPX or KMZ file, ZIP archive with ESRI Shapefile or any other vector file compatible with GDAL library.
*  Name of output format

.. note::
   If uploaded file has incompatible format (SQL or singe SHP file) an error message will appear.

Output:

* ZIP archive with vector layers

Launch the tool: https://toolbox.nextgis.com/t/convert

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/convert/convert_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/convert/convert_outputs.zip>`_ to additionally check the results.

.. admonition:: Related tools

   * `Reprojecting coordinates <https://toolbox.nextgis.com/t/coord_recalc?from-related-tools=1>`_
   * `Check geometries <https://toolbox.nextgis.com/t/check_geometries?from-related-tools=1>`_
   * `KML to geodata <https://toolbox.nextgis.com/t/kml2geodata?from-related-tools=1>`_
   * `MapInfo ready for QGIS <https://toolbox.nextgis.com/t/mapinfo2qgis?from-related-tools=1>`_