Check batch of KPT
=======================================

This tool analyzes XML files with KPT (cadastre data) in order to reveal duplicates and rejected requests. A report upon analysis will be formed as CSV file.

Inputs:

* KPT set - ZIP-archive containing several XML files.
* Create archive - if the box is checked, besides CSV new archive with sorted files will be created.
* Rename - If creation of an archive is chosen, files in the new archive will be renamed. Assigned name will be made of cadastre number and initial name of the file.

Outputs:

* CSV file with report. 
* Optional - ZIP-archive containing sorted XML files.

Launch tool: https://toolbox.nextgis.com/operation/kptbatch_validator
