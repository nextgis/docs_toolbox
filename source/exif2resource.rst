Photos with EXIF to NGW layer
=============================

Convert a set of georeferenced photos with EXIF tags into NextGIS Web point vector layer. You can also add photos to an existing point layer.

Input:

*  A set of photos as a ZIP file. No subfolders, no extra files - only photos.
*  Web GIS link, example: https://sandbox.nextgis.com
*  administrator or other Web GIS user login. User must have writing access
*  User password
*  Parent ID - ID of the folder where layer will be created. Default is 0, layer will be created in the Main resource group.

or

* Layer ID - ID of an existing layer, the photos will be added to this layer.
* Working mode: set to ADD to add points to the layer alongside the existing ones or REPLACE to delete existing points and add new ones.

Also you can create an additional field storing some information, for example, the author of the photos.

* Additional attribute - Name of the attribute field to store a custom value
* Additional field value - A text string to add to each new feature


Output:

* Vector layer where each photo corresponds to a point. The same photo is added as an attachment to this point.

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/r5v0wzOufV8?si=VIIy1yaVWmXAtxLI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


Watch the video on `youtube <https://youtu.be/r5v0wzOufV8>`_.


Launch the tool: https://toolbox.nextgis.com/t/exif2resource


Result on the web map: https://demo.nextgis.com/resource/5950/display?panel=info

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/exif2resource/exif2resource_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

