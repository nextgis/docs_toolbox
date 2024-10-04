Join layer and table by field
=============================

The tool combines data from a table and a layer using a given field. The tool involves the use of two different join types: one-to-one - finds the first matching element of the table and attaches its attributes; one-to-many - connects all elements of the table for which the given field matches, the geometry of the feature is duplicated for each element.

Inputs:

* Web GIS URL - address of the used Web GIS
* resource_id - layer ID to combine from the currently used Web GIS
* CSV file for join
* Key field in WebGIS layer - the name of the field in the Web GIS layer
* Target field in CSV - field name in the table
* Join type - enter "1" for one-to-one, otherwise the default join bype is "one-to-many"

Outputs:

*  layer in ESRI Shapefile format, which is in an archive (zip)

Launch tool: https://toolbox.nextgis.com/operation/join_by_field

Usage example:

.. figure:: _static/join_by_field.png
   :align: center
   :width: 16cm

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/join_by_field/join_by_field_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/join_by_field/join_by_field_outputs.zip>`_ to additionally check the results.
