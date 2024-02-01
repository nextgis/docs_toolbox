KML to geodata
==============

Convert KML, KMZ to structured geodata (GeoJSON). This tool can work with attachments (photo) and can parse structured tables added to description of the KML feature.

Inputs:

* Input dataset in KML/KMZ format.
* NextGIS Drive ID or link (if you have access)
* Table fields. Comma-separated list of table field names to be extracted from the description.
* Check files presence. If checked, the result will contain only the files that are present in the archive.
* Ignore extended data. If checked, lc:attachment will be ignored.
* Keep Z coordinate. If checked, Z coordinate will be preserved and PointZ/LinestringZ etc geometries will be created.

Outputs:

* ZIP compressed GeoJSON with attachments if any.

Download an example of source data and result: https://nextgis.ru/data/toolbox/kml2geodata/kml2geodata.zip

Launch tool: https://toolbox.nextgis.com/operation/kml2geodata


.. figure:: _static/kml2geodata-src.png
   :align: center
   :width: 16cm
   
   Source data example. KML with attributes structured as the table in the description of a feature

.. figure:: _static/kml2geodata-res.png 
   :align: center
   :width: 16cm
   
   Result example. Data opened in QGIS after conversion with the tool
