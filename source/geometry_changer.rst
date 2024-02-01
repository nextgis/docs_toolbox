Change geometry for a group of layers
=====================================

The tool changes the geometry of features in a layer group of the Web GIS resource. The change is possible in 3 modes: Delete, Insert, Replace. In delete mode, the tool deletes the selected features. The selection is based on the specified values of a layer’s attribute field. In insert mode, the tool adds new features from the uploaded shp file, the structure of the file and the layer must match. Otherwise, the tool will not be able to add new features. 
In replacement mode, the tool replaces the geometry value for features from the uploaded shp file, the values of the specified attribute of which match with the attribute values of the Web GIS layer. The attribute name in the shp file and the Web GIS layer must match.

Inputs:

* Web GIS Address — The URL of your Web GIS (http (s): //***.nextgis.com)
* Login - The username of the user who has the permission to write data to the specified resource
* Password - Web GIS user password
* Resource Group Identifier - Web GIS Resource Identifier for a layer group
* Initial field - Name of the initial field used to search for features
* Mode - A type of mode, which changes the geometry of features. To delete features, select the Delete mode, to Add - insert, to Change - replace
* Initial value - The value of the field by which the features are selected. If you need to specify multiple values, use a comma to separate
* Start year - Starting date of the time range (optional parameter)
* End year - Ending date of the time range (optional parameter)
* SHP file - An ESRI Shapefile (zipped) that contains features. Required parameter in Add and Change modes

.. note::
    Start year and end year are optional parameters. These parameters allow you to limit the time range for the selected layers. To use these parameters, you must make sure that the time ranges are indicated in the names of the layers of the Web GIS resource. For example, in layer 1245_1246_rus_earl_v.1.0 1245 and 1246 the years are indicated. If these parameters are in use, you need to enter three or four digit values. Other parameters are **mandatory**.

Outputs:

*  A CSV file that contains data on the selected mode, the source field and its value, a list of hyperlinks to features that have been changed, in case of errors they will also be indicated in this file.

.. figure:: _static/geometry_changer.PNG
   :align: center
   :width: 16cm

   Launch tool: https://toolbox.nextgis.com/operation/geometry_changer
