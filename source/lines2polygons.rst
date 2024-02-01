Temporal polygons from lines and points
=======================================

The tool creates polygons that reflect the state of the area at a particular point in time. Polygons are formed from a set of polylines, each of which is characterized by the start and end dates of its existence. Attributes for polygons are assigned from a layer of points, which also has a time reference.

In addition, grouping of polygon identifiers by a given parameter is carried out by creating a separate field with an ID common to each group (its minimum value). The geometry of the polygons does not change.

Inputs:

*  gis_url - address of the used Web GIS
*  lines_id - ID of the polyline layer from the used Web GIS
*  points_id - ID of the layer with points from the used Web GIS
*  Requested year - the year for which you want to get a time slice
*  year_field - name of the field where the requested year will be written
*  Result field - a new field where the grouping results will be entered, that is, ID
*  Field with identifiers - a field with unique values in the polyline layer; IDs for grouping are borrowed from it 
*  Grouping field - the field by which polygons are grouped

Outputs:

*  a layer with polygons (shapefile) relevant for the given year

Launch tool: https://toolbox.nextgis.com/operation/lines2polygons

Usage example:

What are the borders of Russia for the 1598th year AD?

*  gis_url - https://demo.nextgis.com
*  lines_id - 6747 (as the address of the layer with polylines https://demo.nextgis.com/resource/6747/feature/)
*  points_id - 6749 (since the address of the layer with points is https://demo.nextgis.com/resource/6749/feature/)
*  The requested year - 1598
*  year_field - Year
*  Result Field - Result
*  Field with identifiers - fid 
*  Grouping field - linecmnt
 
.. figure:: _static/lines2polygons_lines_points_map2.png
   :align: center
   :width: 16cm
   
   Sample input data. Layers of polylines and dots 
   
.. figure:: _static/lines2polygons_lines_table2.png
   :align: center
   :width: 16cm
   
   Sample input data. Polyline Layer Attributes Table  
   
.. figure:: _static/lines2polygons_polygons_map_table2.png
   :align: center
   :width: 16cm
   
   An example of the result of a tool    
