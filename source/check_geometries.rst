Check geometries
================

Checking the vector file for geometry validity. The output is a CSV file with a list of errors and coordinates and a GeoJSON file with geometries of the location of errors.

Inputs:

* ZIP archive with vector files. 

Single-file formats should be in the root of the archive. For multi-file formats such as ESRI Shapefile, each layer should be put in a separate ZIP inside the main input archive. Input archive may contain mixed files.

.. figure:: _static/check_geometries_structure_en.png
   :name: check_geometries_structure_pic
   :align: center
   :width: 18cm

   Example of possible archive structure. Archive input.zip contains a single-file GeoJSON and a zipped MapInfo TAB

Outputs:

* CSV file containing the list of errors;
* GeoJSON file with points marking the placement of the errors.

Launch the tool: https://toolbox.nextgis.com/t/check_geometries



.. figure:: _static/check_geometries_result.png
   :name: check_geometries_result_pic
   :align: center
   :width: 18cm

   Example output image

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/check_geometries/check_geometries_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/check_geometries/check_geometries_outputs.zip>`_ of the tool run.

.. admonition:: Related tools

   * `Fix geometries <https://toolbox.nextgis.com/t/fix_geometries>`_
   * `Fix geometries (QGIS) <https://toolbox.nextgis.com/t/qgis_fix_geometries>`_
   * `Check geometries (QGIS) <https://toolbox.nextgis.com/t/qgis_check_geometries>`_