Merge vector layers
===================
   
The tool merges many vector layers into one. Layers should be of same geometry type.

Inputs:

* ZIP archive with ESRI Shapefile, GeoJSON, GeoPackage or MapInfo TAB layers. You can combine files of different formats and coordinate reference systems in one set. Subfolders in the archive are supported.

Outputs:

* GeoPackage file with the result of the merge.

The tool has no limit on the number of input layers. The name of the source layer is also saved.

Launch the tool: https://toolbox.nextgis.com/t/ogrmerge

Example:

.. figure:: _static/ogrmerge_input_en.png
   :name: ogrmerge_input_pic
   :align: center
   :width: 16cm

   Example input

.. figure:: _static/ogrmerge_result_en.png
   :name: ogrmerge_result_pic
   :align: center
   :width: 16cm

   Example output

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Merge two Web GIS vector layers <https://toolbox.nextgis.com/t/ngw_merge_layers?from-related-tools=1>`_