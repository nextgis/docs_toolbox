Generate a set of squares with transects
==========================================

This tool creates a set of square grids (polygons) and a transect for the territory.

Inputs:

* Coordinates of the first point (center of the first cell), in decimal degrees, example ``40.415378, -3.688743``;
* Coordinates of the second point that indicates direction, in decimal degrees, example ``40.417436, -3.683170``;
* Side - on which side to generate the grid: right or left;
* Cell count 1 - Number of cells on the first axis;
* Cell count 2 - Number of cells on the second axis;
* Cell size - The size of a cell’s side, in meters.

The result of the process is a set of layers:

* rect1 - a grid of cells "Size 1" by "Size 2", the center of the first cell is at the point 1;
* rect2 - a grid of smaller cells (i.e. each large cell is divided into 4 parts);
* line1 - transect lines in the direction perpendicular to the line between points 1 and 2;
* line2 - transect lines in the direction parallel to the line between points 1 and 2;
* centers - cell centers of rect1 grid.

Styles for all the layers are also included as QML files.

Launch the tool: https://toolbox.nextgis.com/t/quadro



View the results on an interactive map: https://demo.nextgis.com/resource/4582/display?panel=layers

.. figure:: _static/quadro_result_styles.png
   :align: center
   :width: 18cm
   
   An example of the results

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Create forestplots scheme for Garmin <https://toolbox.nextgis.com/t/forestplots_field?from-related-tools=1>`_
   * `Meter grid <https://toolbox.nextgis.com/t/grid?from-related-tools=1>`_
