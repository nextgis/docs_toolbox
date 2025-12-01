Check geometries (QGIS)
=======================

Checks a vector file for geometry validity using the QGIS *checkvalidity* algorithm. 

Inputs:

* ZIP archive with vector files in single-file formats (for example, GeoPackage, GeoJSON, etc.).

.. note:: Even if you have one file only, it needs to be in a ZIP archive.

Outputs:

* CSV file with a list of errors and coordinates;
* GeoJSON file with points marking the location of the errors.

Launch the tool: https://toolbox.nextgis.com/t/qgis_check_geometries

Example:

.. figure:: _static/qgis_check_geometries_result.png
   :name: qgis_check_geometries_result_pic
   :align: center
   :width: 16cm

   Example output. Points mark the geometry errors

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/qgis_check_geometries/qgis_check_geometries_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/qgis_check_geometries/qgis_check_geometries_outputs.zip>`_ of the tool run.

.. admonition:: Related tools

   * `Fix geometries (QGIS) <https://toolbox.nextgis.com/t/qgis_fix_geometries?from-related-tools=1>`_
   * `Fix geometries <https://toolbox.nextgis.com/t/fix_geometries?from-related-tools=1>`_