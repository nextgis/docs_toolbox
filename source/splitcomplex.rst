Split Complex Polygons
======================

Splits polygons with too many vertices into smaller parts. Each part is a separate feature that keeps all the attributes of the split polygon.

Inputs:

* Source file - Vector layer in one of the formats supported by GDAL, e.g. GeoJSON, GeoPackage, zipped Shapefile.
* Max count of vertices - Maximum number of vertices allowed in a polygon. Default is 200000.

Outputs:

* GeoPackage file with split polygons.

Launch the tool: https://toolbox.nextgis.com/t/splitcomplex

.. figure:: _static/splitcomplex_input_en.png
   :name: splitcomplex_input_pic
   :align: center
   :width: 20cm

   Example input

.. figure:: _static/splitcomplex_result_en.png
   :name: splitcomplex_result_pic
   :align: center
   :width: 20cm

   Example output

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Polygons topological simplifier <https://toolbox.nextgis.com/t/polysimplifier?from-related-tools=1>`_
   * `Split into equal parts <https://toolbox.nextgis.com/t/split_to_equal?from-related-tools=1>`_
   * `Advanced vector generalization <https://toolbox.nextgis.com/t/generalization?from-related-tools=1>`_
   * `Split data by 180 degrees <https://toolbox.nextgis.com/t/split180?from-related-tools=1>`_