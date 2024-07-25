Web GIS structure into spreadsheet
==================================

Creates XLSX spreadsheet with a Web GIS structure (a list of resources).

Inputs:

* Full Web GIS address (URL), e.g. https://les.nextgis.com
* Web GIS user login
* Password for Web GIS user
* Resource type – specify the type of the resource for filtering data within your Web GIS. 

Possible type options:

#. all – all resources from Web GIS

#. resource_group – resource group (directory)

#. postgis_layer – PostGIS layer

#. wmsserver_service – WMS service

#. baselayers – basemap

#. postgis_connection – PostGIS connection

#. webmap – web map

#. wfsserver_service – WFS service

#. vector_layer – vector layer

#. raster_layer – raster layer

#. mapserver_style – MapServer style

#. qgis_vector_style – QGIS vector style

#. raster_style – raster style

#. file_bucket

#. lookup_table – lookup table

#. wmsclient_layer – WMS layer

#. wmsclient_connection – WMS connection

#. formbuilder_form - form

#. trackers_group – trackers group

#. tracker - tracker

#. collector_project – Collector project


Output:

* XLSX spreadsheet with the list of selected resources from Web GIS.

Launch tool: https://toolbox.nextgis.com/operation/web_gis_structure

**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/web_gis_structure/web_gis_structure_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/web_gis_structure/web_gis_structure_outputs.zip>`_ to additionally check the results.
