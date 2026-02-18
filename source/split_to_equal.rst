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

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Meter grid <https://toolbox.nextgis.com/t/grid?from-related-tools=1>`_
   * `Set of squares with transects <https://toolbox.nextgis.com/t/quadro?from-related-tools=1>`_