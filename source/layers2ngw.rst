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

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Vector layers from Web GIS to GeoPackage <https://toolbox.nextgis.com/t/ngw_to_gpkg?from-related-tools=1>`_