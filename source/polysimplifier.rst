Polygons topological simplifier
===============================

This tool simplifies linear and polygonal geometries. Useful for simplifying administrative boundaries, vegetation, and other polygons that touch each other. This tool keeps topology, boundaries between features will not get gaps or overlaps.

Input:

* Linear or polygonal layer file in OGR-compatible vector format. For formats with several files upload a ZIP archive.
* Simplification percentage - Range 1 to 100. Use 90 for testing. The **higher** the percentage - the **higher** the simplification.

Output:

* Simplified GeoJSON

Launch the tool: https://toolbox.nextgis.com/t/polysimplifier

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/polysimplifier/polysimplifier_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/polysimplifier/polysimplifier_outputs.zip>`_ to additionally check the results.

.. admonition:: Related tools

   * `Advanced vector generalization <https://toolbox.nextgis.com/t/generalization?from-related-tools=1>`_
   * `Split Complex Polygons <https://toolbox.nextgis.com/t/splitcomplex?from-related-tools=1>`_
