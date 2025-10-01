Split into equal parts
=======================

Splits polygon layer into equal parts. 

.. note:: Doesn't process multipolygons. You can first `transform Multipart to singleparts <https://toolbox.nextgis.com/t/qgis_multiparttosingleparts>`_.

Inputs:

* Source file. Vector polygon layer in one of the formats, supported by GDAL, e.g. Shapefile in ZIP-archive, GeoJSON, GeoPackage.
* Number of parts. Specify, into how many parts source polygon should be split. 

Output:

* Polygon GeoPackaged in a ZIP archive.

Launch the tool: https://toolbox.nextgis.com/t/split_to_equal


.. figure:: _static/split_to_equal_result.png
   :name: split_to_equal_result_pic
   :align: center
   :width: 11cm

   Example of a split polygon

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/split_to_equal/split_to_equal_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/split_to_equal/split_to_equal_outputs.zip>`_ of the tool run.

.. admonition:: Related tools

   * `Meter grid <https://toolbox.nextgis.com/t/grid>`_
   * `Generate a set of squares with transects <https://toolbox.nextgis.com/t/quadro>`_