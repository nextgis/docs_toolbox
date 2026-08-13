Field combiner
==============

Concatenates values of several fields and writes it to the target field.

Inputs:

* Web GIS address. URL of your Web GIS, e.g. https://demo.nextgis.com and login/password if necessary;
* Layer ID. Numbers at the end of the layer's URL;
* Source field 1. Name of the attribute containing the 1st part, e.g. 'id_prefix';
* Source field 2. Name of the attribute containing the 1st part, e.g. 'id_date';
* Source field 3. Name of the attribute containing the 1st part, e.g. 'id_suffix';
* Target field. Name of the field to store the combined value, e.g. 'id_combined';
* Order custom name. Custom name for the order (optional).

Outputs:

* Сhanged vector layer in Web GIS.

Launch the tool: https://toolbox.nextgis.com/t/field_combiner

Example:

.. todo:: _static/field_combiner_input_en.png
   :name: field_combiner_input_pic
   :align: center
   :width: 20cm

   Example input

.. todo:: _static/field_combiner_result_en.png
   :name: field_combiner_result_pic
   :align: center
   :width: 20cm

   Example output


**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.
