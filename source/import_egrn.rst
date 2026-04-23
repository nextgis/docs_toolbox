EGRN data import
================

Convert official cadaster documents from EGRN into geodata package. Supports batch mode.

Supported formats: KPT (cadastral register): extract_cadastral_plan_territory_v01 and KPT_v10, KVZU (cadastral excerpt): KVZU_v07, construction: KVOKS_v03.


Inputs:

* Source file - XML file or ZIP archive, containing a batch of XML. Subarchives are supported.
* Source CRS (optional) - proj4, WKT or EPSG code string.
* Data format - output data format, GPKG, GeoJSON, ESRI Shapefile or MapInfo TAB. If left blank, GPKG will be used.
* Identifier - Prefix for output files.
* Target crs (optional) - proj4, WKT or EPSG code string.
* Merge datasets - Merge layers of same type derived from different XML files (initial result of conversion will also be preserved). We do not recommend this option for MapInfo TAB format.
* Merge not recognized CRS - if ticked, merges all layers of the same geometry type with unrecognized CRS into one.
* Ignore objects without geometry - Skip entries in the XML documents that don't have geometry (coordinates).
* Remove empty attributes - Attributes that have no data even for a one object will be removed.
* Convert additional data - Sometimes XML docs have a special section ReestrExtract, containing additional information, e.g. ownership. If the option is enabled, such data will be added to separate layers without geometry.

Outputs:

* ZIP archive, containing converted files. 

Launch the tool: https://toolbox.nextgis.com/t/import_egrn

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.
