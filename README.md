# sample-apps-stu3
This modifies the SMART on FHIR fhir-downloader sample to better work with the OpenEMR Bulk Export process. The sample downloader does not respect the content-disposition file-name and so we append the type of the Entity exported.

Also OpenEMR does not allow system/*.* scope access which the fhir-downloader requires.  We modified the downloader in order to support specifying the scopes both at the command line and inside the config file.  Read up on the fhir downloader by going here:

(FHIR Downloader)[fhir-downloader/README.md]
Collection of simple sample apps
