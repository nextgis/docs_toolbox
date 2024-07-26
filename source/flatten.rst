Strip ZM from a vector layer
============================
The tool converts vector file to same format stripping ZM measurements. E.g., converts geometries from PolygonZ into Polygon.

Input: 

* Source data - vector file in GeoPackage or GeoJSON format. Geometries could contain Z and/or M measurements.

Output:

* GeoPackage or GeoJSON file without ZM coordinates in geometry.

Launch tool: https://toolbox.nextgis.com/operation/flatten

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/flatten/flatten_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/flatten/flatten_outputs.zip>`_ to additionally check the results.
