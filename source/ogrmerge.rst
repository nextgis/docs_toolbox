Merge vector layers
===================
   
The tool merges many vector layers into one. Layers should be of same geometry type.

Inputs:

* ZIP archive with SHP, GeoJSON, GeoPackage or MapInfo TAB layers. You can combine files of different formats and coordinate reference systems together in one set. Subfolders in the archive are supported.

Outputs:

* GeoPackage file with the result of the merge.

The tool has no limit on the number of input layers. The name of the source layer is stored in the attributes.

Launch tool: https://toolbox.nextgis.com/operation/ogrmerge

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/ogrmerge/ogrmerge_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/ogrmerge/ogrmerge_outputs.zip>`_ to additionally check the results.
