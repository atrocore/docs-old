# Import Feeds: Database

This module extends the functionality of the module `Import Feeds` and enables you to automate import process by importing files from a certain database in the web.

> Module `Import Feeds` is required for this module to work.

## Importing database

To import database go to `Import Feeds` and select `Create Import Feed` option. There select `Database` type. Proseed threw other steps as usual untill `IMPORT DATA SETTINGS` tab.

![create](_assets/import-feeds-database/import-feeds-database-create.png)

## Import data settings tab

Here you have to first select `Connection` - select existing or create one.

`Header Row`, `Field Delimiter *` and `Text Qualifier *` are the same as in all import feeds. Proceed threw them as usual.

`Query *` is an SQL request to your database. Use it to select information you want to get.

![create](_assets/import-feeds-database/import-feeds-database-settings.png)

### Connection menu

Here you can select established connections or create a new one. Use name, `Host` and `Port` to locate it and  `User` and `Password` (of your database) for the system to get access to it.

![create](_assets/import-feeds-database/import-feeds-database-connection.png)