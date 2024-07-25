KML to geodata
==============

Convert KML, KMZ to structured geodata (GeoJSON). This tool can work with attachments (photo) and can parse structured tables added to description of the KML feature.

Inputs:

* Source data - KML or KMZ file.
* Table fieldnames - optional. Indicate table fieldnames from Description section of KML file, which should be processed. Should be listed without space and separated by comma.
* Check for files presence - if checked, the result GeoJSON will mention only the files that are present in the archive indeed.
* Ignore extended data - if checked, lc:attachment will be ignored.
* Keep Z coordinate -i f checked, Z coordinate will be preserved and PointZ/LinestringZ etc geometries will be created.

Outputs:

* ZIP compressed GeoJSON with attachments if any.

Launch tool: https://toolbox.nextgis.com/operation/kml2geodata


.. figure:: _static/kml2geodata-src.png
   :align: center
   :width: 16cm
   
   Source data example. KML with attributes structured as the table in the description of a feature

.. figure:: _static/kml2geodata-res.png 
   :align: center
   :width: 16cm
   
   Result example. Data opened in QGIS after conversion with the tool

**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/kml2geodata/kml2geodata_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/kml2geodata/kml2geodata_outputs.zip>`_ to additionally check the results.
