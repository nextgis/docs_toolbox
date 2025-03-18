Copernicus Sentinel image search
===================================


The tool generates a list of Sentinel scenes in the Copernicus archive that match the specified parameters.

Inputs:

* **Image search area** ``Required field`` - GeoJSON file with one polygon covering the area of interest;
* **Start date**, in dd.mm.yyyy format - scenes produced before that date won't be included;
* **End date**, in dd.mm.yyyy format - scenes produced after that date won't be included;
* **Service username** ``Required field`` - your username on https://scihub.copernicus.eu website;
* **Service password** ``Required field`` - your password for https://scihub.copernicus.eu website;
* **Mission** ``Required field`` - Enter one of the mission names: ``Sentinel-1``, ``Sentinel-2``, ``Sentinel-3``;
* **Product type** - depends on the chosen mission:

  * For Sentinel-1 choose from: ``RAW``, ``SLC``, ``GRD``, ``OCN``; 
  * For Sentinel-2: ``RAW``, ``S2MSI1C``, ``S2MSI2A``, ``S2MSI2Ap``;
  * For Sentinel-3: ``RAW``, ``OL_1_EFR___``, ``OL_1_ERR___``, ``SR_1_SRA___``, ``SR_1_SRA_A_``, ``SR_1_SRA_BS``, ``SR_2_LAN___``, ``SL_1_RBT___``, ``SL_2_LST___``, ``SY_2_SYN___``, ``SY_2_V10___``, ``SY_2_VG1___``, ``SY_2_VGP___``, ``OL_2_LFR___``, ``OL_2_LRR___``;

* **Polarisation mode** - Only for Sentinel-1, enter one of the following: ``HH, VV, HV, VH, HH+HV, VV+VH``. For Sentinel-2 or Sentinel-3 leave this field empty;
* **Sensor mode** - Only for Sentinel-1, enter one of the following: ``SM, IW, EW, WV``. For Sentinel-2 or Sentinel-3 leave this field empty;
* **Cloud cover** - Only for Sentinel-2. Specify acceptable range of cloud cover with two numbers (min and max percentage), separated by comma. E.g. ``0, 20``.

Outputs:

* XLSX file containing a list of scene IDs.

Launch tool: https://toolbox.nextgis.com/t/imagesearch

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/imagesearch/imagesearch_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/imagesearch/imagesearch_outputs.zip>`_ to additionally check the results.
