Check KPT (Cadastral register) batches 
=======================================

This tool validates cadastral register batches, sorts them and provides reports on files. Sorting helps to discern duplicates, declines and confirmations. If you select "Renaming", every file will have the cadastral number added to its name (*cadastral number* + '_' + *original file number*). Select "Zipping" to get an archive containing the sorted files and a CSV file of the report. If this option is disabled, the tool only returns CSV report file.

Inputs:

* ZIP file - zip archive containing KPT batch
* Rename - change file names in the archive
* Zipping - return archive with sorted files

.. note::
    Uploaded zip archive can have one of the following structures:
    1) archive has one folder containing KPT files;
    2) archive contains KPT files.
    The names of the archive and the folder within (if the first structure is used) must only contain plain latin characters. 

Outputs:

* CSV file of the report if "Zipping" is disabled;
* ZIP file containing sorted KPT files and a CSV report file if "Zipping" is enabled.

In the report the "Status" field can have one of three values: OK, Double, Declined. *OK* means that the file is verified, it has a cadastral number and the query response in it. *Double* means that the file with the same cadastral number has already been processed, so all the following files with the same number will me marked as doubles. The first file will have the OK status, all the other will be marked Double. If the "zipping" option is enabled, the archived files will be sorted the same way. *Declined* status is for the files that have a query returned negative or files that have no cadastral number in them.

In most cases, if "Zipping" is disabled, the "Renaming" option does not affect the output.

Launch tool: https://toolbox.nextgis.com/operation/kptbatch_validator
