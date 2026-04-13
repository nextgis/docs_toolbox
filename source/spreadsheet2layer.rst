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
*  Vector layer ID to update. Leave blank to create new vector layer.
*  Resource group ID. Specify the group to upload layer to. Use only if creating a new layer.
*  Google Sheets ID (e.g. '1cKvjCMBZajaortAkdQqVwQ_06LuLm3bHyvybJgmAeQg') or URL. This link should be accessible for data reading.
*  Mode: by default the tool appends data to existing layer or creates a new layer (ADD mode); select REPLACE to overwrite an existing layer (ID specified above).

Output:

* Created/updated layer in Web GIS

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/mEhUaRTFl3M?si=N8n7IOYa65xmcVSv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch the video on `youtube <https://youtu.be/mEhUaRTFl3M>`_.

Launch the tool: https://toolbox.nextgis.com/t/spreadsheet2layer

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Table to vector file <https://toolbox.nextgis.com/t/table2geo?from-related-tools=1>`_
