Reproject coordinates
========================

Tool reprojects coordinates of the objects, presented in CSV file, into a given coordinate system.

Inputs:

* CSV file - file with a list of objects and its coordinates
* ID of X coordinate - index number of the column in CSV file, where X coordinates are located (longitude).
* ID of Y coordinate - index number of the column in CSV file, where Y coordinates are located (latitude).
* ID of the first row - index number of the row, from which reprojection should be applied.
* Separator - specify separator type, which is used in source CSV (e.g., ; (semicolon) or , (comma) and so on).
* Source CRS - coordinate reference system, used in source CSV. Should be specified in proj4 format (e.g. +proj=longlat +ellps=WGS84 +datum=WGS84 + no_defs).
* Target CRS - coordinate reference system into which data will be reprojected. Should be specified in proj4 format (optional, by default "+proj=longlat +ellps=WGS84 +datum=WGS84 + no_defs" will be applied).

Output: 

Launch the tool: https://toolbox.nextgis.com/t/coord_recalc

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Convert format of vector layer <https://toolbox.nextgis.com/t/convert?from-related-tools=1>`_
  * `KML to geodata <https://toolbox.nextgis.com/t/kml2geodata?from-related-tools=1>`_