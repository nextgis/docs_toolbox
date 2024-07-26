Photos with EXIF to NGW layer
=============================

Convert a set of georeferenced photos with EXIF tags into NextGIS Web vector layer.

Input:

*  A set of photos as a ZIP file. No subfolders, no extra files - only photos.
*  Web GIS link, example: https://sandbox.nextgis.com
*  administrator or other Web GIS user login. User must have writing access
*  User password
*  Resource ID where layer will be created. Default is 0, layer will be created in the Main resource group.

Output:

* New vector layer where each photo is represented by point. The same photo is added as an attachment to this point.

Launch tool: https://toolbox.nextgis.com/operation/exif2resource


Result on the web map: https://demo.nextgis.com/resource/5950/display?panel=info

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/exif2resource/exif2resource_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

