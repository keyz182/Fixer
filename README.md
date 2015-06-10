#Fixer

A shared Google Drive folder got Cryptolocker'ed. This runs through all the files with a .encrypted extension, and reverts them to the last good revision.

You need to create credentials for the Google Drive API, and populate them in src/main/resources/client_secret.json before running.

Processes up to 2000 files per run. If you have more files than that, either re-run the application, or increase ```setMaxResults()``` to a higher number.
