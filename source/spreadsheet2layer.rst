Google Sheets to Web GIS
========================

Tool creates or updates point vector layer in NextGIS Web using Google Sheets.
Spreadsheet must be accessible for reading via shared link.

There are two ways to store coordinates for this tool:

1. Coumns 'lat' and 'lon', Coordinate reference system - WGS84.
2. Google maps links to locations.

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

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/mEhUaRTFl3M?si=N8n7IOYa65xmcVSv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch the video on `youtube <https://youtu.be/mEhUaRTFl3M>`_.

Launch tool: https://toolbox.nextgis.com/operation/spreadsheet2layer

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/spreadsheet2layer/spreadsheet2layer_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/spreadsheet2layer/spreadsheet2layer_outputs.zip>`_ to additionally check the results.
