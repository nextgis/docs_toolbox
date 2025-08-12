Change geometry for a group of layers
=====================================

The tool changes the geometry of features in all the layers of a group in Web GIS. 

Three modes are available:

* **Delete** - the tool deletes the selected features. The selection is based on the specified values of a layer’s attribute field;
* **Add** - the tool adds new features from the uploaded ESRI Shapefile. The structures of the file and the layer must match. Otherwise, the tool will not be able to add new features;
* **Change** - the tool replaces the geometry value for features with the geometries from the uploaded Shapefile. The selection is based on the specified values of a layer’s attribute field. The attribute name in the SHP file and the Web GIS layer must match.

Inputs:

* Web GIS address. Example: https://sandbox.nextgis.com.
* Login. NextGIS ID or login of a user who has write access to the resource group;
* Password of that user;
* Group resource ID. ID of the Web GIS resource that contains the layer group;
* Source field. The name of the source field by which objects are searched.
* Mode. Select ``DELETE``, ``ADD`` or ``CHANGE``;
* Initial value. The value of the field by which objects are selected. If you need to specify multiple values, use a comma as a separator. The parameter is required in the Delete and Change modes.
* First year. Start of time range (optional).
* Last year. End of time range (optional parameter).
* Select SHP file. File upload is required in Add and Change modes.

.. note::
    Start year and end year are optional parameters. These parameters allow you to limit the time range for the selected layers. To use these parameters, you must make sure that the time ranges are indicated in the names of the layers of the Web GIS resource. For example, in layer 1245_1246_earl_v.1.0 1245 and 1246 the years are indicated. If these parameters are in use, you need to enter three or four digit values. Other parameters are **required**.

Outputs:

*  A CSV file that contains data on the selected mode, the source field and its value, a list of hyperlinks to features that have been changed. If there are errors, they will also be indicated in this file.

.. figure:: _static/geometry_changer_result.png
   :name: geometry_changer_result_pic
   :align: center
   :width: 7cm

   Report example

Launch tool: https://toolbox.nextgis.com/t/geometry_changer

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/geometry_changer/geometry_changer_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/geometry_changer/geometry_changer_outputs.zip>`_ to additionally check the results.
