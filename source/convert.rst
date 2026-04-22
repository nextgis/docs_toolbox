Конвертация векторных слоёв
===========================

Конвертация векторных слоёв между разными форматами файлов.


На входе:

*  Векторный слой. Одиночный файл или ZIP-архив с одним векторным слоем любого формата, поддерживаемого библиотекой GDAL, например GeoPackage или архив с ESRI Shapefile. `Список поддерживаемых исходных форматов <https://docs.nextgis.ru/docs_toolbox/source/convert.html#format-list>`_.
*  Название выходного формата: ESRI Shapefile, MapInfo TAB, GeoJSON, GPKG, DXF, FlatGeobuf.

.. note::
   Если загрузить в инструмент файл неподходящего формата (например, SQL или одиночный файл SHP), появится сообщение об ошибке.

На выходе:

* ZIP архив с векторным слоем. 

Система координат не изменяется. 

Если конвертация в ESRI Shapefile, то атрибуты конвертируются в UTF-8. У остальных форматов кодировка не изменяется, подразумевается что их создатели уже создают их в UTF-8.

Запуск инструмента: https://toolbox.nextgis.com/t/convert

**Попробуйте инструмент в действии**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. _format_list:

Список поддерживаемых форматов исходных файлов
------------------------------------------------------

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
* MapInfo File -  MapInfo TAB and MIF/MID
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


   
.. seealso::

   * `Перепроецирование координат <https://toolbox.nextgis.com/t/coord_recalc?from-related-tools=1>`_
   * `Проверка геометрии <https://toolbox.nextgis.com/t/check_geometries?from-related-tools=1>`_
   * `KML в геоданные <https://toolbox.nextgis.com/t/kml2geodata?from-related-tools=1>`_
   * `MapInfo в GeoPackage <https://toolbox.nextgis.com/t/mapinfo2qgis?from-related-tools=1>`_

   
