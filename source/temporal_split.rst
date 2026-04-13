Create temporal cache
=====================

The tool creates several layers from one. Each new layer is a selection of features for a period of time.

Inputs:

* Web GIS URL, example: https://demo.nextgis.com;
* Input resource ID - numbers at the end of the URL of the input layer;
* Date the feature disappeared - field containing the date when the feature stopped existing;
* Date the feature appeared - field containing the date when the feature started existing;
* The start year of the interval - name for the 'year1' field (the field will be created);
* The end year of the interval - name for the 'year2' field (the field will be created);
* Output format - enter one of the following: ``GeoJSON, GPKG, CSV, ESRI Shapefile``. ESRI Shapefile is the default;
* Ignore errors - Leave empty to **stop execution** if an empty time slice is found. Enter 1 to **ignore** time slices with no features (ignore errors).

Outputs:

*  ZIP archive of layers, each also in an archive.

Launch the tool: https://toolbox.nextgis.com/t/temporal_split

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.
