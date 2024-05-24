Set of squares generator
========================

This tool creates a set of square grids (polygons) and a transect of their detour for a given territory.

Inputs:

* x0 - Longitude of point 0
* y0 - Latitude of point 0
* x1 - Longitude of point 1
* y1 - Latitude of point 1
* Size 1 - Number of cells on the first axis
* Size 2 - Number of cells on the second axis
* Side - Cell generation side (right, left)
* Cell size - The size of a cell’s side, meters

Calculation algorithm: from the point 0 in the direction of the point 1 a line is drawn with a length equal to "Size 1" * "Cell size". From this line, either to the right or left of it, a second line is laid out with the length of "Size 2" * "Cell size", meters. These two lines form a grid of squares.

The result of the process is a set of layers:

* rect1 - a grid of cells the size of "Size 1" * "Size 2" cells, the center of the first cell is at the point 0
* rect2 - a grid of smaller cells the size of "Size 1" * "Size 2" cells (i.e. 4 times larger cells, each large cell is divided into 4 parts)
* line1 - bypass lines in the direction, which if perpendicular to the line represented by the point 0 and point 1
* line2 - bypass lines in the direction, which is parallel to the line represented by the point 0 and point 1
* centers - cell centers of rect1 grid

Launch tool: https://toolbox.nextgis.com/operation/quadro

Download sample results: https://nextgis.ru/data/toolbox/quadro/outputs.zip

View the results on an interactive map: https://demo.nextgis.com/resource/4582/display?panel=layers

.. figure:: _static/quadro.png
   :align: center
   :width: 16cm
   
An example of the results
