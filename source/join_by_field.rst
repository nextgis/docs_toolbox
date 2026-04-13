Join layer and table by field
=============================

The tool combines data from a table and a layer using a given field. The tool involves the use of two different join types: one-to-one - finds the first matching element of the table and attaches its attributes; one-to-many - connects all elements of the table for which the given field matches, the geometry of the feature is duplicated for each element.

Inputs:

* Web GIS URL - address of the Web GIS on NextGIS Web platform in the following format: ``https://example.nextgis.com``;
* Resource ID - numbers at the end of the source layer URL;
* CSV file for join;
* Key field in WebGIS layer - the name of the field in the Web GIS layer;
* Target field in CSV - field name in the table;
* Join type - select one-to-one or one-to-many.

Outputs:

*  layer in ESRI Shapefile format, which is in an archive (zip)

Launch the tool: https://toolbox.nextgis.com/t/join_by_field

Usage example:

.. todo:: _static/join_by_field.png
   :align: center
   :width: 16cm

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Update Web GIS layer from CSV <https://toolbox.nextgis.com/t/update_vector_layer?from-related-tools=1>`_
