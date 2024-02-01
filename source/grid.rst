Meter grid
==========

.. figure:: _static/grids-demo.png
   :align: center
   :width: 16cm

   Generated grid
   
The tool generates a grid within the boundaries of features of a vector layer. The grid size is set in meters. Features can be anywhere in the world.

Inputs:

*  A multipolygon layer with one or more features. It should be GeoPackage
*  Grid step in meters
*  Mode: points (points), rect (squares)
*  Algorithm for cropping the grid along the borders: all (leave all the squares in extent), touches (leave all the squares touching features), intersection (crop the squares along the borders of the features)

.. figure:: _static/grid-1000-rect-all.png
   :align: center
   :width: 16cm

   all
   
   
.. figure:: _static/grid-1000-rect-touches.png
   :align: center
   :width: 16cm

   touches
   
   
.. figure:: _static/grid-1000-rect-intersection.png
   :align: center
   :width: 16cm

   intersection
   
   
.. figure:: _static/grid-1000-point-all.png
   :align: center
   :width: 16cm

   all для точек
   
   
.. figure:: _static/grid-1000-point-intersection.png
   :align: center
   :width: 16cm

   touches и intersection для точек

   
.. figure:: _static/grid-planet.png
   :align: center
   :width: 16cm

   Generated grids for several polygons in different places of the globe
   

*  output geodata format - GeoJSON, ESRI Shape, Mapinfo TAB

Outputs:

* Geopackage


Launch tool: https://toolbox.nextgis.com/operation/grid
