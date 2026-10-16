Add points to Web GIS layer from table
======================================

Update an existing Web GIS layer on NextGIS platform using uploaded CSV, XLS or XLSX file. Works only with point vector layers. It is possible to either add data or to replace existing features completely. Data structure of the input file should be the same as of target Web GIS layer.

NextGIS Web (NGW) is a geodata managing system. You can use it for free after `signing up <https://docs.nextgis.com/docs_ngcom/source/create.html>`_. With NextGIS Web you can store geodata, create interactive online maps, give access to them to your teammates and clients, edit features directly on the map and in the feature tables, as well as process them with specialized Toolbox tools. `More on what NGW can do <https://docs.nextgis.com/docs_ngweb/source/general.html>`_.

Inputs:

* Choose CSV, XLS or XLSX file with coordinates. Coordinates should be in WGS84 (EPSG:4326). If the table contains dates and you need them to be recognized as DATETIME they must be written in `ISO <https://docs.python.org/3/library/datetime.html#datetime.datetime.isoformat>`_ format, for example, 2019-05-18T15:17:08.132263.
* Web GIS address. Example: https://sandbox.nextgis.com;
* Login. NextGIS ID or Web GIS user login;
* Password. User password;
* Vector layer resource ID. Number at the end of the layer resource URL.
* Mode. Use ``ADD`` to add to the data or ``REPLACE`` to completely replace existing data;
* Delimiter. Specify delimiter in uploaded CSV-file, e.g. ``;`` (semicolon). Optional value for CSV input, default is comma;
* Latitude column. Specify latitude column name. Optional value, default is lat;
* Longitude column. Specify longitude column name. Optional value, default is lon;
* Skip first lines. Number of lines to skip before CSV header. Optional value, default is 0 (no skipping);


Outputs:

* Updated vector layer in Web GIS.
* CSV report, showing ID of the updated layer, selected mode, number of uploaded features and hyperlink to updated layer in Web GIS.

Troubleshooting

* Invalid type error - incorrect resource ID. Specify the ID of the vector layer resource, not that of the resource group containing the layer.
* Invalid type of the layer - incorrect layer type. Only vector layers can be used.
* Invalid geometry type - target layer geometry is not point.

Launch the tool: https://toolbox.nextgis.com/t/update_vector_layer

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Join layer and table by field <https://toolbox.nextgis.com/t/join_by_field?from-related-tools=1>`_
  * `Spatial Join (Join by location) <https://toolbox.nextgis.com/t/spatial_join?from-related-tools=1>`_
