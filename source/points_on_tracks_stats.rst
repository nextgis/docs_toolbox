Statistics of points and tracks in polygons from NGW
====================================================

Calculating the number of points per kilometer of tracks inside polygons, all data from NextGIS Web


Inputs:

*  Web GIS address. Example: https://sandbox.nextgis.com
*  Web GIS user login
*  Web GIS user password
*  Resource ID of the vector layer that contains polygons
*  Name of the field with the name in the polygon layer. The names of the polygons (for example, area names or grid cell numbers) will be used in the report
*  Resource ID of the vector layer that contains points
*  Fields with point categories. You can specify multiple attributes separated by commas, for example: author,species. Leave the input blank if you do not need to use point categories for calculations
*  The name of the field that stores the date the point was registered. Leave blank if you do not need to filter points by date
*  Start date for filtering tracks and points. Recorded in the format yyyy-mm-dd, for example 2024-02-01. Leave input empty to use tracks from first day of database
*  End date for filtering tracks and points. Recorded in the format yyyy-mm-dd, for example 2024-02-01. Leave input empty to use all tracks up to today
*  List of trackers whose data needs to be processed. Tracker IDs are written in comma-separated format, for example 314,318,340. Leave blank to use all available trackers
*  Checkbox - Split statistics by trackers. Use tracker ID as another category for calculating statistics
*  Checkbox - Ignore polygons without tracks. Do not include statistics when there are points in polygon, but no tracks

Output:

* CSV file with report

The ID of resources and trackers can be obtained through the web interface of the Web GIS used. Open the resource of the vector layer or tracker, its address in the browser will look like https://demo.nextgis.com/resource/6895. ID is the number on the right side of the address, in this case 6895 

Tool workflow:

1. Loading vector layers with polygons and points from Web GIS
2. Loading data from all (or specified) trackers from Web GIS
3. Calculating track lengths in each polygon, with or without division by individual trackers, depending on the launch parameters
4. Calculating the number of points in each polygon, with or without division by categories from attributes, depending on the launch parameters
5. Calculating statistics on the number of points per 1 km of tracks in each polygon, taking into account all previous divisions - by individual trackers or by all, by all points or with division by categories
6. Generating a report

Launch tool: https://toolbox.nextgis.com/operation/points_on_tracks_stats

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/points_on_tracks_stats/points_on_tracks_stats_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/points_on_tracks_stats/points_on_tracks_stats_outputs.zip>`_ to additionally check the results.
   
