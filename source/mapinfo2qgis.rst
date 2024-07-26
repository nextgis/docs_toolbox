MapInfo ready for QGIS
=======================

Despite that QGIS is able to work with  MapInfo TAB without any preliminary transformation, still, there is an issue with rendering style of a layer. This tool solves named problem as it converts TAB into GeoPackage plus QML style files.

Inputs:

* Source file - ZIP-archive with MapInfo TAB. If archive also includes WOR file, it should be in the root of the archive, do not add it to any directory.

Output:

* ZIP-archive with GeoPackage and  QML style files for each layer.

Launch the tool: https://toolbox.nextgis.com/operation/mapinfo2qgis

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/mapinfo2qgis/mapinfo2qgis_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/mapinfo2qgis/mapinfo2qgis_outputs.zip>`_ to additionally check the results.
