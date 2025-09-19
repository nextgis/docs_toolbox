Polygon intersection
====================

Finds overlapping areas between features of 2 polygon layers.

Inputs:

* Polygon layer 1
* Polygon layer 2

Files should be in GDAL-supported format, e.g. GeoPackage, GeoJSON, MapInfo TAB, ESRI Shapefile (the last two - in ZIP-archive).

You can use this tool to clip line geometry. Upload the line layer to the field 1 and the clipping boundary to the field 2. 

Outputs:

* GeoPackage file with polygon layer containing only the overlapping areas.

Launch the tool: https://toolbox.nextgis.com/t/vectorclip

.. figure:: _static/vectorclip_input_en.png
   :name: vectorclip_input_pic
   :align: center
   :width: 16cm

   Example input

.. figure:: _static/vectorclip_result_en.png
   :name: vectorclip_result_pic
   :align: center
   :width: 16cm

   Example output image

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/vectorclip/vectorclip_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/vectorclip/vectorclip_outputs.zip>`_ of the tool run.