Rosreestr extracts to map
=========================

The tool converts extracts from `Rosreestr <https://rosreestr.gov.ru>`_ to web map with one-direction sync. During next runs script detects changes in vector features and updates or appends new features if the extract has a later date. Features are not deleted. 

.. important:: Only features with recognized SRS are displayed on the map. Features will not be displayed if they are without geometry, SRS could not be determineded, coordinates do not correspond to the SRS specified in XML file, or they not fall within the boundaries of cadastral unit. The number of missed/processed features is displayed in the form of a report.


Input:

*  Rosreestr extract - one xml or zip
*  Web GIS link, example: https://sandbox.nextgis.com
*  Administrator or other Web GIS user login. User must have writing access
*  User password
*  Resource group id for data. User must create group only before very first run

Output:

* Layers and web map.

Launch the tool: https://toolbox.nextgis.com/t/Dezhurcad

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.


