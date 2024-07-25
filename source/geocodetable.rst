Geocode a table
===============

The tool processes addresses from a CSV file and adds its coordinates back to the file. A relevant geocoding license is needed.

Inputs:

*  Source data - CSV file with a list of addresses. First row should contain field names. File should be in UTF-8 encoding.
*  Field with address - name of the field that contains addresses in a source CSV file.
*  Geocoder - specify one of the two available geocoder providers: Google. Case insensitive. 
*  API key - API key to run chosen geocoder.

.. note::
    **How to get a geocoder API key**

    Google Geocoding API - https://developers.google.com/maps/documentation/geocoding/usage-and-billing


**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/geocodetable/geocodetable_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/geocodetable/geocodetable_outputs.zip>`_ to additionally check the results.
Outputs:

*  CSV file, containing two additional columns with latitude and longitude besides original data.

Launch the tool: https://toolbox.nextgis.com/operation/geocodetable
