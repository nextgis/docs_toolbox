Projection (Dae, Collada) to Shapefile
======================================

The tool makes a projection of three-dimensional features on the earth's surface.

Inputs:

* Zip archive containing * .kmz and * .dae files
* *.kmz must contain the geolocation of * .dae models (coordinates of polygons in EPSG: 4326, units of measurement are metric)

Outputs:

*  A zip archive with Shapefile
*  In the resulting Shapefile for each model, the attributes “name” and “altitude” are added

You can submit several models, each of them gets a separate polygon.

Launch tool: https://toolbox.nextgis.com/operation/kmldae2footprints

Download an example of initial data and calculation results: https://nextgis.ru/data/toolbox/kmldae2footprints/kmldae2footprints.zip
