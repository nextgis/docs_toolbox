Create temporal cache
=====================

The tool creates several layers from one. Each new layer is a selection of features for a period of time.

Inputs:

* gis_url - address of the used Web GIS
* resource_id - ID of the polyline layer used by Web GIS
* upper_field - date the feature disappeared
* lower_field - date the feature appeared
* year1_field - the start year of the interval
* year2_field - the end year of the interval
* Date Format - date format for dates
* The output format is GeoJSON, GPKG, CSV, ESRI Shapefile (the default value is ESRI Shapefile)
* Ignore errors - leave blank to stop completion if an empty range is found. Enter 1 to ignore errors

Outputs:

*  archive of layers, each of which is also in an archive (zip)

Launch tool: https://toolbox.nextgis.com/operation/temporal_split

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/temporal_split/temporal_split_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/temporal_split/temporal_split_outputs.zip>`_ to additionally check the results.
