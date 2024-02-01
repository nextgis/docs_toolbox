Change attributes in the layer group
====================================

The tool changes the value of the target attribute for the selected features in the layer group in the specified Web GIS resource. Features are selected according to the set value of the selected field.

Inputs:

* Web GIS Address — The URL of your Web GIS (http(s): //***.nextgis.com)
* Login - The username of the user who has the permission to write data to the specified resource
* Password - Web GIS user password
* Resource Group Identifier - Web GIS Resource Identifier that contains layer groups
* Initial field - the name of the initial field used to search for features
* Initial value - The value of the field used to select features (identifier)
* Target field - The name of the target field, which values you want to change
* Target Value - The attribute value, which will be applied
* Start year - Starting date of the time range (optional parameter)
* End year - Ending date of the time range (optional parameter)

.. note::
    Start year and end year are optional parameters. These parameters allow you to limit the time range for the selected layers. To use these parameters, you must make sure that the time ranges are indicated in the names of the layers of the Web GIS resource. For example, in layer 1245_1246_rus_earl_v.1.0 1245 and 1246 the years are indicated. If these parameters are in use, you need to enter three or four digit values. Other parameters are **mandatory**.

Outputs:

*  A CSV file that contains data about the initial and target fields, the identifier value, the previous and new values ​​of the target field, as well as a list of hyperlinks to features that have been changed.

.. figure:: _static/result.PNG
   :align: center
   :width: 16cm

   An example of the result of the tool’s usage

Launch tool: https://toolbox.nextgis.com/operation/field_value_changer

Resource group example: https://demo.nextgis.com/resource/4793

Example of initial data:

* Web gis address = https://demo.nextgis.com
* Login = *****
* Password = *****
* Resource Group Id = 4793
* Initial field = fid
* Initial value = 1216
* Target field = fid2
* Target valuе = 1112
* Start Year = 1244
* End Year = 1300
