Add photos to an existing NGW layer
===================================

Add a set of photos to an existing layer by identifiers (FID - feature ID).

Inputs:

*  photos.zip - a compressed set with photos. A zip file should contain a set of folders, each containing 1 or more images. Folder name should be equal to FID of a feature to add photos too. Folders with photos should not be subfolders, i.e. compressed file should contain numbered folders. See example below for reference.
*  Web GIS link - address of a destination Web GIS https://sandbox.nextgis.com
*  Login - administrator or other Web GIS user login. User must have writing access
*  Password - Password for the user above
*  layer_id - Layer resource ID to which attachments will be added. Layer ID is the number that indicates the unique number of the resource in your Web GIS. For example, your vector layer resource link is https://demo.nextgis.com/resource/6273, layer_id in this case is 6273.

Outputs:

* Import report showing how many photos were uploaded successfuly.

Launch tool: https://toolbox.nextgis.com/operation/attach2resource

An example of source data: https://nextgis.ru/data/toolbox/attach2resource/attach2resource.zip
