Photos with EXIF to NGW layer
=============================

Convert a set of georeferenced photos with EXIF tags into NextGIS Web point vector layer. You can also add photos to an existing point layer.

NextGIS Web (NGW) is a geodata managing system. You can use it for free after `signing up <https://docs.nextgis.com/docs_ngcom/source/create.html>`_. With NextGIS Web you can store geodata, create interactive online maps, give access to them to your teammates and clients, edit features directly on the map and in the feature tables, as well as process them with specialized Toolbox tools. `More on what NGW can do <https://docs.nextgis.com/docs_ngweb/source/general.html>`_.

Input:

* Photos. ZIP archive containing photos with EXIF tags. No subfolders, no extra files - only photos;
* Web GIS link. NextGIS Web GIS link, e.g.: https://sandbox.nextgis.com
* Login. NextGIS ID or Web GIS user login. User must have permission to write data.
* Password. Password for the user above
* Group ID. Numbers at the end of the resource group URL. Default is 0, layer will be created in the Main resource group (root).
* Layer ID. To add photos to an existing layer, enter the numbers at the end of its URL
* Mode. Working mode: set to ADD to add points to existing ones or REPLACE to wipe existing points and add new ones.

Also you can create an additional field storing some information, for example, the author of the photos:

* Additional attribute. Name of the attribute field to store a custom value
* Additional field value. A text string to add to each new feature


Output:

* Vector layer where each photo corresponds to a point. The same photo is added as an attachment to this point.

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/r5v0wzOufV8?si=VIIy1yaVWmXAtxLI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


Watch the video on `youtube <https://youtu.be/r5v0wzOufV8>`_.


Launch the tool: https://toolbox.nextgis.com/t/exif2resource


Result on the web map: https://demo.nextgis.com/resource/5950/display?panel=info

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/exif2resource/exif2resource_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

