Convert GeoPackage to MapInfo Enhanced TAB
==========================================

Convert GeoPackage (GPKG) to Enhanced TAB (NativeX) for MapInfo Pro 15.2 and above. 

If you have geodata with global coverage containing attribute values in a variety of languages, converting it in GDAL or QGIS may pose problems because Unicode characters are not supported for the format. 

This tool allows you to preserve the correct symbols. The output encoding is UTF-8.

Inputs:

* Single GeoPackage file with one vector layer.

Outputs:

* ZIP archive with MapInfo Enhanced TAB (NativeX) result file.

Launch the tool: https://toolbox.nextgis.com/t/gpkg2etab

Example:

.. figure:: _static/gpkg2etab_result_en.jpg
   :name: gpkg2etab_result_pic
   :align: center
   :width: 20cm

   Example output with Greek names

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/gpkg2etab/gpkg2etab_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/gpkg2etab/gpkg2etab_outputs.zip>`_ of the tool run.
