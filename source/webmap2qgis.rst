Web Map to QGIS project
=========================

The tool works with Web GIS data: converts vector layers and its styles from any chosen Web Map to QGIS project and GeoPackage file.

Inputs:

* Web GIS address – URL of the Web GIS on NextGIS Web platform, containing the Web Map to be converted into QGIS project. For example, ``https://demo.nextgis.com``;
* Web Map ID - numbers at the end of the Web Map URL;
* Login – NextGIS ID or username of a Web GIS user that has permissions to read the data;
* Password – password for the user;
* Extent - by default, the extent of the Web Map is used. You can enter a different extent in EPSG:4326. Format: bottom, left, top, right (South, West, North, East). Separate by comma. Example: ``54.5, 102.5, 59, 116``;
* Output format. Format in which vector layers from the Web Map will be saved:

    - Geopackage (GeoPackage)
    - GML
    - MID/MIF
    - ESRI Shapefile
    - CSV
    - DXF
    
* CRS ID - Coordinate system identifier for the output project. For standard CRS use the numbers of the EPSG code. Default is 3857. For custom CRS see the id in the `Control panel <https://docs.nextgis.com/docs_ngweb/source/ngw_srs.html#ngw-srs-id>`_ To view the list of all available codes use the following API: ``/api/component/spatial_ref_sys/``.

Outputs:

* ZIP-archive with QGIS project file (.qgs) and GeoPackage file, containing vector layers.

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/uFiOJfK6VQw?si=HK0H6sg7hhF7i7na" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch on `youtube <https://youtu.be/uFiOJfK6VQw?si=VN6jPbsW_5TSWNRY>`_.

Launch the tool: https://toolbox.nextgis.com/t/webmap2qgis

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Vector layers from Web GIS to GeoPackage <https://toolbox.nextgis.com/t/ngw_to_gpkg?from-related-tools=1>`_
   * `Web GIS structure to spreadsheet <https://toolbox.nextgis.com/t/web_gis_structure?from-related-tools=1>`_