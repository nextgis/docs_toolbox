Merge two Web GIS vector layers
===============================

This tool allows you to copy data from one layer to another with the same Web GIS on NextGIS platform, including attachments and attribute values.

NextGIS Web (NGW) is a geodata managing system. You can use it for free after `signing up <https://docs.nextgis.com/docs_ngcom/source/create.html>`_. With NextGIS Web you can store geodata, create interactive online maps, give access to them to your teammates and clients, edit features directly on the map and in the feature tables, as well as process them with specialized Toolbox tools. `More on what NGW can do <https://docs.nextgis.com/docs_ngweb/source/general.html>`_.

The layer you copy features from is **source**.

The layer you want to add the features to is **target**.

Inputs:

* Source layer Web GIS address i.e.: https://sandbox.nextgis.com;
* Source Layer ID - numbers at the end of the resource URL;
* Source username - NextGIS ID or username of a user of the above Web GIS. User must have `permissions <https://docs.nextgis.com/docs_ngcom/source/permissions.html>`_ to read resource and data;
* Password for the source Web GIS user;
* Target layer Web GIS address, i.e.: https://sandbox.nextgis.com. Can be the same as the source.
* Target layer ID - numbers at the end of the resource URL;
* Target username - NextGIS ID or username of a user of the target Web GIS. User must have `permissions to create resources (write) <https://docs.nextgis.com/docs_ngcom/source/permissions.html>`_;
* Target Password - password for the taget Web GIS user.

Outputs:

* Modified layer in the target Web GIS.

Launch the tool: https://toolbox.nextgis.com/t/ngw_merge_layers

.. figure:: _static/ngw_merge_layers_input.png
   :name: ngw_merge_layers_input_pic
   :align: center
   :width: 16cm

   Example input: two layers

.. figure:: _static/ngw_merge_layers_result.png
   :name: ngw_merge_layers_result_pic
   :align: center
   :width: 16cm

   Example output: all features in the same layer

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.com/data/toolbox/ngw_merge_layers/ngw_merge_layers_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.com/data/toolbox/ngw_merge_layers/ngw_merge_layers_outputs.zip>`_ of the tool run.

.. admonition:: Related tools

   * `Duplicate Web GIS layer <https://toolbox.nextgis.com/t/ngw_copy_layer?from-related-tools=1>`_