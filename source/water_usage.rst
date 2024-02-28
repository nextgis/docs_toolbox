Convert data on water objects
==============================

The tool processes data from the State water register: extracts geodata from XLSX file (available for download from https://voda.gov.ru/activities/gosudarstvennyy-vodnyy-reestr/) and forms GeoPackage with vector data.

Inputs:

* Source file - XLSX file, downloaded from https://voda.gov.ru/activities/gosudarstvennyy-vodnyy-reestr/ 
* Object number — unique number of the object from the State water register. Optional field, if a number is specified, the output will contain data only about target object.
* Region of Russia - Optional field. If region is specified, the output will contain data only about this region. Field “Object number“ takes precedence over current field. Basically it means that only one optional field should be filled in at a time.

Output:
                                                                                        
* GeoPackage file with water marks on water objects and attributes from the source file.

Launch the tool: https://toolbox.nextgis.com/operation/water_usage
