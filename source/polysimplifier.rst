Polygons topological simplifier
===============================

This tool simplifies linear and polygonal geometries. Useful for simplifying administrative boundaries, vegetation, and other polygons that touch each other. This tool keeps topology, boundaries between features will not get gaps or overlaps.

Input:

* Linear or polygonal layer in GeoJSON
* Percentage of simplify - number of vertices to keep. Range 1 to 100. Use 90 for tesing. The **higher** the percentage - the **higher** the simplification.

Output:

* Simplified GeoJSON

Launch tool: https://toolbox.nextgis.com/operation/polysimplifier

Download an example of source data and result: https://nextgis.com/data/toolbox/polysimplifier/polysimplifier.zip
