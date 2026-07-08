Split at 180th meridian 
=====================================

Split vector layer feature geometries at antimeridian (180th meridian).

Such split is often required for correct use of such feature in different GIS software and for correct visualization on online maps.

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

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Split Complex Polygons <https://toolbox.nextgis.com/t/splitcomplex?from-related-tools=1>`_
  * `Split into equal parts <https://toolbox.nextgis.com/t/split_to_equal?from-related-tools=1>`_
