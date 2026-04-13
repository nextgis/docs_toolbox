Vector layers in Web GIS from archive 
=========================================

This tool allows to create multiple vector layers in Web GIS at once using a ZIP archive of geodata files.

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

Launch the tool: https://toolbox.nextgis.com/t/layers2ngw

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.com/data/toolbox/empty_geoms/empty_geoms_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

.. admonition:: Related tools

   * `Vector layers from Web GIS to GeoPackage <https://toolbox.nextgis.com/t/ngw_to_gpkg?from-related-tools=1>`_