Vector layers from Web GIS to GeoPackage
========================================

The tool agglomerates all vector layers from the target resource group in Web GIS into one GeoPackage file, available for download.

Input:

* Web GIS address - Full URL, e.g. https://demo.nextgis.com.
* Login - Login for Web GIS user.
* Password - Password for Web GIS user.
* ID of resource group - ID of the group, whithin which the search of all vector layers will be performed, including embedded folders (resource groups). ID could be find in address bar on the webpage of the resource group. E.g. for https://demo.nextgis.com/resource/4332 ID of the resource group is 4332. 

Output:

* GeoPackage file with all vector layers. CRS - WGS 84, attributes will be in UTF-8 encoding. 

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/mp0Z4OTp4Ho?si=xpNnAcoTAVfNHfAK" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch the video on `youtube <https://youtu.be/mp0Z4OTp4Ho?si=QY41ZFrHMQla22k7>`_.

Launch the tool: https://toolbox.nextgis.com/t/ngw_to_gpkg

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/ngw_to_gpkg/ngw_to_gpkg_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/ngw_to_gpkg/ngw_to_gpkg_outputs.zip>`_ to additionally check the results.

.. admonition:: Related tools

   * `Web Map into QGIS project <https://toolbox.nextgis.com/t/webmap2qgis>`_