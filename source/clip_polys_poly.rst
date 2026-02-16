Calculate areas of intersection
==========================================

Calculates area of polygons inside and outside given boundary. Records results in hectares (ha) to the attributes of a vector layer in Web GIS on NextGIS platform.

NextGIS Web (NGW) is a geodata managing system. You can use it for free after `signing up <https://docs.nextgis.com/docs_ngcom/source/create.html>`_. With NextGIS Web you can store geodata, create interactive online maps, give access to them to your teammates and clients, edit features directly on the map and in the feature tables, as well as process them with specialized Toolbox tools. `More on what NGW can do <https://docs.nextgis.com/docs_ngweb/source/general.html>`_.

Inputs:

* Web GIS URL - URL of a NextGIS Web instance. Example: https://sandbox.nextgis.com;
* Login - NextGIS ID or username of a user who has write access to the resource group;
* Password;
* Boundary layer ID - ID of the boundary polygon layer in Web GIS;
* Polygons layer ID - ID of a layer with polygon features in Web GIS;
* Area field - attribute in the features layer where the area of the features will be stored;
* Area field (within boundary) - attribute in the features layer where the area of features falling within the boundary will be stored.

Outputs:

* Modified layer in Web GIS.

Launch the tool: https://toolbox.nextgis.com/t/clip_polys_poly

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.com/data/toolbox/clip_polys_poly/clip_polys_poly_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

.. admonition:: Related tools

   * `Intersector <https://toolbox.nextgis.com/t/ngw_intersect?from-related-tools=1>`_
   * `Polygon intersection <https://toolbox.nextgis.com/t/vectorclip?from-related-tools=1>`_