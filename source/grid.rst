Meter grid
========================

.. figure:: _static/grids_multi.png
   :align: center
   :name: grids_multi_pic
   :width: 10cm

   A combination of generated grids
   
The tool generates a grid within the boundaries of features of a vector layer or a bounding box. The grid size is set in meters. Features can be anywhere in the world.

Inputs:

* Cell size in meters;
* Mode: ``points`` or ``rect`` (squares);
* Algorithm for cropping the grid along the feature borders: ``all`` (leave all the squares in extent), ``touches`` (leave all the squares touching features), ``intersection`` (crop the squares along the borders of the features);
* GeoPackage file with polygons or multipolygons. Calculation time depends on the number of nodes in the boundary layer; 
* Extent. Instead of uploading a layer, you can set a bounding box. Draw a custom rectangle on the map below. The Extent field will be filled with the numeric value that you can adjust manually.

Resulting grids with different settings:

.. figure:: _static/grid_rect_all.png
   :align: center
   :name: grid_rect_all_pic
   :width: 10cm

   Squares - all
   
   
.. figure:: _static/grid_rect_touches.png
   :align: center
   :name: grid_rect_touches_pic
   :width: 10cm

   Squares - touches
   
   
.. figure:: _static/grid_rect_intersection.png
   :align: center
   :name: grid_rect_intersection_pic
   :width: 10cm

   Squares - intersection
   
   
.. figure:: _static/grid_point_all.png
   :align: center
   :name: grid_point_all_pic
   :width: 10cm

   Points - all
   
   
.. figure:: _static/grid_point_intersection.png
   :align: center
   :name: grid_point_intersection_pic
   :width: 10cm

   Points - intersection

.. todo:: _static/grid_point_touches.png
   :align: center
   :name: grid_point_touches_pic
   :width: 10cm

   Points - touches



Launch tool: https://toolbox.nextgis.com/operation/grid

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/grid/grid_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/grid/grid_outputs.zip>`_ to additionally check the results.
