Strip ZM from vector layer
============================
The tool converts vector file to same format stripping ZM measurements. E.g., converts geometries from PolygonZ into Polygon.

Input: 

* Source data - vector file in GeoPackage or GeoJSON format. Geometries could contain Z and/or M measurements.

Output:

* GeoPackage or GeoJSON file without ZM coordinates in geometry.

Launch the tool: https://toolbox.nextgis.com/t/flatten

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Multipart to singleparts <https://toolbox.nextgis.com/t/qgis_multiparttosingleparts?from-related-tools=1>`_