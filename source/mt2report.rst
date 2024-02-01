Create marine traffic report
============================

This tool generates a table (format - CSV), which lists the ships entering given territory, the date and coordinates of their last location, as well as the number of times each ship entered a given territory for a certain period of time. It makes sense to use this tool, if you have already configured a service that updates data on ship locations in your Web GIS.

Inputs:

* name - Web GIS Name
* layer_id_border - zone resource ID
* layer_id_ships - ship data resource ID
* date - Start date

Calculation algorithm: Uploading layers of the boundary of the analysis zone and ship locations. Checking each location for intersection with the analysis zone; locations registered later than the specified starting date are also selected. Among the selected locations for each ship the last location and its coordinates, as well as the total number of locations are obtained. The information obtained for each ship is recorded in a table. 

The result of the process is a table in CSV format with information about all ships registered on a given territory later than the specified date, information about the last registered location and the number of registered locations within a given territory for a certain period of time.

Launch tool: https://toolbox.nextgis.com/operation/mt2report

View an example of initial data on an interactive map: https://demo.nextgis.com/resource/4693/display?panel=layers

.. figure:: _static/mt2report_map.png
   :align: center
   :width: 16cm
   
   Initial Data Example
   
.. figure:: _static/mt2report_table.png
   :align: center
   :width: 16cm
   
   An example of the result of the tool’s usage 
