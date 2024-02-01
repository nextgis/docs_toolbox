Rosreestr extracts to map
=========================

The tool converts extracts from `Rosreestr <https://rosreestr.gov.ru>`_ to web map with one-direction sync. During next runs script detects changes in vector features and updates or appends new features. Features are not deleted. 


Input:

*  Rosreestr extract - one xml or zip
*  Web GIS link, example: https://sandbox.nextgis.com
*  Administrator or other Web GIS user login. User must have writing access
*  User password
*  Resource group id for data. User must create group only before very first run

Output:

* Layers and web map.

Launch tool: https://toolbox.nextgis.com/operation/Dezhurcad
