Batch search by cadastral numbers
=================================

The tool creates a set of layers with the boundaries of cadastral objects, receiving as input a text file with a list of their numbers.
Requires access to `geoservices <https://geoservices.nextgis.com/settings/profile>`_. Auth via my.nextgis.com (NextGIS ID)

Input:

* API-key from https://geoservices.nextgis.com/settings/profile (Settings -> Profile)
* Text file (*.txt) containing numbers of items. One cadastral number per string. Max 100 numbers.

Output:

* Archive with geodata of cadastral objects

Launch tool: https://toolbox.nextgis.com/operation/cadnums_to_geodata

An example of source data and result: https://nextgis.ru/data/toolbox/cadnums_to_geodata/cadnums_to_geodata.zip
