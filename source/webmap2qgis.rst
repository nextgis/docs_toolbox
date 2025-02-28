Web Map into QGIS project
=======================
The tool works with Web GIS data: converts vector layers and its styles from any chosen Web Map into QGIS project and GeoPackage file.

Inputs:

* Web GIS address – URL of the Web GIS, containing target Web Map. For example, https://demo.nextgis.com.
* Web Map ID - numeric value, ID of the Web GIS resource (Web Map) to be converted into QGIS project.
* Login – Web GIS user login.
* Password – Web GIS user password.
* Extent - by default, the extent of the Web Map is used. You can enter a different extent in EPSG:4326. Format: bottom, left, top, right (South, West, North, East). Separate by comma. Example: ``54.5, 102.5, 59, 116``.

Outputs:

* ZIP-archive with QGIS project file (.qgs) and GeoPackage file, containing vector layers.

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/uFiOJfK6VQw?si=HK0H6sg7hhF7i7na" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch on `youtube <https://youtu.be/uFiOJfK6VQw?si=VN6jPbsW_5TSWNRY>`_.

Launch the tool: https://toolbox.nextgis.com/operation/webmap2qgis

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/webmap2qgis/webmap2qgis_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/webmap2qgis/webmap2qgis_outputs.zip>`_ to additionally check the results.
