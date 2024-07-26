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

Launch tool: https://toolbox.nextgis.com/operation/joinreforma

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/joinreforma/joinreforma_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/joinreforma/joinreforma_outputs.zip>`_ to additionally check the results.
