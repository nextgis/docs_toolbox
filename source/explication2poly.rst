Explication to a polygon
========================

The tool converts an explication report in correct format to a polygon. Explication report has to be an MS Excel file that contains data about direcions and distances between points. Directions should be presented in degrees and corresponds to magnetic azimuth.

.. figure:: _static/poly2explication-1.png
   :align: center
   :width: 16cm
   
   Example of a source xlx(x) file

Inputs:

* XLS(X) file - MS Excel file containing the explicaton report;
* Latitude of an anchor point. This value is specified in the coordinate system EPSG 4326. Use dot as a separator between the integer part and the fractional part;
* Longitude of an anchor point. This value is specified in the coordinate system EPSG 4326. Use dot as a separator between the integer part and the fractional part.

.. note::
    Due to inaccuracies in measuring angles and distances on the ground, the first point of the output polygon may be farther from the last one than on the ground. As a rule, the difference does not exceed 2-3 meters. 

Outputs:

*  Zipped polygonal shapefile

   Launch tool: https://toolbox.nextgis.com/operation/explication2poly
   
**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/explication2poly/explication2poly_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/explication2poly/explication2poly_outputs.zip>`_ to additionally check the results.
