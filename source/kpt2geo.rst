Convert EGRN KPT to geodata
===========================

.. figure:: _static/kpt2geo.png
   :align: center
   :width: 16cm

   Initial and resulting data
   
The tool converts one or several Rosreestr KPT from XML format into a convenient geodata format with a GIS project.

Inputs:

*  Zip archive with zip archives of Rosreestr downloads (archive of archives with the name format Response-80-105152635.zip)
*  Output geodata format - GeoJSON, ESRI Shape, Mapinfo TAB

Outputs:

* zip archive with the QGIS project and geodata

The archive contains directories: a geodata directory in the local coordinate system (msk), a geodata directory in EPSG: 4326 (wgs) and a project for QGIS with data in EPSG: 4326 with the design.

A description of the layers is given at https://data.nextgis.com/en/cadastre/#region-layers

Launch tool: https://toolbox.nextgis.com/operation/pkk_kpt

Download an example of initial data and calculation results: https://nextgis.ru/data/toolbox/kpt2geo/kpt2geo.zip
