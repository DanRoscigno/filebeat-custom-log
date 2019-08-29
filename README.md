# filebeat-custom-log

something like:

Customers will often have logs or other text that needs to be ingested, but there is no module for.  The sequence might look something like this:

 - Read the file in with no configuration other than pointing Filebeat at the file
 - Look at the results in Kibana -> Discover
 - See that the individual lines of the file end up in the `message` field
 - Decide that parsing of the log entries into individual fields would be nice
 - Setup a pipeline that maps the data in the log entries to fields in Elastic Common Schema
 - Create some visualizations and a dashboard
 - Happy Dance time
