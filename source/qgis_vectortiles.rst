Generate vector tiles from QGIS project
==========================================

Generate zipped vector tiles from an archive with QGIS project and data. Only the vector layers are taken from the project, no styling is applied.

Inputs:

* ZIP file containing QGIS project and data files;
* Extent. If empty, a combined extent of all layers will be used. It may unexpectedly calculate an extent of the entire planet, then the tool will take a lot of time to process. You can mark it on a map, draw it and then correct the numbers or enter the extent manually following the format 'xmin, xmax, ymin, ymax'. Enter coordinates in WGS 84 (EPSG:4326), for example ``-7.3,42.1,10.5,50.5``;
* Min zoom level - between 0 and 25, the default value is 0;
* Max zoom level - between 0 and 25, the default value is 9.

Output:

* ZIP archive with tile images in Protocolbuffer Binary Format (PBF) format organized into folders.

Launch the tool: https://toolbox.nextgis.com/t/qgis_vectortiles

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Generate raster tiles from QGIS project <https://toolbox.nextgis.com/t/qgis_rastertiles?from-related-tools=1>`_
   * `Generate tileset from raster <https://toolbox.nextgis.com/t/raster2tiles?from-related-tools=1>`_
   * `Converting a QGIS project to PDF <https://toolbox.nextgis.com/t/qgis2pdf?from-related-tools=1>`_