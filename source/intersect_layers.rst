Intersect layers
================

The tool intersects a polygonal layer with another vector layer (any type of geometry) and outputs the result as a set of CSV files.

Inputs:

* Shapefile with a layer to intersect. ESRI Shapefile (ZIP-archive) with any type of geometries. Objects from this layer are meant to be intersected with the objects from the polygonal layer
* Shapefile with a polygonal layer. ESRI Shapefile (ZIP-archive) with a polygonal layer. Intersection status with another layer will be traced for each object from this layer
* Field name for CSV files. Field name from the polygonal layer. Values from this field will be used to name CSV files. If this field is blank, CSV file names will be generated automatically.

Outputs:

*  Zipped CSV files, each of which describes one of the objects of the polygonal layer. If an object from a polygon layer has an intersection with an object from another layer, the CSV file will contain the coordinates of the center and the WKT description of the polygon.

Launch the tool: https://toolbox.nextgis.com/t/intersect_layers

.. figure:: _static/intersect_layers_result.png
   :name: intersect_layers_result_pic
   :align: center
   :width: 16cm

   Parts of hydrography intersecting with the park are marked by dotted lines

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/intersect_layers/intersect_layers_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/intersect_layers/intersect_layers_outputs.zip>`_ to additionally check the results.

.. admonition:: Related tools

   * `Intersector <https://toolbox.nextgis.com/t/ngw_intersect>`_
   * `Polygon intersection <https://toolbox.nextgis.com/t/vectorclip>`_
   * `Erase overlapping areas from the layer <https://toolbox.nextgis.com/t/eraser>`_