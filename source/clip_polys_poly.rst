Intersection areas inside/outside boundary
==========================================

Calculates area of polygons and area of polygons inside boundary. Areas calculated in hectares (ha)
Module was created for registration of wildfires in natural protected area. Internal calculations use local UTM zones, so calculations will accurate for any places on Earth.

Inputs:

*  nextgisweb url, login and password
*  nextgisweb layer id of boundary polygonal layer. Layer should have 1 feature, with polygon or multipolygon geometry
*  nextgisweb layer id of feature polygonal layer. Layer should have 2 fields for area calculations results.

Outputs:

*  Areas values will write into fields of layers in nextgisweb




Launch tool: https://toolbox.nextgis.com/operation/clip_polys_poly

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/clip_polys_poly/clip_polys_poly_inputs.zip>`_ to test the instrument. Step-by-step instructions included.
