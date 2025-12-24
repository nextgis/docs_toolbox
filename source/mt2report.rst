Create marine traffic report
============================

This tool generates a table (format - CSV), which lists the ships entering given territory, the date and coordinates of their last location, as well as the number of times each ship entered a given territory for a certain period of time. It makes sense to use this tool, if you have already configured a service that updates data on ship locations in your Web GIS.

Inputs:

* **Web GIS** - URL of your Web GIS (for example, http(s)://mywebgis.nextgis.com)
* **Login** - login of a user with permission to write data in the resource
* **Password** - password for the user
* **AOI resource ID** - ID of a polygon layer in Web GIS representing the area of interest
* **Ship data resource ID** - ID of a point layer in Web GIS containing data on ships
* **Start date** - Starting date for ship data selection (e.g., 2019-09-22)

Calculation algorithm: Uploading layers of the boundary of the analysis zone and ship locations. Checking each location for intersection with the analysis zone; locations registered later than the specified starting date are also selected. Among the selected locations for each ship the last location and its coordinates, as well as the total number of locations are obtained. The information obtained for each ship is recorded in a table. 

The result of the process is a table in CSV format with information about all ships registered on a given territory later than the specified date, information about the last registered location and the number of registered locations within a given territory for a certain period of time.

Launch the tool: https://toolbox.nextgis.com/t/mt2report




**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.
