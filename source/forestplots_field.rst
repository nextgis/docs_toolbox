Create forestplots scheme for Garmin
====================================

The tool generates forest field plots in KMZ format ready to upload to Garmin devices. Areas located closer than 10 m from the plot border are discarded. A buffer zone is added around the plot at a distance of 50 m.

Inputs:

*  Input polygon dataset. Supported formats are zipped shapefile, Mapinfo TAB or OGR-compatible file. Must contain only one feature without rings.
*  Step between points. Distance between plots in meters. Default 55 meters.

Outputs:

* KMZ file with forest field plots ready to upload to Garmin devices.
* Separate JPG file with forest plots scheme.

Download an example of source data and result: https://nextgis.ru/data/toolbox/forestplots_field/forestplots_field.zip

Launch tool: https://toolbox.nextgis.com/operation/forestplots_field

.. figure:: _static/forest-circular-plots.jpg
   :align: center
   :width: 16cm

   An example of result uploded to Garmin. 
