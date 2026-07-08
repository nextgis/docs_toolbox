Geotag photos using GPX track
=====================================

Use timing information to assign coordinates to photos matching them with a GPX track. Coordinates are added to EXIF tags. If your camera doesn't store coordinates or does so incorrectly, you can match photos made while recording a track by using timestamps.

Input:

* GPX file
* ZIP with photos

The tool can process photos with or without EXIF tags. Existing tags will be replaced with new ones.

Output:

* ZIP with photos that have new EXIF tags


Launch instrument: https://toolbox.nextgis.com/t/gpx2exif

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Merge GPX files <https://toolbox.nextgis.com/t/gpxmerge?from-related-tools=1>`_
  * `Photos with EXIF to NGW layer <https://toolbox.nextgis.com/t/exif2resource?from-related-tools=1>`_