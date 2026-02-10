Copy nextgis.com resource group with data
===========================================

Copies structure+data of resource group on NextGIS platform to other resourse group or Web GIS. Copies the data, subgroups, styles and Web Maps with layers added. The following resource types are supported: 

* resource group;
* vector layer;
* QGIS style;
* Web Map.

Inputs:

* Source Web GIS address. URL of your Web GIS, e.g. https://demo.nextgis.com and login/password if necessary
* Source group ID. Source Web GIS group resource number
* Destination Web GIS address. URL of your Web GIS, e.g. https://demo.nextgis.com and login/password if necessary
* Destination group ID. Web GIS group resource number in destination instance, where group will be created
* Do not copy data. Create only empty layers with attributes and styles

Outputs:

* New resource group in the target Web GIS.

Launch the tool: https://toolbox.nextgis.com/t/ngw_copy_group

Example:

.. todo:: _static/ngw_copy_group_input_en.png
   :name: ngw_copy_group_input_pic
   :align: center
   :width: 16cm

   Example input

.. todo:: _static/ngw_copy_group_result_en.png
   :name: ngw_copy_group_result_pic
   :align: center
   :width: 16cm

   Example output

**Try the tool in action by downloading our example:**

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.
