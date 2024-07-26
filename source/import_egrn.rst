EGRN data import
================

Convert official cadaster documents from EGRN into geodata package. Supports batch mode.

Supported formats: KPT (cadastral register): extract_cadastral_plan_territory_v01 and KPT_v10, KVZU (cadastral excerpt): KVZU_v07, ОКС: KVOKS_v03.


Inputs:

* Source file - XML file or ZIP archive, containing a batch of XML. Subarchives are supported.
* Data format - output data format, GPKG, GeoJSON, ESRI Shapefile or MapInfo File. If left blank, GPKG will be used.
* Identifier - Name to be used in the names of output files. If empty, "converted" is used.
* Merge datasets - Merge layers of same type derived from different XML files (initial result of conversion will also be preserved). We do not recommend this option for MapInfo File format.
* Do not transform coordinates - Leave objects in their initial CRS, without transforming into WGS84.
* Ignore objects without geometry - Skip entries in the XML documents that don't have geometry (coordinates).
* Remove empty attributes - Attributes that have no data even for a one object will be removed.
* Convert additional data - Sometimes XML docs have a special section ReestrExtract, containing additional information, e.g. ownership. If the option is enabled, such data will be added to separate layers without geometry.

Outputs:

* ZIP archive, containing converted files. 

Launch tool: https://toolbox.nextgis.com/operation/import_egrn

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/import_egrn/import_egrn_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/import_egrn/import_egrn_outputs.zip>`_ to additionally check the results.
