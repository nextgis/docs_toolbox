Update a Web GIS layer from a CSV
=================================

Update an existing Web GIS layer using uploaded CSV file. Works only with point vector layers. It is possible either to add data to existing one or to replace existing features.
Data structure of CSV file should be the same as of target Web GIS layer. 

Inputs:

* Web GIS address - Your Web GIS URL, e.g. https://demo.nextgis.com.
* Login - Web GIS user login.
* Password - Web GIS user password.
* Vector layer ID - Please specify the number corresponding to the target layer, you can find it in address bar of the browser. For instance, corresponding number for resource “Matter levels” is 5150 since its address is https://demo.nextgis.com/resource/5150.
* CSV file - file with coordinates of the points. Fields with latitude and longitude should be named lat and lon, respectively. Coordinates should be in WGS84 (EPSG:4326). If the table contains dates, they must be written in `ISO <https://docs.python.org/3/library/datetime.html#datetime.datetime.isoformat>`_ format, for example, 2019-05-18T15:17:08.132263.
* CSV separator - symbol used to separate values in CSV file, for example, ; (semicolon). 
* Mode - Use Add to add features to already existing ones, and Replace to completely replace existing data. Case-insensitive.

Outputs:

* Updated vector layer in Web GIS.
* CSV report, showing ID of the updated layer, selected mode, number of uploaded features and hyperlink to updated layer in Web GIS.

Troubleshooting

* Invalid type error - incorrect resource ID. Specify vector layer resource ID, not resource group containing the layer.
* Invalid type of the layer - incorrect layer type. Only vector layers can be used.
* Invalid operation mode - incorrect mode. You can only type in Replace or Add. 
* Invalid geometry type - target layer geometry is not point.
* Invalid structure of the layer - data structures of CSV and target layer mismatch.

Launch tool: https://toolbox.nextgis.com/operation/update_vector_layer

**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/update_vector_layer/update_vector_layer_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/update_vector_layer/update_vector_layer_outputs.zip>`_ to additionally check the results.
