Google Sheets to Web GIS
========================

Tool creates or updates point vector layer in NextGIS Web using Google Sheets.
Spreadsheet must contain 'lat' and 'lon' fields and be accessible for reading via shared link.
Coordinate reference system - WGS84.

Input:

*  Web GIS link, example: https://sandbox.nextgis.com.
*  Web GIS user login. User must have writing access.
*  Web GIS User password.
*  Vector layer ID to update. Use '0' to create new vector layer.
*  Resource group ID. Specify the group to upload layer to. Use only if creating a new layer.
*  Google Sheets ID (e.g. '1cKvjCMBZajaortAkdQqVwQ_06LuLm3bHyvybJgmAeQg') or URL. This link should be accessible for data reading.
*  Mode: ADD - to append data to existing layer or to create a new layer; REPLACE - to rewrite existing layer.

Output:

* Created/updated layer in Web GIS

`Google Sheets sample <https://docs.google.com/spreadsheets/d/1cKvjCMBZajaortAkdQqVwQ_06LuLm3bHyvybJgmAeQg/edit?usp=sharing>`_

`Video <https://youtu.be/mEhUaRTFl3M?si=xD8JZjZPL0qIam8F>`_

Launch tool: https://toolbox.nextgis.com/operation/Googlesheets2layer
