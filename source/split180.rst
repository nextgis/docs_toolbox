Split data by 180 degrees 
=====================================

Split vector layer feature geometries at antimeridian (180th meridian) for correct visualization on online maps.

.. figure:: _static/split180tiles_en.png
   :name: split180tiles_pic
   :align: center
   :width: 20cm

   Data split by the antimeridian on a Web Map

Inputs:

* Vector layer in a GDAL-supported format, e.g. GeoPackage, GeoJSON, MapInfo TAB, ESRI Shapefile (the latter two should be in ZIP archive).

Outputs:

* Vector layer in GeoPackage.

To make sure the layer is correctly displayed on the Web Map, set the adapter to "Tiles". 

.. to do:: See how it works in our video:



Launch the tool: https://toolbox.nextgis.com/t/split180

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/split180/split180_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/split180/split180_outputs.zip>`_ to additionally check the results.
