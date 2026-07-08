MapInfo ready for QGIS
=======================

Despite that QGIS is able to work with  MapInfo TAB without any preliminary transformation, still, there is an issue with rendering style of a layer. This tool solves named problem as it converts TAB into GeoPackage plus QML style files.

Inputs:

* Source file - ZIP-archive with MapInfo TAB. If archive also includes WOR file, it should be in the root of the archive, do not add it to any directory.

Output:

* ZIP-archive with GeoPackage and  QML style files for each layer.

Launch the tool: https://toolbox.nextgis.com/t/mapinfo2qgis

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Convert format of vector layer <https://toolbox.nextgis.com/t/convert?from-related-tools=1>`_
  * `DWG to DXF <https://toolbox.nextgis.com/t/import_dwg?from-related-tools=1>`_
  * `KML to geodata <https://toolbox.nextgis.com/t/kml2geodata?from-related-tools=1>`_