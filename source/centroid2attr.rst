Point inside polygon coordinates
================================

Calculate coorinates of a point guaranteed to be inside a polygon and add the calculated coordinates to point_X, point_Y attributes. PointOnSurface method.

Inputs:

* Polygon vector layer in one of the formats, supported by GDAL, e.g. Shapefile in ZIP-archive, GeoJSON, GeoPackage.

Outputs:

* ZIP with polygonal shapefile with two fields added: point_X, point_Y 


.. figure:: _static/point_on_surface.png
   :align: center
   :width: 16cm
   
   Visualization of the calculated centroids 

.. figure:: _static/centroid2attr_en.png
   :align: center
   :width: 16cm

   Resulting feature table of the layer with added attributes

Launch the tool: https://toolbox.nextgis.com/t/centroid2attr

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/centroid2attr/centroid2attr_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/centroid2attr/centroid2attr_outputs.zip>`_ to additionally check the results.
