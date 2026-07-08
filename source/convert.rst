Convert format of vector layer
==============================

Convert vector layer to other file format.

Coordinate refrence system (CRS) is not changing.
If output format is ESRI Shapefile, encoding of attributes cast to UTF-8.

Input:

*  Vector layer file or ZIP archive compatible with GDAL library. `List of supported formats <https://docs.nextgis.com/docs_toolbox/source/convert.html#format-list>`_
*  Name of output format: ESRI Shapefile, MapInfo TAB, GeoJSON, GPKG, DXF, FlatGeobuf.

.. note::
   If uploaded file has incompatible format (for example, single SHP file) an error message will appear.

Output:

* ZIP archive with vector layers

Launch the tool: https://toolbox.nextgis.com/t/convert

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. _format_list:

Supported input formats
-----------------------

* ADBC -  Arrow Database Connectivity
* AIVector -  Artificial intelligence powered vector driver
* AmigoCloud -  AmigoCloud
* Arrow -  (Geo)Arrow IPC File Format / Stream
* AVCBIN -  Arc/Info Binary Coverage
* AVCE00 -  Arc/Info E00 (ASCII) Coverage
* CAD -  AutoCAD DWG
* CARTO -  Carto
* CSV -  Comma Separated Value (.csv)
* CSW -  OGC CSW (Catalog Service for the Web)
* DGN -  Microstation DGN
* DGNv8 -  Microstation DGN v8
* DWG -  AutoCAD DWG
* DXF -  AutoCAD DXF
* EDIGEO -  EDIGEO
* EEDA -  Google Earth Engine Data API
* Elasticsearch -  Elasticsearch: Geographically Encoded Objects for Elasticsearch
* ESRI Shapefile -  ESRI Shapefile / DBF
* ESRIJSON -  ESRIJSON / FeatureService driver
* FileGDB -  ESRI File Geodatabase (FileGDB)
* FlatGeobuf -  FlatGeobuf
* GDALG -  GDALG: GDAL Streamed Algorithm
* GeoJSON -  GeoJSON
* GeoJSONSeq -  GeoJSONSeq: sequence of GeoJSON features
* GeoRSS -  GeoRSS : Geographically Encoded Objects for RSS feeds
* GML -  Geography Markup Language
* GMLAS -  Geography Markup Language (GML) driven by application schemas
* GMT -  GMT ASCII Vectors (.gmt)
* GPKG -  GeoPackage vector
* GPSBabel -  GPSBabel
* GPX -  GPS Exchange Format
* GRASS -  GRASS Vector Format
* GTFS -  General Transit Feed Specification
* HANA -  SAP HANA
* IDB -  IDB
* IDRISI -  Idrisi Vector (.VCT)
* INTERLIS 1 -  "INTERLIS 1" and "INTERLIS 2" drivers
* JML -  JML: OpenJUMP JML format
* JSONFG -  OGC Features and Geometries JSON
* KML -  Keyhole Markup Language
* LIBKML -  LIBKML Driver (.kml .kmz)
* LVBAG -  Dutch Kadaster LV BAG 2.0 Extract
* MapInfo TAB -  MapInfo TAB and MIF/MID
* MapML -  MapML
* MEM -  In Memory datasets
* Memory -  Memory (deprecated)
* MiraMonVector -  MiraMon Vector
* MongoDBv3 -  MongoDBv3
* MSSQLSpatial -  Microsoft SQL Server Spatial Database
* MVT -  MVT: Mapbox Vector Tiles
* MySQL -  MySQL
* NAS -  ALKIS
* netCDF -  NetCDF: Network Common Data Form - Vector
* NGW -  NextGIS Web
* OAPIF -  OGC API - Features
* OCI -  Oracle Spatial
* ODBC -  ODBC RDBMS
* ODS -  Open Document Spreadsheet
* OpenFileGDB -  ESRI File Geodatabase vector (OpenFileGDB)
* OSM -  OpenStreetMap XML and PBF
* Parquet -  (Geo)Parquet
* PDF -  Geospatial PDF
* PDS -  Planetary Data Systems TABLE
* PGDump -  PostgreSQL SQL Dump
* PGeo -  ESRI Personal GeoDatabase
* PLScenes -  PLScenes (Planet Labs Scenes/Catalog API)
* PMTiles -  PMTiles
* PostgreSQL -  PostgreSQL / PostGIS
* S57 -  IHO S-57 (ENC)
* Selafin -  Selafin files
* SOSI -  Norwegian SOSI Standard
* SQLite -  SQLite / Spatialite RDBMS
* SXF -  SXF
* TileDB -  TileDB vector
* TopoJSON -  TopoJSON driver
* VDV -  VDV-451/VDV-452/INTREST Data Format
* VFK -  Czech Cadastral Exchange Data Format
* VRT -  OGR Virtual Format
* WAsP -  WAsP .map format
* WFS -  OGC WFS service
* XLS -  MS Excel format
* XLSX -  MS Office Open XML spreadsheet
* XODR -  OpenDRIVE Road Description Format


.. admonition:: Related tools

  * `Reproject coordinates <https://toolbox.nextgis.com/t/coord_recalc?from-related-tools=1>`_
  * `Check geometries <https://toolbox.nextgis.com/t/check_geometries?from-related-tools=1>`_
  * `KML to geodata <https://toolbox.nextgis.com/t/kml2geodata?from-related-tools=1>`_
  * `MapInfo ready for QGIS <https://toolbox.nextgis.com/t/mapinfo2qgis?from-related-tools=1>`_
