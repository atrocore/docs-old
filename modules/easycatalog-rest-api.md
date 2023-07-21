# EasyCatalog: Rest API

For EasyCatalog Integration, there are 2 rest apis that are available to export and import data, one in `Import Feeds` module and the other in `Export Feeds` module.


## Rest api in `Export Feeds` Module

To use this api, you need an active exportFeed with a valid code. Then you can do a `GET` request to `/api/v1/ExportFeed/action/EasyCatalog?code=ExportFeedCode&offset=0`.
This will return data configured in the ExportFeed.

![Export Rest Api Example](_assets/easycatalog-rest-api/export-api-example.png)

## Rest api in `Import Feeds` Module

To use this api, you need an active importFeed with a valid code. Then you can do a `POST` request to `/api/v1/ImportFeed/action/EasyCatalog`. 
In the body of the request we have 2 parameters.

- `code` – the importFeed code
- `json` – an array of object that contains values to update

![Import Rest Api Example](_assets/easycatalog-rest-api/import-api-example.png)