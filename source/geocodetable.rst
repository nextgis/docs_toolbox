Geocode a table
===============

Add two coordinates for every address in the input table.

Inputs:

*  CSV file - input data in CSV format, first row is for field names. Encoding - UTF-8.
*  Address field name - name of the table field that contains addresses.
*  API key 

Currently two geocoding services are supported:

1. Google Geocoding API (see https://developers.google.com/maps/documentation/geocoding/usage-and-billing)
2. Yandex.Geocoder service API key (JavaScript API and HTTP Geocoder), get one here: https://developer.tech.yandex.ru/services/. All limitations apply.

Outputs:

*  Input CSV file + two additional field containinf latitude and longitude for each address.

Launch tool: https://toolbox.nextgis.com/operation/geocodetable
