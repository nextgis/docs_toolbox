Fix geometries
==============

Fixes incorrect geometries in vector files. To find out if a vector file has invalid geometries, use `Check geometries <https://toolbox.nextgis.com/t/check_geometries>`_.

Inputs:

* ZIP archive with vector files. Only single-file formats are supported (Geopackage, GeoJSON, etc., but **not** ESRI Shapefile).

Outputs:

* File with fixed geometries in the same format as input.

Launch the tool: https://toolbox.nextgis.com/t/fix_geometries

.. figure:: static/fix_geometries_input.png
   :name: fix_geometries_input_pic
   :align: center
   :width: 16cm

   Example input

.. figure:: _static/fix_geometries_result.png
   :name: fix_geometries_result_pic
   :align: center
   :width: 16cm

   Example output image

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/fix_geometries/fix_geometries_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/fix_geometries/fix_geometries_outputs.zip>`_ of the tool run.
