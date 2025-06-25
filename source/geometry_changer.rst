Change geometry for a group of layers
=====================================

The tool changes the geometry of features in all the layers of a group in Web GIS. 

Three modes are available:

* **Delete** - the tool deletes the selected features. The selection is based on the specified values of a layer’s attribute field;
* **Insert** - the tool adds new features from the uploaded ESRI Shapefile. The structure of the file and the layer must match. Otherwise, the tool will not be able to add new features.;
* **Replace** - the tool replaces the geometry value for features with the geometries from the uploaded Shapefile, the values of the specified attribute of which match with the attribute values of the Web GIS layer. The attribute name in the SHP file and the Web GIS layer must match.

Inputs:

* Web GIS Address — URL of your Web GIS (for example, http (s): //mywebgis.nextgis.com);
* Login - NextGIS ID or username of the user who has the permission to write data to the specified resource;
* Password - Web GIS user password;
* Resource Group Identifier - Web GIS Resource ID for the layer group;
* Initial field - Name of the attribute field used to search for features;
* Mode - enter ``Delete``, ``Insert`` or ``Replace``;
* Initial value - The value of the initial field by which the features are selected. If you need to specify multiple values, use a comma to separate them;
* Start year - Starting date of the time range (optional parameter);
* End year - Ending date of the time range (optional parameter)
* SHP file - An ESRI Shapefile (zipped) that contains features. Required parameter in Add and Change modes.

.. note::
    Start year and end year are optional parameters. These parameters allow you to limit the time range for the selected layers. To use these parameters, you must make sure that the time ranges are indicated in the names of the layers of the Web GIS resource. For example, in layer 1245_1246_earl_v.1.0 1245 and 1246 the years are indicated. If these parameters are in use, you need to enter three or four digit values. Other parameters are **required**.

Outputs:

*  A CSV file that contains data on the selected mode, the source field and its value, a list of hyperlinks to features that have been changed. If there are errors, they will also be indicated in this file.


Launch tool: https://toolbox.nextgis.com/operation/geometry_changer

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/geometry_changer/geometry_changer_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/geometry_changer/geometry_changer_outputs.zip>`_ to additionally check the results.
