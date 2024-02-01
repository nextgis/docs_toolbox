Combine OSM and Reforma
=======================

Combine building data from OpenStreetMap and Reforma to produce polygon layer with building outlines and all attributes from Reforma.


.. figure:: _static/joinreforma.png
   :align: center
   :width: 16cm
   
   Example of the result data.

Inputs:

* Polygon building layer from OSM, ZIP file.
* Point building data from Reforma, CSV file.

Outputs:

A compressed file containing:

* Polygon layer with building footprints successfuly matched with OSM data, ESRI Shapefile.
* Point layer with source points not matched with OSM data, ESRI Shapefile.
* Source data, CSV file.

Download an example of source data and result: https://nextgis.ru/data/toolbox/joinreforma/joinreforma.zip

Launch tool: https://toolbox.nextgis.com/operation/joinreforma
