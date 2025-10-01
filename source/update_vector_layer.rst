Update Web GIS layer from CSV
=================================

Update an existing Web GIS layer using uploaded CSV file. Works only with point vector layers. It is possible either to add data to existing one or to replace existing features.
Data structure of CSV file should be the same as of target Web GIS layer. 

Inputs:

* Web GIS address. Example: https://sandbox.nextgis.com;
* Login. NextGIS ID or Web GIS user login;
* Password. User password;
* Vector layer resource ID. Numbers at the end of the layer resource URL. For instance, corresponding number for resource “Matter levels” is 5150 since its address is https://demo.nextgis.com/resource/5150.;
* Delimiter. Specify delimiter in uploaded CSV-file, e.g. ``,`` (comma)
* Mode. Use ``Add`` to add to the data and ``Replace`` to completely replace existing data;
* Skip frist lines. Number of lines to skip before CSV header;
* Choose CSV file. Point file with coordinates in *.CSV format. Fields with latitude and longitude should be named ``lat`` and ``lon``, respectively. Coordinates should be in WGS84 (EPSG:4326). If the table contains dates, they must be written in `ISO <https://docs.python.org/3/library/datetime.html#datetime.datetime.isoformat>`_ format, for example, 2019-05-18T15:17:08.132263.

Outputs:

* Updated vector layer in Web GIS.
* CSV report, showing ID of the updated layer, selected mode, number of uploaded features and hyperlink to updated layer in Web GIS.

Troubleshooting

* Invalid type error - incorrect resource ID. Specify the ID of the vector layer resource, not that of the resource group containing the layer.
* Invalid type of the layer - incorrect layer type. Only vector layers can be used.
* Invalid operation mode - incorrect mode. You can only type in Replace or Add. 
* Invalid geometry type - target layer geometry is not point.
* Invalid structure of the layer - data structures of CSV and target layer do not match.

Launch the tool: https://toolbox.nextgis.com/t/update_vector_layer

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/update_vector_layer/update_vector_layer_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/update_vector_layer/update_vector_layer_outputs.zip>`_ to additionally check the results.

.. admonition:: Related tools

   * `Join layer and table by field <https://toolbox.nextgis.com/t/join_by_field>`_
   * `Spatial Join (Join by location) <https://toolbox.nextgis.com/t/spatial_join>`_