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

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/kml2geodata/kml2geodata_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/kml2geodata/kml2geodata_outputs.zip>`_ to additionally check the results.
