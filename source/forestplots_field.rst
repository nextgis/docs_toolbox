Create forestplots scheme for Garmin
====================================

The tool generates forest field plots in KMZ format ready to upload to Garmin devices. Areas located closer than 10 m from the plot border are discarded. A buffer zone is added around the plot at a distance of 50 m.

Inputs:

*  Input polygon dataset. Supported formats are zipped shapefile, MapInfo TAB or OGR-compatible file. Must contain only one feature without rings.
*  Step between points. Distance between plots in meters. Default 55 meters.

Outputs:

* KMZ file with forest field plots ready to upload to Garmin devices.
* Separate JPG file with forest plots scheme.


Launch the tool: https://toolbox.nextgis.com/t/forestplots_field

.. figure:: _static/forest-circular-plots.jpg
   :align: center
   :width: 8cm

   An example of result uploded to Garmin

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Generate a set of squares with transects <https://toolbox.nextgis.com/t/quadro?from-related-tools=1>`_
   * `Coordinates to polygon <https://toolbox.nextgis.com/t/coords2poly?from-related-tools=1>`_
   * `Geotag photos using GPX track <https://toolbox.nextgis.com/t/gpx2exif?from-related-tools=1>`_
   * `KML to geodata <https://toolbox.nextgis.com/t/kml2geodata?from-related-tools=1>`_