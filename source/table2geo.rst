Table to vector file
====================

The tool converts spreadsheet file (XLSX, ODS, CSV) to a vector file in a format of your choice.

Input:

*  Spreadsheet file in ODS, XSLX or CSV format. Spreadsheet must be located on the first page (if input file format implies books) and contain fields "lat" and "lon" for latitude and longitude, respectively. Coordinate reference system - WGS84. Coordinates should be expressed as decimal degrees.
*  Optional: format of an output vector file. Choose one from ESRI SHAPEFILE, GEOPACKAGE, GEOJSON, TAB, MIF, SQL, CSV (in any letter case). Whith a blank field, an ESRI SPAPEFILE will be used by default.
*  Optional: field type - list of field types for an output vector file, which correspond to the columns from initial spreadsheet. Should be specified without quotes and be comma separated. Possible types: Integer, Real, String, Date (YYYY-MM-DD), Time (HH:MM:SS), DateTime (YYYY-MM-DD HH:MM:SS). Example: Integer,Real,Real,String,String,String.

Output:

* ZIP-archive with vector file. You can import this file into NextGIS QGIS or NextGIS Web without unpacking.

Input data :download:`sample <files/table2geo_example.xlsx>`.

Launch tool: https://toolbox.nextgis.com/operation/table2geo
