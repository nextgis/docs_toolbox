Get the contribution activity for the resource
==============================================

Get user activity report for a resource from the NextGIS Web server.

Works for one of the following resource types: 

* vector layer - you'll get user activity for a particular layer;
* resource group - all versioned vector layers within this group are analyzed;
* Web Map - all versioned layers added to the map are analyzed.



Inputs:

* NGW URL - Web GIS address (e.g., https://demo.nextgis.com);
* Login - NextGIS ID or user login;
* Password - password for that user;
* Resource ID - numbers at the end of the resource URL;
* Start time - optional. First day of the period, in YYYY-mm-dd format;
* End time - optionsl. Last day of the period, in YYYY-mm-dd format, not less than 28 days and not over 366 days from the initial date;
* Report language - language to generate report in.

Outputs:

* HTML file with an interactive activity report.

Launch the tool: https://toolbox.nextgis.com/t/ngw_contribution_activity

Example:

.. figure:: _static/ngw_contribution_activity_result_en.png
   :name: ngw_contribution_activity_result_pic
   :align: center
   :width: 16cm

   Example output image

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/ngw_contribution_activity/ngw_contribution_activity_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/ngw_contribution_activity/ngw_contribution_activity_outputs.zip>`_ of the tool run.

.. admonition:: Related tools

   * `Get the history of a vector feature <https://toolbox.nextgis.com/t/ngw_feature_history>`_
   * `Web GIS structure into spreadsheet <https://toolbox.nextgis.com/t/web_gis_structure>`_