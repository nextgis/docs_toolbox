Central lines of polygons
============================

This instrument creates centerlines for polygons. It is helpful for transforming roads or rivers digitized as polygons into lines.

.. figure:: _static/centerline_result_en.png
   :name: centerline_result_pic
   :align: center
   :width: 20cm

   Input polygon layer and resulting line layer

Inputs:

* Polygon vector layer in a GDAL-supported format, e.g. GeoPackage, GeoJSON, MapInfo TAB, ESRI Shapefile (the latter two should be in ZIP archive).

Outputs:

* Line vector layer in GeoPackage.


Launch the tool: https://toolbox.nextgis.com/t/centerline

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Calculate max distance between polygon nodes <https://toolbox.nextgis.com/t/maxdist?from-related-tools=1>`_
   * `Point inside polygon coordinates <https://toolbox.nextgis.com/t/centroid2attr?from-related-tools=1>`_