# Reference
Collects data via cronjob and submits to an s3 bucket

# Variables
```
# local_path - temporarily stores data for transfer to s3 - example:
/var/spool/data-to-s3

# s3_path - example:
s3://somebucket/somedirectory

# data_source_url - example:
https://some_url_here.xyz/a-dynamic-data-source?format=json

# fname_pattern - a string to use within the filename default cron is fname_pattern-datetime.fext - example:
webdata

# fext - an extension for the downloaded files - example:
json

# data_user, the user to pull and push the data via cron
# requires user exists, has configured aws cli - example:
chad

# target, the inventory host to perform the operation - example:
somehost1u

# for data sources, see https://github.com/jdorfman/awesome-json-datasets
```
