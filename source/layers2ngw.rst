Vector layers from an archive to Web GIS 
=========================================

Input:

* Web GIS - URL of the Web GIS, i.e. https://sandbox.nextgis.com
* Username
* Password
* Resource group ID - Number at the end of the link to the folder. For Main resource group ID=0
* ZIP archive - ZIP archive with GPKG, SHP or GeoJSON files. May contain sidecar QML file. May include subfolders.
* QML file - QML file of a style that will be added to all the loaded layers. Make sure the geometry type is correct.
* Optional: Notify on completion by email

Output:

* Layers created in NextGIS Web in the selected resource group

Launch tool: https://toolbox.nextgis.com/t/layers2ngw

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/layers2ngw/layers2ngw_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/layers2ngw/layers2ngw_outputs.zip>`_ to additionally check the results.
