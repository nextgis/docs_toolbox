Polygons topological simplifier
===============================

This tool simplifies linear and polygonal geometries. Useful for simplifying administrative boundaries, vegetation, and other polygons that touch each other. This tool keeps topology, boundaries between features will not get gaps or overlaps.

Input:

* Linear or polygonal layer in GeoJSON
* Percentage of simplify - number of vertices to keep. Range 1 to 100. Use 90 for tesing. The **higher** the percentage - the **higher** the simplification.

Output:

* Simplified GeoJSON

Launch tool: https://toolbox.nextgis.com/operation/polysimplifier

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/polysimplifier/polysimplifier_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/polysimplifier/polysimplifier_outputs.zip>`_ to additionally check the results.
