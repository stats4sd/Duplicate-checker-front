# Duplicate Checker demo
This polymer 2.0 application is a front-end to a system built to run data quality checks on ODK form submissions.  The rough setup is:

1. Your ODK aggregate server is setup with a webhook, so all data is posted to a specific Server
2. That server contains a node.js app (going up onto Github shortly) that reads the form data.
3. The node.js app compares the new data with the previous submissions and sends an email notification if it spots a Duplicate
4. The form data is posted to a Firebase database, which powers this app.

## This app
This app shows the set of duplicates present in the submitted dataset, along with extra details that might (in theory) help a project supervisor track down the source of the duplicate data and resolve the issue.

--
Based on the Polymer App Toolbox starter kit.
