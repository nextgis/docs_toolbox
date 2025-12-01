Intersector
===========

The tool intersects all layers of the nextgis.com web map using the specified geometry and generates a report for each layer. 

Inputs:

* Web GIS address. NextGIS Web URL, e.g.: https://sandbox.nextgis.com;
* Web Map ID. Numbers at the end of the Web Map URL;
* WKT geometry. Geometry for intersection in WKT format. Coordinate system: EPSG:3857.

Outputs:

*  XLSX table with a list of intersected layers.

Launch the tool: https://toolbox.nextgis.com/t/ngw-intersect
	
Example:

.. figure:: _static/ngw_intersect_input_en.png
   :name: ngw_intersect_input_pic
   :align: center
   :width: 16cm

   Example input

.. figure:: _static/ngw_intersect_result_en.png
   :name: ngw_intersect_result_pic
   :align: center
   :width: 16cm

   Example output

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/ngw_intersect/ngw_intersect_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/ngw_intersect/ngw_intersect_outputs.zip>`_ to additionally check the results.

.. admonition:: Related tools

   * `Polygon intersection <https://toolbox.nextgis.com/t/vectorclip?from-related-tools=1>`_