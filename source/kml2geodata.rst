KML to geodata
==============

Convert KML, KMZ to structured geodata (GeoJSON). This tool can work with attachments (photo) and can parse structured tables added to description of the KML feature.

Inputs:

* Source data - KML or KMZ file;
* Field names - Fields of the table from the description section which should be processed. Comma-separated list, no spaces;
* Only files in the archive - If checked, the resulting GeoJSON will mention only the files that are present in the archive;
* Ignore KML extended data - If checked, lc:attachment will be ignored;
* Keep Z coordinate - If checked, Z coordinate will be preserved and PointZ/LinestringZ etc geometries will be created.

Outputs:

* ZIP-compressed GeoJSON with attachments (if any) in a folder.

Launch the tool: https://toolbox.nextgis.com/t/kml2geodata


.. todo:: _static/kml2geodata-src.png
   :align: center
   :width: 16cm
   
   Source data example. KML with attributes structured as the table in the description of a feature

.. todo:: _static/kml2geodata-res.png 
   :align: center
   :width: 16cm
   
   Result example. Data opened in QGIS after conversion with the tool

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Convert format of vector layer <https://toolbox.nextgis.com/t/convert?from-related-tools=1>`_
   * `MapInfo ready for QGIS <https://toolbox.nextgis.com/t/mapinfo2qgis?from-related-tools=1>`_
   * `DWG to DXF <https://toolbox.nextgis.com/t/import_dwg?from-related-tools=1>`_
