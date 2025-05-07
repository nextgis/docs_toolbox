Check geometries
================

Checking the vector file for geometry validity. The output is a CSV file with a list of errors and coordinates and a GeoJSON file with geometries of the location of errors.

Inputs:

* ZIP archive with vector files. A ZIP archive should be arranged in this way: files of formats consisting of a single file should be in the form of the file itself. files of multiple file formats must be in the form of a ZIP archive

Outputs:

* output_csv_file
* output_geojson_file

Launch the tool: https://toolbox.nextgis.com/t/check_geometries

.. figure:: static/check_geometries_input_en.png
   :name: check_geometries_input_pic
   :align: center
   :width: 16cm

   Example input

.. figure:: _static/check_geometries_result_en.png
   :name: check_geometries_result_pic
   :align: center
   :width: 16cm

   Example output image

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/check_geometries/check_geometries_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/check_geometries/check_geometries_outputs.zip>`_ of the tool run.
