Vector files from Web GIS to GeoPackage
=======================================

The tool agglomerates all vector layers from the target resource group in Web GIS into one GeoPackage file, available for download.

Input:

* Web GIS address - Full URL, e.g. https://demo.nextgis.com.
* Login - Login for Web GIS user.
* Password - Password for Web GIS user.
* ID of resource group - ID of the group, whithin which the search of all vector layers will be performed, including embedded folders (resource groups). ID could be find in address bar on the webpage of the resource group. E.g. for https://demo.nextgis.com/resource/4332 ID of the resource group is 4332. 

Output:

* GeoPackage file with all vector layers. CRS - WGS 84, attributes will be in UTF-8 encoding. 

Launch tool: https://toolbox.nextgis.com/operation/ngw_to_gpkg
