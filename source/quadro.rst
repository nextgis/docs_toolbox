Set of squares generator
========================

This tool creates a set of square grids (polygons) and a transect of their detour for a given territory.

Inputs:

* x0 - Longitude of the anchor point
* y0 - Latitude of the anchor point
* x1 - Longitude of the reference point
* y1 - Latitude of the reference point
* size1 - Number of cells on the first axis
* size2 - Number of cells on the second axis
* side - Cell generation side (right, left)
* base_interval - The size of a cell’s side, meters

Calculation algorithm: from the anchor point in the direction of the reference point a line is drawn with a length equal to size1 * base_interval. From this line, either to the right or left of it, a second line is laid out with the length of size2 * base_interval, meters. These two lines form a grid of squares.

The result of the process is a set of layers:

* rect1 - a grid of cells the size of size1 * size2 cells, the center of the first cell is at the anchor point
* rect2 - a grid of smaller cells the size of size1 * size2 cells (i.e. 4 times larger cells, each large cell is divided into 4 parts)
* line1 - bypass lines in the direction, which if perpendicular to the line represented by the anchor point and reference point
* line2 - bypass lines in the direction, which is parallel to the line represented by the anchor point and reference point
* centers - grid cell centers rect1

Launch tool: https://toolbox.nextgis.com/operation/quadro

Download sample results: https://nextgis.ru/data/toolbox/quadro/outputs.zip

View the results on an interactive map: https://demo.nextgis.com/resource/4582/display?panel=layers

.. figure:: _static/quadro.png
   :align: center
   :width: 16cm
   
An example of the results
