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
* Extent. Instead of uploading a layer, you can set a bounding box. Draw a custom rectangle on the map below. The Extent field will be filled with the numeric value that you can adjust manually;
*  Vertical orienting or with fine size. By default, ``simple`` mode is used, the grid looks vertical in WGS 84 (EPSG:3857) projection, but angles and distances may be distorted. Enter ``fine`` to get a grid with more precizely matching angles and distances, however it will look tilted in EPSG:3857.

Output:

* GeoPackage containing the grid. Each cell/point of the grid has the following attributes: number (cells are numbered vertically, top to bottom, left to right, starting with the first left column even if it doesn't reach the top), row_index and col_index. To display the numbers, enable lables in the layer style settings and select the desired attribute.

.. figure:: _static/grid_numbers.png
   :align: center
   :name: grid_rect_all_pic
   :width: 10cm

   Cell numbers displayed


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



Launch the tool: https://toolbox.nextgis.com/t/grid

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/grid/grid_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/grid/grid_outputs.zip>`_ to additionally check the results.
